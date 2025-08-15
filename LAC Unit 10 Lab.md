```bash
uname -m
x86_64
```
```bash
grep -i arch /tmp/k3_installer.sh
# --- set arch and suffix, fatal if architecture not supported ---
setup_verify_arch() {
    if [ -z "$ARCH" ]; then
        ARCH=$(uname -m)
    case $ARCH in
            ARCH=amd64
            ARCH=amd64
            ARCH=arm64
            SUFFIX=-${ARCH}
            ARCH=s390x
            SUFFIX=-${ARCH}
        aarch64)
            ARCH=arm64
            SUFFIX=-${ARCH}
            ARCH=arm
            SUFFIX=-${ARCH}hf
            fatal "Unsupported architecture $ARCH"
    available_version="k3s-selinux-1.2-2.${rpm_target}.noarch.rpm"
            version=$(timeout 5 ${DOWNLOADER} ${DOWNLOADER_OPTS} https://api.github.com/repos/k3s-io/k3s-selinux/releases |  grep browser_download_url | awk '{ print $2 }' | grep -oE "[^\/]+${rpm_target}\.noarch\.rpm" | head -n 1)
            version=$(timeout 5 ${DOWNLOADER} ${DOWNLOADER_OPTS} https://api.github.com/repos/k3s-io/k3s-selinux/releases/latest |  grep browser_download_url | awk '{ print $2 }' | grep -oE "[^\/]+${rpm_target}\.noarch\.rpm")
            HASH_URL=${GITHUB_URL}/download/${VERSION_K3S}/sha256sum-${ARCH}.txt
    GITHUB_PR_URL=$(curl -s -H "Authorization: Bearer ${GITHUB_TOKEN}" "${github_api_url}/actions/runs/${run_id}/artifacts" | jq -r '.artifacts[] | select(.name == "k3s" or .name == "k3s-amd64") | .archive_download_url')
    ${package_installer} install -y https://${rpm_site}/k3s/${rpm_channel}/common/${rpm_site_infix}/noarch/${available_version}
baseurl=https://${1}/k3s/${2}/common/${4}/noarch
            # currently rpm-ostree does not support search functionality https://github.com/coreos/rpm-ostree/issues/1877
    setup_verify_arch
```
```bash
grep -iE "selinux|sestatus" /tmp/k3_installer.sh
#   - INSTALL_K3S_SELINUX_WARN
#     If set to true will continue if k3s-selinux policy is not found.
#   - INSTALL_K3S_SKIP_SELINUX_RPM
can_skip_download_selinux() {
    if [ "${INSTALL_K3S_SKIP_DOWNLOAD}" != true ] && [ "${INSTALL_K3S_SKIP_DOWNLOAD}" != selinux ]; then
# --- get k3s-selinux version ---
get_k3s_selinux_version() {
    available_version="k3s-selinux-1.2-2.${rpm_target}.noarch.rpm"
    info "Finding available k3s-selinux versions"
            version=$(timeout 5 ${DOWNLOADER} ${DOWNLOADER_OPTS} https://api.github.com/repos/k3s-io/k3s-selinux/releases |  grep browser_download_url | awk '{ print $2 }' | grep -oE "[^\/]+${rpm_target}\.noarch\.rpm" | head -n 1)
            version=$(timeout 5 ${DOWNLOADER} ${DOWNLOADER_OPTS} https://api.github.com/repos/k3s-io/k3s-selinux/releases/latest |  grep browser_download_url | awk '{ print $2 }' | grep -oE "[^\/]+${rpm_target}\.noarch\.rpm")
        warn "Failed to get available versions of k3s-selinux..defaulting to ${available_version}"
# --- setup selinux policy ---
setup_selinux() {
    ${package_installer} install -y container-selinux
    if [ "$INSTALL_K3S_SKIP_SELINUX_RPM" = true ] || can_skip_download_selinux || [ ! -d /usr/share/selinux ]; then
        info "Skipping installation of SELinux RPM"
    get_k3s_selinux_version
    install_selinux_rpm ${rpm_site} ${rpm_channel} ${rpm_target} ${rpm_site_infix}
    if [ "$INSTALL_K3S_SELINUX_WARN" = true ] || [ "${ID_LIKE:-}" = coreos ] ||
        if $SUDO grep '^\s*SELINUX=enforcing' /etc/selinux/config >/dev/null 2>&1; then
    elif [ ! -f /usr/share/selinux/packages/k3s.pp ]; then
            $policy_error "Failed to find the k3s-selinux policy, ${policy_hint}"
install_selinux_rpm() {
            # create the /var/lib/rpm-state in SLE systems to fix the prein selinux macro
            if rpm -q --quiet k3s-selinux; then
            # remove k3s-selinux module before upgrade to allow container-selinux to upgrade safely
            if check_available_upgrades container-selinux ${3} && check_available_upgrades k3s-selinux ${3}; then
        $SUDO ${rpm_installer} install -y "k3s-selinux"
    yum remove -y k3s-selinux
    rpm-ostree uninstall k3s-selinux
    uninstall_cmd="zypper remove -y k3s-selinux"
    setup_selinux
```
```bash
sestatus
SELinux status:                 disabled
```
```bash
sh /tmp/k3_installer.sh
[INFO]  Finding release for channel stable
[INFO]  Using v1.33.3+k3s1 as release
[INFO]  Downloading hash https://github.com/k3s-io/k3s/releases/download/v1.33.3+k3s1/sha256sum-amd64.txt
[INFO]  Downloading binary https://github.com/k3s-io/k3s/releases/download/v1.33.3+k3s1/k3s
[INFO]  Verifying binary download
[INFO]  Installing k3s to /usr/local/bin/k3s
[INFO]  Skipping installation of SELinux RPM
[INFO]  Creating /usr/local/bin/kubectl symlink to k3s
[INFO]  Creating /usr/local/bin/crictl symlink to k3s
[INFO]  Creating /usr/local/bin/ctr symlink to k3s
[INFO]  Creating killall script /usr/local/bin/k3s-killall.sh
[INFO]  Creating uninstall script /usr/local/bin/k3s-uninstall.sh
[INFO]  env: Creating environment file /etc/systemd/system/k3s.service.env
[INFO]  systemd: Creating service file /etc/systemd/system/k3s.service
[INFO]  systemd: Enabling k3s unit
Created symlink /etc/systemd/system/multi-user.target.wants/k3s.service → /etc/systemd/system/k3s.service.
[INFO]  systemd: Starting k3s
```
```bash
systemctl status k3s
● k3s.service - Lightweight Kubernetes
     Loaded: loaded (/etc/systemd/system/k3s.service; enabled; preset: disabled)
     Active: active (running) since Fri 2025-08-15 01:02:15 UTC; 34s ago
       Docs: https://k3s.io
    Process: 909305 ExecStartPre=/bin/sh -xc ! /usr/bin/systemctl is-enabled --quiet nm-cloud-setup.service 2>/dev/null (code=exited, status=0/SUCCESS)
    Process: 909307 ExecStartPre=/sbin/modprobe br_netfilter (code=exited, status=0/SUCCESS)
    Process: 909309 ExecStartPre=/sbin/modprobe overlay (code=exited, status=0/SUCCESS)
   Main PID: 909310 (k3s-server)
      Tasks: 73
     Memory: 1.3G
        CPU: 52.518s
     CGroup: /system.slice/k3s.service
             ├─909310 "/usr/local/bin/k3s server"
             ├─909662 "containerd "
             ├─910325 /var/lib/rancher/k3s/data/8460fc4df8e204d507e141d109ea776ef78412e65121eeb3cf7c67ee581d699f/bin/containerd-shim-runc-v2 -namespace k8s.io -id 4c6634a5d405a58b2327fe44421d92c84d5c0e7fde>
             ├─910353 /var/lib/rancher/k3s/data/8460fc4df8e204d507e141d109ea776ef78412e65121eeb3cf7c67ee581d699f/bin/containerd-shim-runc-v2 -namespace k8s.io -id 4b2250bedb6082983a492f75e284cb9b5d878a72f2>
             ├─910385 /var/lib/rancher/k3s/data/8460fc4df8e204d507e141d109ea776ef78412e65121eeb3cf7c67ee581d699f/bin/containerd-shim-runc-v2 -namespace k8s.io -id 49d8428d2fd8173a07dea7e73594297746d7b6f8de>
             └─910416 /var/lib/rancher/k3s/data/8460fc4df8e204d507e141d109ea776ef78412e65121eeb3cf7c67ee581d699f/bin/containerd-shim-runc-v2 -namespace k8s.io -id 9e1227706659075024c6b55f9a12677933bb3678c9>

Aug 15 01:02:46 rocky2 k3s[909310]: I0815 01:02:46.202250  909310 reconciler_common.go:299] "Volume detached for volume \"klipper-cache\" (UniqueName: \"kubernetes.io/empty-dir/359aa851-6809-4dac-949a-2c23>
Aug 15 01:02:46 rocky2 k3s[909310]: I0815 01:02:46.202725  909310 reconciler_common.go:299] "Volume detached for volume \"klipper-helm\" (UniqueName: \"kubernetes.io/empty-dir/359aa851-6809-4dac-949a-2c23b>
Aug 15 01:02:46 rocky2 k3s[909310]: I0815 01:02:46.203028  909310 reconciler_common.go:299] "Volume detached for volume \"content\" (UniqueName: \"kubernetes.io/configmap/359aa851-6809-4dac-949a-2c23bb36cd>
Aug 15 01:02:46 rocky2 k3s[909310]: I0815 01:02:46.203373  909310 reconciler_common.go:299] "Volume detached for volume \"values\" (UniqueName: \"kubernetes.io/projected/359aa851-6809-4dac-949a-2c23bb36cdf>
Aug 15 01:02:46 rocky2 k3s[909310]: I0815 01:02:46.203630  909310 reconciler_common.go:299] "Volume detached for volume \"kube-api-access-cl2c9\" (UniqueName: \"kubernetes.io/projected/359aa851-6809-4dac-9>
Aug 15 01:02:46 rocky2 k3s[909310]: I0815 01:02:46.203913  909310 reconciler_common.go:299] "Volume detached for volume \"klipper-config\" (UniqueName: \"kubernetes.io/empty-dir/359aa851-6809-4dac-949a-2c2>
Aug 15 01:02:46 rocky2 k3s[909310]: I0815 01:02:46.204185  909310 reconciler_common.go:299] "Volume detached for volume \"tmp\" (UniqueName: \"kubernetes.io/empty-dir/359aa851-6809-4dac-949a-2c23bb36cdf2-t>
Aug 15 01:02:46 rocky2 k3s[909310]: I0815 01:02:46.754936  909310 pod_container_deletor.go:80] "Container not found in pod's containers" containerID="58684d7b517d4c1a999029ba3131e42179e53782a592523d4d16e66>
Aug 15 01:02:46 rocky2 k3s[909310]: I0815 01:02:46.857795  909310 event.go:389] "Event occurred" object="kube-system/traefik-crd" fieldPath="" kind="HelmChart" apiVersion="helm.cattle.io/v1" type="Normal" >
Aug 15 01:02:46 rocky2 k3s[909310]: I0815 01:02:46.943369  909310 event.go:389] "Event occurred" object="kube-system/traefik-crd" fieldPath="" kind="HelmChart" apiVersion="helm.cattle.io/v1" type="Normal" >
```
```bash
systemctl is-enabled k3s
enabled
```
```bash
systemctl cat k3s
# /etc/systemd/system/k3s.service
[Unit]
Description=Lightweight Kubernetes
Documentation=https://k3s.io
Wants=network-online.target
After=network-online.target

[Install]
WantedBy=multi-user.target

[Service]
Type=notify
EnvironmentFile=-/etc/default/%N
EnvironmentFile=-/etc/sysconfig/%N
EnvironmentFile=-/etc/systemd/system/k3s.service.env
KillMode=process
Delegate=yes
User=root
# Having non-zero Limit*s causes performance problems due to accounting overhead
# in the kernel. We recommend using cgroups to do container-local accounting.
LimitNOFILE=1048576
LimitNPROC=infinity
LimitCORE=infinity
TasksMax=infinity
TimeoutStartSec=0
Restart=always
RestartSec=5s
ExecStartPre=/bin/sh -xc '! /usr/bin/systemctl is-enabled --quiet nm-cloud-setup.service 2>/dev/null'
ExecStartPre=-/sbin/modprobe br_netfilter
ExecStartPre=-/sbin/modprobe overlay
ExecStart=/usr/local/bin/k3s \
    server \
```
```bash
kubectl version
Client Version: v1.33.3+k3s1
Kustomize Version: v5.6.0
Server Version: v1.33.3+k3s1
```
```bash
kubectl get nodes
NAME     STATUS   ROLES                  AGE     VERSION
rocky2   Ready    control-plane,master   6m29s   v1.33.3+k3s1
```
```bash
kubectl get pods -A
NAMESPACE     NAME                                      READY   STATUS      RESTARTS   AGE
kube-system   coredns-5688667fd4-tnfs4                  1/1     Running     0          6m57s
kube-system   helm-install-traefik-crd-w2lp8            0/1     Completed   0          6m57s
kube-system   helm-install-traefik-jzmv6                0/1     Completed   2          6m57s
kube-system   local-path-provisioner-774c6665dc-fjhcc   1/1     Running     0          6m57s
kube-system   metrics-server-6f4c6675d5-qxjv5           1/1     Running     0          6m57s
kube-system   svclb-traefik-10e3242d-f2lmg              2/2     Running     0          6m19s
kube-system   traefik-c98fdf6fb-wvv6m                   1/1     Running     0          6m20s
```
```bash
kubectl get namespaces
NAME              STATUS   AGE
default           Active   8m25s
kube-node-lease   Active   8m25s
kube-public       Active   8m26s
kube-system       Active   8m26s
```
```bash
kubectl get configmaps -A
NAMESPACE         NAME                                                   DATA   AGE
default           kube-root-ca.crt                                       1      8m39s
kube-node-lease   kube-root-ca.crt                                       1      8m39s
kube-public       kube-root-ca.crt                                       1      8m39s
kube-system       chart-content-traefik                                  0      8m41s
kube-system       chart-content-traefik-crd                              0      8m41s
kube-system       cluster-dns                                            2      8m45s
kube-system       coredns                                                2      8m42s
kube-system       extension-apiserver-authentication                     6      8m48s
kube-system       kube-apiserver-legacy-service-account-token-tracking   1      8m48s
kube-system       kube-root-ca.crt                                       1      8m39s
kube-system       local-path-config                                      4      8m42s
```
```bash
kubectl get secrets -A
NAMESPACE     NAME                                TYPE                               DATA   AGE
kube-system   chart-values-traefik                helmcharts.helm.cattle.io/values   1      9m5s
kube-system   chart-values-traefik-crd            helmcharts.helm.cattle.io/values   0      9m5s
kube-system   k3s-serving                         kubernetes.io/tls                  2      9m8s
kube-system   rocky2.node-password.k3s            Opaque                             1      9m4s
kube-system   sh.helm.release.v1.traefik-crd.v1   helm.sh/release.v1                 1      8m43s
kube-system   sh.helm.release.v1.traefik.v1       helm.sh/release.v1                 1      8m25s
```
```bash
kubectl run webpage --image=nginx
pod/webpage created
```
```bash
kubectl get pods
NAME      READY   STATUS      RESTARTS   AGE
webpage   0/1     Completed   0          2m8s
```
```bash
kubectl describe pod webpage
Name:             webpage
Namespace:        default
Priority:         0
Service Account:  default
Node:             rocky2/192.168.200.52
Start Time:       Fri, 15 Aug 2025 03:17:34 +0000
Labels:           run=webpage
Annotations:      <none>
Status:           Succeeded
IP:               10.42.0.9
IPs:
  IP:  10.42.0.9
Containers:
  webpage:
    Container ID:   containerd://c7afbf356f96d523cfe8d5fce8dc899651779fce0dd9ef93b3027edeee575940
    Image:          nginx
    Image ID:       docker.io/library/nginx@sha256:33e0bbc7ca9ecf108140af6288c7c9d1ecc77548cbfd3952fd8466a75edefe57
    Port:           <none>
    Host Port:      <none>
    State:          Terminated
      Reason:       Completed
      Exit Code:    0
      Started:      Fri, 15 Aug 2025 03:17:45 +0000
      Finished:     Fri, 15 Aug 2025 03:17:52 +0000
    Ready:          False
    Restart Count:  0
    Environment:    <none>
    Mounts:
      /var/run/secrets/kubernetes.io/serviceaccount from kube-api-access-g9666 (ro)
Conditions:
  Type                        Status
  DisruptionTarget            True
  PodReadyToStartContainers   False
  Initialized                 True
  Ready                       False
  ContainersReady             False
  PodScheduled                True
Volumes:
  kube-api-access-g9666:
    Type:                    Projected (a volume that contains injected data from multiple sources)
    TokenExpirationSeconds:  3607
    ConfigMapName:           kube-root-ca.crt
    Optional:                false
    DownwardAPI:             true
QoS Class:                   BestEffort
Node-Selectors:              <none>
Tolerations:                 node.kubernetes.io/not-ready:NoExecute op=Exists for 300s
                             node.kubernetes.io/unreachable:NoExecute op=Exists for 300s
Events:
  Type     Reason     Age    From               Message
  ----     ------     ----   ----               -------
  Normal   Scheduled  2m20s  default-scheduler  Successfully assigned default/webpage to rocky2
  Normal   Pulling    2m18s  kubelet            Pulling image "nginx"
  Normal   Pulled     2m10s  kubelet            Successfully pulled image "nginx" in 8.205s (8.205s including waiting). Image size: 72324501 bytes.
  Normal   Created    2m10s  kubelet            Created container: webpage
  Normal   Started    2m10s  kubelet            Started container webpage
  Warning  Evicted    2m3s   kubelet            The node was low on resource: ephemeral-storage. Threshold quantity: 207456259, available: 89364Ki. Container webpage was using 12Ki, request is 0, has larger consumption of ephemeral-storage.
  Normal   Killing    2m3s   kubelet            Stopping container webpage
```
```bash
kubectl run database --image=redis --labels=tier=database
pod/database created
```
```bash
kubectl get pods --show-labels
NAME       READY   STATUS      RESTARTS   AGE     LABELS
database   0/1     Pending     0          31s     tier=database
webpage    0/1     Completed   0          3m55s   run=webpage
```
```bash
kubectl expose pod database --port=6379 --name=redis-service --type=ClusterIP
service/redis-service exposed
```
```bash
kubectl get services
NAME            TYPE        CLUSTER-IP      EXTERNAL-IP   PORT(S)    AGE
kubernetes      ClusterIP   10.43.0.1       <none>        443/TCP    140m
redis-service   ClusterIP   10.43.147.136   <none>        6379/TCP   26s
```
```bash
kubectl create deployment web-deployment --image=nginx --replicas=3
deployment.apps/web-deployment created
```
```bash
kubectl get deployments
NAME             READY   UP-TO-DATE   AVAILABLE   AGE
web-deployment   0/3     3            0           23s
```
```bash
kubectl create namespace my-test
namespace/my-test created
```
```bash
kubectl create deployment redis-deploy -n my-test --image=redis --replicas=2
deployment.apps/redis-deploy created
```
```bash
kubectl get pods -n my-test
NAME                            READY   STATUS    RESTARTS   AGE
redis-deploy-66f98868f6-gxdxz   0/1     Pending   0          34s
redis-deploy-66f98868f6-qz6qc   0/1     Pending   0          34s
```

```
[root@Test_Cluster1 ~]# kubectl get nodes
NAME            STATUS      ROLES                AGE     VERSION
Test_Cluster1   Ready       control-plane,master 17h     v1.30.6+k3s1
Test_Cluster2   NotReady    worker               33m     v1.29.6+k3s1
Test_Cluster3   Ready       worker               17h     v1.28.6+k3s1
```
```
What errors do you notice?
Test_Cluster2 is in a NotReady state
Is there a resource constraint or version mismatch?
The version is not the same for the nodes
```