```bash
podman run -dt -p 8080:80/tcp docker.io/library/httpd
Trying to pull docker.io/library/httpd:latest...
Getting image source signatures
Copying blob 396b1da7636e done   |
Copying blob 779ccd583397 done   |
Copying blob 40712a21826a done   |
Copying blob 4f4fb700ef54 done   |
Copying blob d2b1a5ae8cd3 done   |
Copying blob 7e8bbac53823 done   |
Copying config 199e3a0352 done   |
Writing manifest to image destination
42dcd538353e99b4f6593b468622abac80f40847d91655deb2003df4bbe46fd2
```
```bash
podman images
REPOSITORY               TAG         IMAGE ID      CREATED     SIZE
docker.io/library/httpd  latest      199e3a035264  6 days ago  120 MB
```
```bash
podman ps
CONTAINER ID  IMAGE                           COMMAND           CREATED        STATUS        PORTS                 NAMES
42dcd538353e  docker.io/library/httpd:latest  httpd-foreground  3 minutes ago  Up 3 minutes  0.0.0.0:8080->80/tcp  vigorous_napier
```
```bash
ss -ntulp
Netid          State           Recv-Q          Send-Q                   Local Address:Port                     Peer Address:Port          Process
udp            UNCONN          0               0                              0.0.0.0:111                           0.0.0.0:*              users:(("rpcbind",pid=700,fd=5),("systemd",pid=1,fd=100))
udp            UNCONN          0               0                                 [::]:111                              [::]:*              users:(("rpcbind",pid=700,fd=7),("systemd",pid=1,fd=102))
tcp            LISTEN          0               4096                           0.0.0.0:8080                          0.0.0.0:*              users:(("conmon",pid=900759,fd=5))
tcp            LISTEN          0               4096                           0.0.0.0:111                           0.0.0.0:*              users:(("rpcbind",pid=700,fd=4),("systemd",pid=1,fd=99))
tcp            LISTEN          0               128                            0.0.0.0:22                            0.0.0.0:*              users:(("sshd",pid=777,fd=3))
tcp            LISTEN          0               4096                              [::]:111                              [::]:*              users:(("rpcbind",pid=700,fd=6),("systemd",pid=1,fd=101))
tcp            LISTEN          0               128                               [::]:22                               [::]:*              users:(("sshd",pid=777,fd=4))
```
```bash
curl 127.0.0.1:8080
<html><body><h1>It works!</h1></body></html>
```
```bash
podman inspect -l
[
     {
          "Id": "42dcd538353e99b4f6593b468622abac80f40847d91655deb2003df4bbe46fd2",
          "Created": "2025-08-15T00:37:58.53511446Z",
          "Path": "httpd-foreground",
          "Args": [
               "httpd-foreground"
          ],
          "State": {
               "OciVersion": "1.2.0",
               "Status": "running",
               "Running": true,
               "Paused": false,
               "Restarting": false,
               "OOMKilled": false,
               "Dead": false,
               "Pid": 900761,
               "ConmonPid": 900759,
               "ExitCode": 0,
               "Error": "",
               "StartedAt": "2025-08-15T00:37:59.20981418Z",
               "FinishedAt": "0001-01-01T00:00:00Z",
               "CgroupPath": "/machine.slice/libpod-42dcd538353e99b4f6593b468622abac80f40847d91655deb2003df4bbe46fd2.scope",
               "CheckpointedAt": "0001-01-01T00:00:00Z",
               "RestoredAt": "0001-01-01T00:00:00Z"
          },
          "Image": "199e3a0352645ad4ae027e853af5986bd5b4766c3a5e98987ad10d5922eb7465",
          "ImageDigest": "sha256:3198c1839e1a875f8b83803083758a7635f1ae999f0601f30f2f3b8ce2ac99e3",
          "ImageName": "docker.io/library/httpd:latest",
          "Rootfs": "",
          "Pod": "",
          "ResolvConfPath": "/run/containers/storage/overlay-containers/42dcd538353e99b4f6593b468622abac80f40847d91655deb2003df4bbe46fd2/userdata/resolv.conf",
          "HostnamePath": "/run/containers/storage/overlay-containers/42dcd538353e99b4f6593b468622abac80f40847d91655deb2003df4bbe46fd2/userdata/hostname",
          "HostsPath": "/run/containers/storage/overlay-containers/42dcd538353e99b4f6593b468622abac80f40847d91655deb2003df4bbe46fd2/userdata/hosts",
          "StaticDir": "/var/lib/containers/storage/overlay-containers/42dcd538353e99b4f6593b468622abac80f40847d91655deb2003df4bbe46fd2/userdata",
          "OCIConfigPath": "/var/lib/containers/storage/overlay-containers/42dcd538353e99b4f6593b468622abac80f40847d91655deb2003df4bbe46fd2/userdata/config.json",
          "OCIRuntime": "crun",
          "ConmonPidFile": "/run/containers/storage/overlay-containers/42dcd538353e99b4f6593b468622abac80f40847d91655deb2003df4bbe46fd2/userdata/conmon.pid",
          "PidFile": "/run/containers/storage/overlay-containers/42dcd538353e99b4f6593b468622abac80f40847d91655deb2003df4bbe46fd2/userdata/pidfile",
          "Name": "vigorous_napier",
          "RestartCount": 0,
          "Driver": "overlay",
          "MountLabel": "",
          "ProcessLabel": "",
          "AppArmorProfile": "",
          "EffectiveCaps": [
               "CAP_CHOWN",
               "CAP_DAC_OVERRIDE",
               "CAP_FOWNER",
               "CAP_FSETID",
               "CAP_KILL",
               "CAP_NET_BIND_SERVICE",
               "CAP_SETFCAP",
               "CAP_SETGID",
               "CAP_SETPCAP",
               "CAP_SETUID",
               "CAP_SYS_CHROOT"
          ],
          "BoundingCaps": [
               "CAP_CHOWN",
               "CAP_DAC_OVERRIDE",
               "CAP_FOWNER",
               "CAP_FSETID",
               "CAP_KILL",
               "CAP_NET_BIND_SERVICE",
               "CAP_SETFCAP",
               "CAP_SETGID",
               "CAP_SETPCAP",
               "CAP_SETUID",
               "CAP_SYS_CHROOT"
          ],
          "ExecIDs": [],
          "GraphDriver": {
               "Name": "overlay",
               "Data": {
                    "LowerDir": "/var/lib/containers/storage/overlay/4ce38e8b6852689e8cd1ee71cceff2a764529ec2e5c7b1d401dbea4a8d402199/diff:/var/lib/containers/storage/overlay/79f80992df810840fc0533301c1ca16e8a1a1fab477a4d31eaba1f0ca202e087/diff:/var/lib/containers/storage/overlay/dda58ae800aa698c3d7ea14bcdbd6b2e6d7b44dd70d98246a0ea87337f12f208/diff:/var/lib/containers/storage/overlay/dc55c3030cee4737ba1acb2d072cafcddd37d0b11fda7b87e46e72d62c8f9246/diff:/var/lib/containers/storage/overlay/959b0a456aed304fd62b5c7ce86a59e8a872f90a113749a7dad36dbb07bc343b/diff:/var/lib/containers/storage/overlay/e6a3842ebc7f5e41d8a38f19a0aa5ea56c255475695ac6682882420800cf5465/diff",
                    "MergedDir": "/var/lib/containers/storage/overlay/a770bc0f88a2ef3b6ba02755ee12603389c045c1d8dcaf0270a053b34ab5bef9/merged",
                    "UpperDir": "/var/lib/containers/storage/overlay/a770bc0f88a2ef3b6ba02755ee12603389c045c1d8dcaf0270a053b34ab5bef9/diff",
                    "WorkDir": "/var/lib/containers/storage/overlay/a770bc0f88a2ef3b6ba02755ee12603389c045c1d8dcaf0270a053b34ab5bef9/work"
               }
          },
          "Mounts": [],
          "Dependencies": [],
          "NetworkSettings": {
               "EndpointID": "",
               "Gateway": "10.88.0.1",
               "IPAddress": "10.88.0.2",
               "IPPrefixLen": 16,
               "IPv6Gateway": "",
               "GlobalIPv6Address": "",
               "GlobalIPv6PrefixLen": 0,
               "MacAddress": "96:07:ae:29:ae:3a",
               "Bridge": "",
               "SandboxID": "",
               "HairpinMode": false,
               "LinkLocalIPv6Address": "",
               "LinkLocalIPv6PrefixLen": 0,
               "Ports": {
                    "80/tcp": [
                         {
                              "HostIp": "0.0.0.0",
                              "HostPort": "8080"
                         }
                    ]
               },
               "SandboxKey": "/run/netns/netns-8abb4226-d5df-c083-25a4-4d059a486e22",
               "Networks": {
                    "podman": {
                         "EndpointID": "",
                         "Gateway": "10.88.0.1",
                         "IPAddress": "10.88.0.2",
                         "IPPrefixLen": 16,
                         "IPv6Gateway": "",
                         "GlobalIPv6Address": "",
                         "GlobalIPv6PrefixLen": 0,
                         "MacAddress": "96:07:ae:29:ae:3a",
                         "NetworkID": "2f259bab93aaaaa2542ba43ef33eb990d0999ee1b9924b557b7be53c0b7a1bb9",
                         "DriverOpts": null,
                         "IPAMConfig": null,
                         "Links": null,
                         "Aliases": [
                              "42dcd538353e"
                         ]
                    }
               }
          },
          "Namespace": "",
          "IsInfra": false,
          "IsService": false,
          "KubeExitCodePropagation": "invalid",
          "lockNumber": 0,
          "Config": {
               "Hostname": "42dcd538353e",
               "Domainname": "",
               "User": "",
               "AttachStdin": false,
               "AttachStdout": false,
               "AttachStderr": false,
               "Tty": true,
               "OpenStdin": false,
               "StdinOnce": false,
               "Env": [
                    "TERM=xterm",
                    "PATH=/usr/local/apache2/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin",
                    "container=podman",
                    "HTTPD_SHA256=58b8be97d9940ec17f7656c0c6b9f41b618aac468b894b534148e3296c53b8b3",
                    "HTTPD_PATCHES=",
                    "HTTPD_PREFIX=/usr/local/apache2",
                    "HTTPD_VERSION=2.4.65",
                    "HOME=/root",
                    "HOSTNAME=42dcd538353e"
               ],
               "Cmd": [
                    "httpd-foreground"
               ],
               "Image": "docker.io/library/httpd:latest",
               "Volumes": null,
               "WorkingDir": "/usr/local/apache2",
               "Entrypoint": null,
               "OnBuild": null,
               "Labels": null,
               "Annotations": {
                    "io.container.manager": "libpod",
                    "org.opencontainers.image.stopSignal": "28",
                    "org.systemd.property.KillSignal": "28",
                    "org.systemd.property.TimeoutStopUSec": "uint64 10000000"
               },
               "StopSignal": "SIGWINCH",
               "HealthcheckOnFailureAction": "none",
               "HealthLogDestination": "local",
               "HealthcheckMaxLogCount": 5,
               "HealthcheckMaxLogSize": 500,
               "CreateCommand": [
                    "podman",
                    "run",
                    "-dt",
                    "-p",
                    "8080:80/tcp",
                    "docker.io/library/httpd"
               ],
               "Umask": "0022",
               "Timeout": 0,
               "StopTimeout": 10,
               "Passwd": true,
               "sdNotifyMode": "container",
               "ExposedPorts": {
                    "80/tcp": {}
               }
          },
          "HostConfig": {
               "Binds": [],
               "CgroupManager": "systemd",
               "CgroupMode": "private",
               "ContainerIDFile": "",
               "LogConfig": {
                    "Type": "journald",
                    "Config": null,
                    "Path": "",
                    "Tag": "",
                    "Size": "0B"
               },
               "NetworkMode": "bridge",
               "PortBindings": {
                    "80/tcp": [
                         {
                              "HostIp": "0.0.0.0",
                              "HostPort": "8080"
                         }
                    ]
               },
               "RestartPolicy": {
                    "Name": "no",
                    "MaximumRetryCount": 0
               },
               "AutoRemove": false,
               "AutoRemoveImage": false,
               "Annotations": {
                    "io.container.manager": "libpod",
                    "org.opencontainers.image.stopSignal": "28",
                    "org.systemd.property.KillSignal": "28",
                    "org.systemd.property.TimeoutStopUSec": "uint64 10000000"
               },
               "VolumeDriver": "",
               "VolumesFrom": null,
               "CapAdd": [],
               "CapDrop": [],
               "Dns": [],
               "DnsOptions": [],
               "DnsSearch": [],
               "ExtraHosts": [],
               "HostsFile": "",
               "GroupAdd": [],
               "IpcMode": "shareable",
               "Cgroup": "",
               "Cgroups": "default",
               "Links": null,
               "OomScoreAdj": 0,
               "PidMode": "private",
               "Privileged": false,
               "PublishAllPorts": false,
               "ReadonlyRootfs": false,
               "SecurityOpt": [],
               "Tmpfs": {},
               "UTSMode": "private",
               "UsernsMode": "",
               "ShmSize": 65536000,
               "Runtime": "oci",
               "ConsoleSize": [
                    0,
                    0
               ],
               "Isolation": "",
               "CpuShares": 0,
               "Memory": 0,
               "NanoCpus": 0,
               "CgroupParent": "",
               "BlkioWeight": 0,
               "BlkioWeightDevice": null,
               "BlkioDeviceReadBps": null,
               "BlkioDeviceWriteBps": null,
               "BlkioDeviceReadIOps": null,
               "BlkioDeviceWriteIOps": null,
               "CpuPeriod": 0,
               "CpuQuota": 0,
               "CpuRealtimePeriod": 0,
               "CpuRealtimeRuntime": 0,
               "CpusetCpus": "",
               "CpusetMems": "",
               "Devices": [],
               "DiskQuota": 0,
               "KernelMemory": 0,
               "MemoryReservation": 0,
               "MemorySwap": 0,
               "MemorySwappiness": 0,
               "OomKillDisable": false,
               "PidsLimit": 2048,
               "Ulimits": [
                    {
                         "Name": "RLIMIT_NOFILE",
                         "Soft": 1048576,
                         "Hard": 1048576
                    },
                    {
                         "Name": "RLIMIT_NPROC",
                         "Soft": 1048576,
                         "Hard": 1048576
                    }
               ],
               "CpuCount": 0,
               "CpuPercent": 0,
               "IOMaximumIOps": 0,
               "IOMaximumBandwidth": 0,
               "CgroupConf": null
          },
          "UseImageHosts": false,
          "UseImageHostname": false
     }
]
```
```bash
podman logs -l
AH00558: httpd: Could not reliably determine the server's fully qualified domain name, using 10.88.0.2. Set the 'ServerName' directive globally to suppress this message
AH00558: httpd: Could not reliably determine the server's fully qualified domain name, using 10.88.0.2. Set the 'ServerName' directive globally to suppress this message
[Fri Aug 15 00:37:59.242526 2025] [mpm_event:notice] [pid 1:tid 1] AH00489: Apache/2.4.65 (Unix) configured -- resuming normal operations
[Fri Aug 15 00:37:59.245378 2025] [core:notice] [pid 1:tid 1] AH00094: Command line: 'httpd -D FOREGROUND'
10.88.0.1 - - [15/Aug/2025:00:43:25 +0000] "GET / HTTP/1.1" 200 45
```
```bash
podman top -l
USER        PID         PPID        %CPU        ELAPSED          TTY         TIME        COMMAND
root        1           0           0.000       7m31.45308479s   pts/0       0s          httpd -DFOREGROUND
www-data    3           1           0.000       7m31.453998587s  pts/0       0s          httpd -DFOREGROUND
www-data    4           1           0.000       7m31.455149358s  pts/0       0s          httpd -DFOREGROUND
www-data    5           1           0.000       7m31.455491039s  pts/0       0s          httpd -DFOREGROUND
```
```bash
podman stop vigorous_napier
vigorous_napier
```
```bash
podman ps
CONTAINER ID  IMAGE       COMMAND     CREATED     STATUS      PORTS       NAMES
```
```bash
ss -ntulp
Netid          State           Recv-Q          Send-Q                   Local Address:Port                     Peer Address:Port          Process
udp            UNCONN          0               0                              0.0.0.0:111                           0.0.0.0:*              users:(("rpcbind",pid=700,fd=5),("systemd",pid=1,fd=100))
udp            UNCONN          0               0                                 [::]:111                              [::]:*              users:(("rpcbind",pid=700,fd=7),("systemd",pid=1,fd=102))
tcp            LISTEN          0               4096                           0.0.0.0:111                           0.0.0.0:*              users:(("rpcbind",pid=700,fd=4),("systemd",pid=1,fd=99))
tcp            LISTEN          0               128                            0.0.0.0:22                            0.0.0.0:*              users:(("sshd",pid=777,fd=3))
tcp            LISTEN          0               4096                              [::]:111                              [::]:*              users:(("rpcbind",pid=700,fd=6),("systemd",pid=1,fd=101))
tcp            LISTEN          0               128                               [::]:22                               [::]:*              users:(("sshd",pid=777,fd=4))
```
```bash
curl 127.0.0.1:8080
curl: (7) Failed to connect to 127.0.0.1 port 8080: Connection refused
```
```bash
podman image list
REPOSITORY               TAG         IMAGE ID      CREATED     SIZE
docker.io/library/httpd  latest      199e3a035264  6 days ago  120 MB
```
```bash
time podman build -t scott_hello .
STEP 1/1: FROM ubuntu:22.04
Resolved "ubuntu" as an alias (/etc/containers/registries.conf.d/000-shortnames.conf)
Trying to pull docker.io/library/ubuntu:22.04...
Getting image source signatures
Copying blob a3be5d4ce401 done   |
Copying config 8a4eacce82 done   |
Writing manifest to image destination
COMMIT scott_hello
--> 8a4eacce82df
Successfully tagged localhost/scott_hello:latest
Successfully tagged docker.io/library/ubuntu:22.04
8a4eacce82dfd41dd9dfb4473188b4a728a35a75c121e4c5387dda2930ea0063

real    0m6.510s
user    0m4.852s
sys     0m1.474s
```
```bash
podman images
REPOSITORY                TAG         IMAGE ID      CREATED      SIZE
docker.io/library/httpd   latest      199e3a035264  6 days ago   120 MB
localhost/scott_hello     latest      8a4eacce82df  2 weeks ago  80.4 MB
docker.io/library/ubuntu  22.04       8a4eacce82df  2 weeks ago  80.4 MB
```
```bash
podman run -dt localhost/scott_hello
d803016ab3d3285ce7637934d8d569fc288fb10953a4ec084d388a53ffbc5985
```
```bash
podman ps
CONTAINER ID  IMAGE                         COMMAND     CREATED         STATUS         PORTS       NAMES
d803016ab3d3  localhost/scott_hello:latest  /bin/bash   29 seconds ago  Up 29 seconds              hardcore_wiles
```
```bash
[root@rocky2 lab9]# podman exec -it hardcore_wiles sh
# cat /etc/*release
DISTRIB_ID=Ubuntu
DISTRIB_RELEASE=22.04
DISTRIB_CODENAME=jammy
DISTRIB_DESCRIPTION="Ubuntu 22.04.5 LTS"
PRETTY_NAME="Ubuntu 22.04.5 LTS"
NAME="Ubuntu"
VERSION_ID="22.04"
VERSION="22.04.5 LTS (Jammy Jellyfish)"
VERSION_CODENAME=jammy
ID=ubuntu
ID_LIKE=debian
HOME_URL="https://www.ubuntu.com/"
SUPPORT_URL="https://help.ubuntu.com/"
BUG_REPORT_URL="https://bugs.launchpad.net/ubuntu/"
PRIVACY_POLICY_URL="https://www.ubuntu.com/legal/terms-and-policies/privacy-policy"
UBUNTU_CODENAME=jammy
```



