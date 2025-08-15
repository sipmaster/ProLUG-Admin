```bash
more /etc/passwd
root:x:0:0:root:/root:/bin/bash
bin:x:1:1:bin:/bin:/sbin/nologin
daemon:x:2:2:daemon:/sbin:/sbin/nologin
adm:x:3:4:adm:/var/adm:/sbin/nologin
lp:x:4:7:lp:/var/spool/lpd:/sbin/nologin
sync:x:5:0:sync:/sbin:/bin/sync
shutdown:x:6:0:shutdown:/sbin:/sbin/shutdown
halt:x:7:0:halt:/sbin:/sbin/halt
mail:x:8:12:mail:/var/spool/mail:/sbin/nologin
operator:x:11:0:operator:/root:/sbin/nologin
games:x:12:100:games:/usr/games:/sbin/nologin
ftp:x:14:50:FTP User:/var/ftp:/sbin/nologin
nobody:x:65534:65534:Kernel Overflow User:/:/sbin/nologin
tss:x:59:59:Account used for TPM access:/:/usr/sbin/nologin
systemd-coredump:x:999:999:systemd Core Dumper:/:/sbin/nologin
dbus:x:81:81:System message bus:/:/sbin/nologin
rpc:x:32:32:Rpcbind Daemon:/var/lib/rpcbind:/sbin/nologin
rpcuser:x:29:29:RPC Service User:/var/lib/nfs:/sbin/nologin
sshd:x:74:74:Privilege-separated SSH:/usr/share/empty.sshd:/usr/sbin/nologin
polkitd:x:998:998:User for polkitd:/:/sbin/nologin
```
```bash
more /etc/group
root:x:0:
bin:x:1:
daemon:x:2:
sys:x:3:
adm:x:4:
tty:x:5:
disk:x:6:
lp:x:7:
mem:x:8:
kmem:x:9:
wheel:x:10:
cdrom:x:11:
mail:x:12:
man:x:15:
dialout:x:18:
floppy:x:19:
games:x:20:
tape:x:33:
video:x:39:
ftp:x:50:
lock:x:54:
audio:x:63:
users:x:100:
nobody:x:65534:
utmp:x:22:
utempter:x:35:
tss:x:59:
ssh_keys:x:101:
input:x:104:
kvm:x:36:
render:x:105:
sgx:x:106:
systemd-journal:x:190:
systemd-coredump:x:999:
dbus:x:81:
rpc:x:32:
rpcuser:x:29:
sshd:x:74:
polkitd:x:998:
screen:x:84:
```
```bash
more /etc/shadow
root:$6$rounds=100000$1234567890123456$78901234567890123456789.012345678901234567890123456789012345678901.2345678901234567//890:12345:6:99999:7:::
bin:*:19820:0:99999:7:::
daemon:*:19820:0:99999:7:::
adm:*:19820:0:99999:7:::
lp:*:19820:0:99999:7:::
sync:*:19820:0:99999:7:::
shutdown:*:19820:0:99999:7:::
halt:*:19820:0:99999:7:::
mail:*:19820:0:99999:7:::
operator:*:19820:0:99999:7:::
games:*:19820:0:99999:7:::
ftp:*:19820:0:99999:7:::
nobody:*:19820:0:99999:7:::
tss:!!:20239::::::
systemd-coredump:!!:20283::::::
dbus:!!:20283::::::
rpc:!!:20283:0:99999:7:::
rpcuser:!!:20283::::::
sshd:!!:20283::::::
polkitd:!!:20303::::::
```
```bash
more /etc/gshadow
root:::
bin:::
daemon:::
sys:::
adm:::
tty:::
disk:::
lp:::
mem:::
kmem:::
wheel:::
cdrom:::
mail:::
man:::
dialout:::
floppy:::
games:::
tape:::
video:::
ftp:::
lock:::
audio:::
users:::
nobody:::
utmp:!::
utempter:!::
tss:!::
ssh_keys:!::
input:!::
kvm:!::
render:!::
sgx:!::
systemd-journal:!::
systemd-coredump:!::
dbus:!::
rpc:!::
rpcuser:!::
sshd:!::
polkitd:!::
screen:!::
```
```bash
ls -l /etc/passwd
-rw-r--r-- 1 root root 950 Aug  3 06:36 /etc/passwd
```
```bash
ls -l /etc/group
-rw-r--r-- 1 root root 485 Aug 14 14:16 /etc/group
```
```bash
ls -l /etc/shadow
---------- 1 root root 628 Aug  7 23:23 /etc/shadow
```
```bash
ls -l /etc/gshadow
---------- 1 root root 380 Aug 14 14:16 /etc/gshadow
```
```bash
tail -5 /etc/passwd
sshd:x:74:74:Privilege-separated SSH:/usr/share/empty.sshd:/usr/sbin/nologin
polkitd:x:998:998:User for polkitd:/:/sbin/nologin
user1:x:1000:1000::/home/user1:/bin/bash
user2:x:1001:1001::/home/user2:/bin/bash
user3:x:1002:1002::/home/user3:/bin/bash
```
```bash
tail -5 /etc/shadow
sshd:!!:20283::::::
polkitd:!!:20303::::::
user1:!!:20314:0:99999:7:::
user2:!!:20314:0:99999:7:::
user3:!!:20314:0:99999:7:::
```
```bash
ls /home
alan  linuxengineer  user1  user2  user3  user4
```
```bash
tail -5 /etc/group
screen:x:84:
user1:x:1000:
user2:x:1001:
user3:x:1002:
project:x:60001:
```
```bash
id user4
uid=1003(user4) gid=1003(user4) groups=1003(user4),60002(project2)
```
```bash
tail -f /etc/group
rpcuser:x:29:
sshd:x:74:
polkitd:x:998:
screen:x:84:
user1:x:1000:
user2:x:1001:
user3:x:1002:
project:x:60001:user4
project2:x:60002:
user4:x:1003:
```
```bash
id user4
uid=1003(user4) gid=1003(user4) groups=1003(user4),60001(project)
id user1
uid=1000(user1) gid=1000(user1) groups=1000(user1),60001(project)
id user2
uid=1001(user2) gid=1001(user2) groups=1001(user2),60001(project)
```
```bash
ls -ld /project
drwxr-xr-x 2 root root 40 Aug 14 23:47 /project
```
```bash
ls -ld /project
drwxrwxr-x 2 root project 40 Aug 14 23:47 /project
```
