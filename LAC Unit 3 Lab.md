```bash
fdisk -l | grep -i xvd
Disk /dev/xvda: 15 GiB, 16106127360 bytes, 31457280 sectors
Disk /dev/xvdb: 3 GiB, 3221225472 bytes, 6291456 sectors
Disk /dev/xvdc: 3 GiB, 3221225472 bytes, 6291456 sectors
Disk /dev/xvde: 3 GiB, 3221225472 bytes, 6291456 sectors
```
```bash
for disk in b c e; do pvcreate /dev/xvd$disk; done
  Physical volume "/dev/xvdb" successfully created.
  Creating devices file /etc/lvm/devices/system.devices
  Physical volume "/dev/xvdc" successfully created.
  Physical volume "/dev/xvde" successfully created.
```
```bash
pvs
  PV         VG Fmt  Attr PSize PFree
  /dev/xvdb     lvm2 ---  3.00g 3.00g
  /dev/xvdc     lvm2 ---  3.00g 3.00g
  /dev/xvde     lvm2 ---  3.00g 3.00g
```
```bash
vgcreate VolGroupTest /dev/xvdb /dev/xvdc /dev/xvde
  Volume group "VolGroupTest" successfully created
```
```bash
vgs
  VG           #PV #LV #SN Attr   VSize  VFree
  VolGroupTest   3   0   0 wz--n- <8.99g <8.99g
```
```bash
lvcreate -l +100%FREE -n lv_test VolGroupTest
WARNING: ext4 signature detected on /dev/VolGroupTest/lv_test at offset 1080. Wipe it? [y/n]: y
  Wiping ext4 signature on /dev/VolGroupTest/lv_test.
  Logical volume "lv_test" created.
```
```bash
lvs
  LV      VG           Attr       LSize  Pool Origin Data%  Meta%  Move Log Cpy%Sync Convert
  lv_test VolGroupTest -wi-a----- <8.99g
```
```bash
mkfs.ext4 /dev/mapper/VolGroupTest-lv_test
mke2fs 1.46.5 (30-Dec-2021)
Creating filesystem with 2356224 4k blocks and 589824 inodes
Filesystem UUID: 431bc464-52df-4f56-a1f9-4bb9b85a48e7
Superblock backups stored on blocks:
        32768, 98304, 163840, 229376, 294912, 819200, 884736, 1605632

Allocating group tables: done
Writing inode tables: done
Creating journal (16384 blocks): done
Writing superblocks and filesystem accounting information: done
```
```bash
mount /space
df -h
Filesystem          Size  Used Avail Use% Mounted on
devtmpfs            4.0M     0  4.0M   0% /dev
tmpfs               3.9G     0  3.9G   0% /dev/shm
tmpfs               1.6G   17M  1.6G   2% /run
tmpfs               3.9G  2.2G  1.8G  56% /
tmpfs               3.9G     0  3.9G   0% /run/shm
warewulf:/labs      194G   67G  128G  35% /labs
warewulf:/opt       194G   67G  128G  35% /opt
warewulf:/home      194G   67G  128G  35% /home
warewulf:/lab_work  194G   67G  128G  35% /lab_work
tmpfs               792M     0  792M   0% /run/user/0
/dev/mapper/VolGroupTest-lv_test  8.8G   24K  8.3G   1% /space
```
```bash
grep lv_test /etc/fstab; perl -pi -e "s/\/dev\/mapper\/VolGroupTest/#removed \/dev\/mapper\/VolGroupTest/" /etc/fstab; grep removed /etc/fstab
/dev/mapper/VolGroupTest-lv_test /space ext4 defaults 0 0
#removed /dev/mapper/VolGroupTest-lv_test /space ext4 defaults 0 0
```
```bash
lvremove /dev/mapper/VolGroupTest-lv_test
Do you really want to remove active logical volume VolGroupTest/lv_test? [y/n]: y
  Logical volume "lv_test" successfully removed.
```
```bash
vgremove VolGroupTest
  Volume group "VolGroupTest" successfully removed
```
```bash
for disk in b c e; do pvremove /dev/xvd$disk; done
  Labels on physical volume "/dev/xvdb" successfully wiped.
  Labels on physical volume "/dev/xvdc" successfully wiped.
  Labels on physical volume "/dev/xvde" successfully wiped.
```
```bash
for disk in b c e ; do pvcreate /dev/xvd$disk; done
  Physical volume "/dev/xvdb" successfully created.
  Physical volume "/dev/xvdc" successfully created.
  Physical volume "/dev/xvde" successfully created.
```
```bash
vgcreate VolGroupTest /dev/xvdc /dev/xvde /dev/xvdb
  Volume group "VolGroupTest" successfully created
```
```bash
lvcreate -l +100%FREE --type raid5 -n lv_test VolGroupTest
  Using default stripesize 64.00 KiB.
  Rounding size (2301 extents) down to stripe boundary size (2300 extents)
  Logical volume "lv_test" created.
```
```bash
mkfs.xfs /dev/mapper/VolGroupTest-lv_test
meta-data=/dev/mapper/VolGroupTest-lv_test isize=512    agcount=8, agsize=196080 blks
         =                       sectsz=512   attr=2, projid32bit=1
         =                       crc=1        finobt=1, sparse=1, rmapbt=0
         =                       reflink=1    bigtime=1 inobtcount=1 nrext64=0
data     =                       bsize=4096   blocks=1568640, imaxpct=25
         =                       sunit=16     swidth=32 blks
naming   =version 2              bsize=4096   ascii-ci=0, ftype=1
log      =internal log           bsize=4096   blocks=16384, version=2
         =                       sectsz=512   sunit=16 blks, lazy-count=1
realtime =none                   extsz=4096   blocks=0, rtextents=0
```
```bash
df -h
Filesystem                        Size  Used Avail Use% Mounted on
devtmpfs                          4.0M     0  4.0M   0% /dev
tmpfs                             3.9G     0  3.9G   0% /dev/shm
tmpfs                             1.6G   17M  1.6G   2% /run
tmpfs                             3.9G  2.2G  1.8G  56% /
tmpfs                             3.9G     0  3.9G   0% /run/shm
warewulf:/labs                    194G   67G  128G  35% /labs
warewulf:/opt                     194G   67G  128G  35% /opt
warewulf:/home                    194G   67G  128G  35% /home
warewulf:/lab_work                194G   67G  128G  35% /lab_work
tmpfs                             792M     0  792M   0% /run/user/0
/dev/mapper/VolGroupTest-lv_test  6.0G   75M  5.9G   2% /space
```
```bash
lvs
  LV      VG           Attr       LSize Pool Origin Data%  Meta%  Move Log Cpy%Sync Convert
  lv_test VolGroupTest rwi-aor--- 5.98g
```
```bash
umount /space
lvremove /dev/mapper/VolGroupTest-lv_test
Do you really want to remove active logical volume VolGroupTest/lv_test? [y/n]: y
  Logical volume "lv_test" successfully removed.
```
```bash
vgremove VolGroupTest
  Volume group "VolGroupTest" successfully removed
```
```bash
for disk in c e b; do pvremove /dev/xvd$disk; done
  Labels on physical volume "/dev/xvdc" successfully wiped.
  Labels on physical volume "/dev/xvde" successfully wiped.
  Labels on physical volume "/dev/xvdb" successfully wiped.
```
```bash
mdadm --create -l raid5 /dev/md0 -n 3 /dev/xvdc /dev/xvde /dev/xvdb
mdadm: Defaulting to version 1.2 metadata
mdadm: array /dev/md0 started.
```
```bash
pvcreate /dev/md0
  Physical volume "/dev/md0" successfully created.
```
```bash
vgcreate VolGroupTest /dev/md0
  Volume group "VolGroupTest" successfully created
```
```bash
lvcreate -l +100%Free -n lv_test VolGroupTest
  Logical volume "lv_test" created.
```
```bash
lvs
  LV      VG           Attr       LSize Pool Origin Data%  Meta%  Move Log Cpy%Sync Convert
  lv_test VolGroupTest -wi-a----- 5.99g
```
```bash
mkfs.xfs /dev/mapper/VolGroupTest-lv_test
log stripe unit (524288 bytes) is too large (maximum is 256KiB)
log stripe unit adjusted to 32KiB
meta-data=/dev/mapper/VolGroupTest-lv_test isize=512    agcount=8, agsize=196224 blks
         =                       sectsz=512   attr=2, projid32bit=1
         =                       crc=1        finobt=1, sparse=1, rmapbt=0
         =                       reflink=1    bigtime=1 inobtcount=1 nrext64=0
data     =                       bsize=4096   blocks=1569792, imaxpct=25
         =                       sunit=128    swidth=256 blks
naming   =version 2              bsize=4096   ascii-ci=0, ftype=1
log      =internal log           bsize=4096   blocks=16384, version=2
         =                       sectsz=512   sunit=8 blks, lazy-count=1
realtime =none                   extsz=4096   blocks=0, rtextents=0
```
```bash
cat /etc/mdadm.conf
ARRAY /dev/md0 metadata=1.2 UUID=bbee437d:8e0c0039:0402e4e5:4a4970fe
```
```bash
df -h
Filesystem                        Size  Used Avail Use% Mounted on
devtmpfs                          4.0M     0  4.0M   0% /dev
tmpfs                             3.9G     0  3.9G   0% /dev/shm
tmpfs                             1.6G   17M  1.6G   2% /run
tmpfs                             3.9G  2.2G  1.8G  56% /
tmpfs                             3.9G     0  3.9G   0% /run/shm
warewulf:/labs                    194G   67G  128G  35% /labs
warewulf:/opt                     194G   67G  128G  35% /opt
warewulf:/home                    194G   67G  128G  35% /home
warewulf:/lab_work                194G   67G  128G  35% /lab_work
tmpfs                             792M     0  792M   0% /run/user/0
/dev/mapper/VolGroupTest-lv_test  6.0G   75M  5.9G   2% /space
```
```bash
umount /space
rm /etc/mdadm.conf
vgremove VolGroupTest
Do you really want to remove volume group "VolGroupTest" containing 1 logical volumes? [y/n]: y
Do you really want to remove active logical volume VolGroupTest/lv_test? [y/n]: y
  Logical volume "lv_test" successfully removed.
  Volume group "VolGroupTest" successfully removed
pvremove /dev/md0
  Labels on physical volume "/dev/md0" successfully wiped.
mdadm --stop md0
mdadm: stopped md0
mdadm --zero-superblock /dev/xvdb
mdadm --zero-superblock /dev/xvdc
mdadm --zero-superblock /dev/xvde
cat /proc/mdstat
Personalities : [raid6] [raid5] [raid4]
unused devices: <none>

https://bobcares.com/blog/removal-of-mdadm-raid-devices/
```




