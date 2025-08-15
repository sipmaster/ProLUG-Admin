```bash
cat /etc/*release
uname
uname -a
uname -r
NAME="Rocky Linux"
VERSION="9.6 (Blue Onyx)"
ID="rocky"
ID_LIKE="rhel centos fedora"
VERSION_ID="9.6"
PLATFORM_ID="platform:el9"
PRETTY_NAME="Rocky Linux 9.6 (Blue Onyx)"
ANSI_COLOR="0;32"
LOGO="fedora-logo-icon"
CPE_NAME="cpe:/o:rocky:rocky:9::baseos"
HOME_URL="https://rockylinux.org/"
VENDOR_NAME="RESF"
VENDOR_URL="https://resf.org/"
BUG_REPORT_URL="https://bugs.rockylinux.org/"
SUPPORT_END="2032-05-31"
ROCKY_SUPPORT_PRODUCT="Rocky-Linux-9"
ROCKY_SUPPORT_PRODUCT_VERSION="9.6"
REDHAT_SUPPORT_PRODUCT="Rocky Linux"
REDHAT_SUPPORT_PRODUCT_VERSION="9.6"
Rocky Linux release 9.6 (Blue Onyx)
Rocky Linux release 9.6 (Blue Onyx)
Rocky Linux release 9.6 (Blue Onyx)
Linux
Linux rocky2 5.14.0-570.25.1.el9_6.x86_64 #1 SMP PREEMPT_DYNAMIC Mon Jul 7 18:09:10 UTC 2025 x86_64 x86_64 x86_64 GNU/Linux
5.14.0-570.25.1.el9_6.x86_64
```
```bash
rpm -qa | grep -i kernel
kernel-modules-core-5.14.0-570.25.1.el9_6.x86_64
kernel-core-5.14.0-570.25.1.el9_6.x86_64
kernel-modules-5.14.0-570.25.1.el9_6.x86_64
kernel-srpm-macros-1.0-13.el9.noarch
kernel-headers-5.14.0-570.32.1.el9_6.x86_64

rpm -qi kernel-core
Name        : kernel-core
Version     : 5.14.0
Release     : 570.25.1.el9_6
Architecture: x86_64
Install Date: Mon Jul 14 21:25:55 2025
Group       : Unspecified
Size        : 70871354

License     : ((GPL-2.0-only WITH Linux-syscall-note) OR BSD-2-Clause) AND ((GPL-2.0-only WITH Linux-syscall-note) OR BSD-3-Clause) AND ((GPL-2.0-only WITH Linux-syscall-note) OR CDDL-1.0) AND ((GPL-2.0-only WITH Linux-syscall-note) OR Linux-OpenIB) AND ((GPL-2.0-only WITH Linux-syscall-note) OR MIT) AND ((GPL-2.0-or-later WITH Linux-syscall-note) OR BSD-3-Clause) AND ((GPL-2.0-or-later WITH Linux-syscall-note) OR MIT) AND Apache-2.0 AND BSD-2-Clause AND BSD-3-Clause AND BSD-3-Clause-Clear AND GFDL-1.1-no-invariants-or-later AND GPL-1.0-or-later AND (GPL-1.0-or-later OR BSD-3-Clause) AND (GPL-1.0-or-later WITH Linux-syscall-note) AND GPL-2.0-only AND (GPL-2.0-only OR Apache-2.0) AND (GPL-2.0-only OR BSD-2-Clause) AND (GPL-2.0-only OR BSD-3-Clause) AND (GPL-2.0-only OR CDDL-1.0) AND (GPL-2.0-only OR GFDL-1.1-no-invariants-or-later) AND (GPL-2.0-only OR GFDL-1.2-no-invariants-only) AND (GPL-2.0-only WITH Linux-syscall-note) AND GPL-2.0-or-later AND (GPL-2.0-or-later OR BSD-2-Clause) AND (GPL-2.0-or-later OR BSD-3-Clause) AND (GPL-2.0-or-later OR CC-BY-4.0) AND (GPL-2.0-or-later WITH GCC-exception-2.0) AND (GPL-2.0-or-later WITH Linux-syscall-note) AND ISC AND LGPL-2.0-or-later AND (LGPL-2.0-or-later OR BSD-2-Clause) AND (LGPL-2.0-or-later WITH Linux-syscall-note) AND LGPL-2.1-only AND (LGPL-2.1-only OR BSD-2-Clause) AND (LGPL-2.1-only WITH Linux-syscall-note) AND LGPL-2.1-or-later AND (LGPL-2.1-or-later WITH Linux-syscall-note) AND (Linux-OpenIB OR GPL-2.0-only) AND (Linux-OpenIB OR GPL-2.0-only OR BSD-2-Clause) AND Linux-man-pages-copyleft AND MIT AND (MIT OR GPL-2.0-only) AND (MIT OR GPL-2.0-or-later) AND (MIT OR LGPL-2.1-only) AND (MPL-1.1 OR GPL-2.0-only) AND (X11 OR GPL-2.0-only) AND (X11 OR GPL-2.0-or-later) AND Zlib

Signature   : RSA/SHA256, Tue Jul  8 02:49:00 2025, Key ID 702d426d350d275d
Source RPM  : kernel-5.14.0-570.25.1.el9_6.src.rpm
Build Date  : Mon Jul  7 17:06:26 2025
Build Host  : iad1-prod-build001.bld.equ.rockylinux.org
Packager    : Release Engineering <releng@rockylinux.org>
Vendor      : Rocky Enterprise Software Foundation
URL         : https://www.kernel.org/
Summary     : The Linux kernel
```
```bash
fdisk -l

Disk /dev/xvda: 15 GiB, 16106127360 bytes, 31457280 sectors
Units: sectors of 1 * 512 = 512 bytes
Sector size (logical/physical): 512 bytes / 512 bytes
I/O size (minimum/optimal): 512 bytes / 512 bytes

Disk /dev/xvdb: 3 GiB, 3221225472 bytes, 6291456 sectors
Units: sectors of 1 * 512 = 512 bytes
Sector size (logical/physical): 512 bytes / 512 bytes
I/O size (minimum/optimal): 512 bytes / 512 bytes

Disk /dev/xvdc: 3 GiB, 3221225472 bytes, 6291456 sectors
Units: sectors of 1 * 512 = 512 bytes
Sector size (logical/physical): 512 bytes / 512 bytes
I/O size (minimum/optimal): 512 bytes / 512 bytes

Disk /dev/xvde: 3 GiB, 3221225472 bytes, 6291456 sectors
Units: sectors of 1 * 512 = 512 bytes
Sector size (logical/physical): 512 bytes / 512 bytes
I/O size (minimum/optimal): 512 bytes / 512 bytes
```
```bash
ls /dev/xvd*
/dev/xvda  /dev/xvdb  /dev/xvdc  /dev/xvde
```
```bash
- When might this command be useful? To find what disks are connected on the system
- What are we assuming about the disks for this to work? They are connected 
- How many disks are there on this system? 4
- How do you know if it's a partition or a disk? a partition has a number
```
```bash
iostat -d
Linux 5.14.0-570.25.1.el9_6.x86_64 (rocky2)     08/14/25        _x86_64_        (2 CPU)

Device             tps    kB_read/s    kB_wrtn/s    kB_dscd/s    kB_read    kB_wrtn    kB_dscd
xvda              0.00         0.02         0.00         0.00       2828          0          0
xvdb              1.11        26.69        21.01         0.00    4172348    3283253          0
xvdc              1.11        46.85         1.08         0.00    7322910     169167          0
xvde              1.11        46.73         0.76         0.00    7303475     119527          0
```
```bash
iostat -d 2
Linux 5.14.0-570.25.1.el9_6.x86_64 (rocky2)     08/14/25        _x86_64_        (2 CPU)

Device             tps    kB_read/s    kB_wrtn/s    kB_dscd/s    kB_read    kB_wrtn    kB_dscd
xvda              0.00         0.02         0.00         0.00       2828          0          0
xvdb              1.11        26.69        21.00         0.00    4172732    3283253          0
xvdc              1.11        46.84         1.08         0.00    7323294     169167          0
xvde              1.11        46.71         0.76         0.00    7303859     119527          0


Device             tps    kB_read/s    kB_wrtn/s    kB_dscd/s    kB_read    kB_wrtn    kB_dscd
xvda              0.00         0.00         0.00         0.00          0          0          0
xvdb              0.00         0.00         0.00         0.00          0          0          0
xvdc              0.00         0.00         0.00         0.00          0          0          0
xvde              0.00         0.00         0.00         0.00          0          0          0
```
```bash
iostat -d 2 5
Linux 5.14.0-570.25.1.el9_6.x86_64 (rocky2)     08/14/25        _x86_64_        (2 CPU)

Device             tps    kB_read/s    kB_wrtn/s    kB_dscd/s    kB_read    kB_wrtn    kB_dscd
xvda              0.00         0.02         0.00         0.00       2828          0          0
xvdb              1.11        26.68        20.99         0.00    4173116    3283253          0
xvdc              1.11        46.82         1.08         0.00    7323678     169167          0
xvde              1.10        46.70         0.76         0.00    7304243     119527          0


Device             tps    kB_read/s    kB_wrtn/s    kB_dscd/s    kB_read    kB_wrtn    kB_dscd
xvda              0.00         0.00         0.00         0.00          0          0          0
xvdb              0.00         0.00         0.00         0.00          0          0          0
xvdc              0.00         0.00         0.00         0.00          0          0          0
xvde              0.00         0.00         0.00         0.00          0          0          0


Device             tps    kB_read/s    kB_wrtn/s    kB_dscd/s    kB_read    kB_wrtn    kB_dscd
xvda              0.00         0.00         0.00         0.00          0          0          0
xvdb              0.00         0.00         0.00         0.00          0          0          0
xvdc              0.00         0.00         0.00         0.00          0          0          0
xvde              0.00         0.00         0.00         0.00          0          0          0


Device             tps    kB_read/s    kB_wrtn/s    kB_dscd/s    kB_read    kB_wrtn    kB_dscd
xvda              0.00         0.00         0.00         0.00          0          0          0
xvdb              0.00         0.00         0.00         0.00          0          0          0
xvdc              0.00         0.00         0.00         0.00          0          0          0
xvde              0.00         0.00         0.00         0.00          0          0          0


Device             tps    kB_read/s    kB_wrtn/s    kB_dscd/s    kB_read    kB_wrtn    kB_dscd
xvda              0.00         0.00         0.00         0.00          0          0          0
xvdb              0.00         0.00         0.00         0.00          0          0          0
xvdc              0.00         0.00         0.00         0.00          0          0          0
xvde              0.00         0.00         0.00         0.00          0          0          0
```
```bash
cat /proc/meminfo
free
free -m
MemTotal:        8103760 kB
MemFree:         5498416 kB
MemAvailable:    5396240 kB
Buffers:               0 kB
Cached:          2262232 kB
SwapCached:            0 kB
Active:          2317136 kB
Inactive:              8 kB
Active(anon):    2317136 kB
Inactive(anon):        0 kB
Active(file):          0 kB
Inactive(file):        8 kB
Unevictable:           0 kB
Mlocked:               0 kB
SwapTotal:             0 kB
SwapFree:              0 kB
Zswap:                 0 kB
Zswapped:              0 kB
Dirty:                 0 kB
Writeback:             0 kB
AnonPages:         54912 kB
Mapped:            60128 kB
Shmem:           2262224 kB
KReclaimable:      61760 kB
Slab:             178528 kB
SReclaimable:      61760 kB
SUnreclaim:       116768 kB
KernelStack:        3248 kB
PageTables:         1860 kB
SecPageTables:         0 kB
NFS_Unstable:          0 kB
Bounce:                0 kB
WritebackTmp:          0 kB
CommitLimit:     4051880 kB
Committed_AS:    2556992 kB
VmallocTotal:   34359738367 kB
VmallocUsed:       21412 kB
VmallocChunk:          0 kB
Percpu:            25600 kB
HardwareCorrupted:     0 kB
AnonHugePages:     16384 kB
ShmemHugePages:        0 kB
ShmemPmdMapped:        0 kB
FileHugePages:         0 kB
FilePmdMapped:         0 kB
CmaTotal:              0 kB
CmaFree:               0 kB
Unaccepted:            0 kB
HugePages_Total:       0
HugePages_Free:        0
HugePages_Rsvd:        0
HugePages_Surp:        0
Hugepagesize:       2048 kB
Hugetlb:               0 kB
DirectMap4k:      346112 kB
DirectMap2M:     5937152 kB
DirectMap1G:     3145728 kB
               total        used        free      shared  buff/cache   available
Mem:         8103760     2707520     5498416     2262224     2323992     5396240
Swap:              0           0           0
               total        used        free      shared  buff/cache   available
Mem:            7913        2644        5369        2209        2269        5269
```
```bash
cat /proc/cpuinfo
processor       : 0
vendor_id       : GenuineIntel
cpu family      : 6
model           : 45
model name      : Intel(R) Xeon(R) CPU E5-2665 0 @ 2.40GHz
stepping        : 7
microcode       : 0x71a
cpu MHz         : 2400.018
cache size      : 20480 KB
physical id     : 0
siblings        : 1
core id         : 0
cpu cores       : 1
apicid          : 0
initial apicid  : 0
fpu             : yes
fpu_exception   : yes
cpuid level     : 13
wp              : yes
flags           : fpu vme de pse tsc msr pae mce cx8 apic sep mtrr pge mca cmov pat pse36 clflush acpi mmx fxsr sse sse2 ss ht syscall nx pdpe1gb rdtscp lm constant_tsc rep_good nopl cpuid tsc_known_freq pni pclmulqdq ssse3 cx16 pcid sse4_1 sse4_2 x2apic popcnt tsc_deadline_timer aes xsave avx hypervisor lahf_lm cpuid_fault pti ssbd ibrs ibpb stibp xsaveopt md_clear flush_l1d
bugs            : cpu_meltdown spectre_v1 spectre_v2 spec_store_bypass l1tf mds swapgs itlb_multihit mmio_unknown bhi
bogomips        : 4800.03
clflush size    : 64
cache_alignment : 64
address sizes   : 46 bits physical, 48 bits virtual
power management:

processor       : 1
vendor_id       : GenuineIntel
cpu family      : 6
model           : 45
model name      : Intel(R) Xeon(R) CPU E5-2665 0 @ 2.40GHz
stepping        : 7
microcode       : 0x71a
cpu MHz         : 2400.018
cache size      : 20480 KB
physical id     : 1
siblings        : 1
core id         : 0
cpu cores       : 1
apicid          : 2
initial apicid  : 2
fpu             : yes
fpu_exception   : yes
cpuid level     : 13
wp              : yes
flags           : fpu vme de pse tsc msr pae mce cx8 apic sep mtrr pge mca cmov pat pse36 clflush acpi mmx fxsr sse sse2 ss ht syscall nx pdpe1gb rdtscp lm constant_tsc rep_good nopl cpuid tsc_known_freq pni pclmulqdq ssse3 cx16 pcid sse4_1 sse4_2 x2apic popcnt tsc_deadline_timer aes xsave avx hypervisor lahf_lm cpuid_fault pti ssbd ibrs ibpb stibp xsaveopt md_clear flush_l1d
bugs            : cpu_meltdown spectre_v1 spectre_v2 spec_store_bypass l1tf mds swapgs itlb_multihit mmio_unknown bhi
bogomips        : 4800.03
clflush size    : 64
cache_alignment : 64
address sizes   : 46 bits physical, 48 bits virtual
power management:
```
```bash
cat /proc/cpuinfo | grep proc | wc -l
2
```
```bash
iostat -c
Linux 5.14.0-570.25.1.el9_6.x86_64 (rocky2)     08/14/25        _x86_64_        (2 CPU)

avg-cpu:  %user   %nice %system %iowait  %steal   %idle
           1.53    0.01    1.22    0.08    0.23   96.93
```
```bash
iostat -c 2
Linux 5.14.0-570.25.1.el9_6.x86_64 (rocky2)     08/14/25        _x86_64_        (2 CPU)

avg-cpu:  %user   %nice %system %iowait  %steal   %idle
           1.53    0.01    1.22    0.08    0.23   96.93



avg-cpu:  %user   %nice %system %iowait  %steal   %idle
           0.00    0.00    0.25    0.25    0.25   99.25



avg-cpu:  %user   %nice %system %iowait  %steal   %idle
           0.00    0.00    0.50    0.00    0.00   99.50



avg-cpu:  %user   %nice %system %iowait  %steal   %idle
           0.25    0.00    0.50    0.00    0.25   99.00



avg-cpu:  %user   %nice %system %iowait  %steal   %idle
           0.00    0.00    0.00    0.25    0.25   99.50
```
```bash
iostat -c 2 5
Linux 5.14.0-570.25.1.el9_6.x86_64 (rocky2)     08/14/25        _x86_64_        (2 CPU)

avg-cpu:  %user   %nice %system %iowait  %steal   %idle
           1.53    0.01    1.22    0.08    0.23   96.93



avg-cpu:  %user   %nice %system %iowait  %steal   %idle
          16.21    0.00   12.22    0.00    0.50   71.07



avg-cpu:  %user   %nice %system %iowait  %steal   %idle
          12.28    0.00    8.77    0.00    0.75   78.20



avg-cpu:  %user   %nice %system %iowait  %steal   %idle
           0.00    0.00    0.50    0.25    0.25   99.00



avg-cpu:  %user   %nice %system %iowait  %steal   %idle
          15.50    0.00   11.25    0.00    0.50   72.75
```
```bash
uptime
 22:46:48 up 1 day, 19:37,  1 user,  load average: 0.00, 0.00, 0.00
```
```bash
w
 22:50:46 up 1 day, 19:41,  1 user,  load average: 0.12, 0.05, 0.01
USER     TTY        LOGIN@   IDLE   JCPU   PCPU WHAT
root     pts/0     15:57    0.00s  0.52s  0.01s w
```
```bash
who
root     pts/0        2025-08-14 15:57 (192.168.11.246)
```
```bash
whoami
root
```
```bash
ps -aux | grep ^root | wc -l
114
```
```bash
sar | more
Linux 5.14.0-570.25.1.el9_6.x86_64 (rocky2)     08/14/25        _x86_64_        (2 CPU)

00:00:01        CPU     %user     %nice   %system   %iowait    %steal     %idle
00:10:01        all      1.53      0.00      1.23      0.08      0.19     96.97
00:20:01        all      1.49      0.00      1.20      0.08      0.19     97.04
00:30:01        all      1.52      0.00      1.18      0.08      0.18     97.05
00:40:01        all      1.46      0.00      1.17      0.08      0.19     97.10
00:50:01        all      1.51      0.00      1.17      0.08      0.18     97.06
01:00:01        all      1.54      0.00      1.21      0.08      0.19     96.98
01:10:01        all      1.55      0.00      1.23      0.08      0.19     96.96
01:20:01        all      1.48      0.04      1.19      0.08      0.19     97.03
01:30:01        all      1.48      0.00      1.18      0.08      0.19     97.07
01:40:01        all      1.44      0.00      1.16      0.07      0.18     97.15
01:50:01        all      1.47      0.00      1.18      0.08      0.19     97.08
02:00:01        all      1.44      0.00      1.16      0.07      0.19     97.14
02:10:01        all      1.48      0.00      1.17      0.07      0.18     97.11
02:20:01        all      1.46      0.00      1.14      0.07      0.17     97.16
```
```bash
sar -r | more
Linux 5.14.0-570.25.1.el9_6.x86_64 (rocky2)     08/14/25        _x86_64_        (2 CPU)

00:00:01    kbmemfree   kbavail kbmemused  %memused kbbuffers  kbcached  kbcommit   %commit  kbactive   kbinact   kbdirty
00:10:01      6136704   6021956    151792      1.87         0   1709320   1994656     24.61   1757192         0         0
00:20:01      6137800   6023044    150580      1.86         0   1709340   1995164     24.62   1757300         0         0
00:30:01      6136412   6021656    151864      1.87         0   1709364   1995188     24.62   1757224         0         0
00:40:01      6150300   6035544    138216      1.71         0   1709388   1995212     24.62   1757308         0         0
00:50:01      6137360   6022604    151096      1.86         0   1709408   1995236     24.62   1757368         0         0
01:00:01      6136976   6022224    151400      1.87         0   1709428   1994760     24.62   1757188         0         0
01:10:01      6139188   6024432    149096      1.84         0   1709452   1995608     24.63   1757328         0         0
01:20:01      6138916   6024160    149268      1.84         0   1709476   1995300     24.62   1757352         0         0
01:30:01      6140028   6025272    148056      1.83         0   1709492   1994828     24.62   1757368         0         0
01:40:01      6143924   6029168    144424      1.78         0   1709516   1995836     24.63   1757556         0         0
01:50:01      6135400   6020644    152904      1.89         0   1709540   1995748     24.63   1757468         0         0
02:00:01      6141652   6026896    146520      1.81         0   1709560   1995384     24.62   1757436         0         0
02:10:01      6138964   6024208    149132      1.84         0   1709580   1994916     24.62   1757364         0         0
```
```bash
sar 2
Linux 5.14.0-570.25.1.el9_6.x86_64 (rocky2)     08/14/25        _x86_64_        (2 CPU)

22:57:07        CPU     %user     %nice   %system   %iowait    %steal     %idle
22:57:09        all      0.00      0.00      0.00      0.25      0.25     99.50
22:57:11        all      0.25      0.00      0.25      0.00      0.25     99.25
22:57:13        all      0.00      0.00      0.00      0.00      0.00    100.00
^C
Average:        all      0.08      0.00      0.08      0.08      0.17     99.58
```
```bash
sar 2 5
Linux 5.14.0-570.25.1.el9_6.x86_64 (rocky2)     08/14/25        _x86_64_        (2 CPU)

22:57:42        CPU     %user     %nice   %system   %iowait    %steal     %idle
22:57:44        all      0.00      0.00      0.00      0.25      0.25     99.50
22:57:46        all      0.00      0.00      0.25      0.00      0.00     99.75
22:57:48        all      0.00      0.00      0.25      0.00      0.25     99.50
22:57:50        all      0.00      0.00      0.50      0.25      0.25     99.00
22:57:52        all      0.00      0.00      0.25      0.00      0.00     99.75
Average:        all      0.00      0.00      0.25      0.10      0.15     99.50
```
```bash
sar -r 2
Linux 5.14.0-570.25.1.el9_6.x86_64 (rocky2)     08/14/25        _x86_64_        (2 CPU)

22:58:44    kbmemfree   kbavail kbmemused  %memused kbbuffers  kbcached  kbcommit   %commit  kbactive   kbinact   kbdirty
22:58:46      5492496   5390348    168976      2.09         0   2263448   2558520     31.57   2318708         8         0
22:58:48      5492496   5390348    168976      2.09         0   2263448   2558520     31.57   2318772         8         0
22:58:50      5492496   5390348    168976      2.09         0   2263448   2558520     31.57   2318772         8         0
^C
Average:      5492496   5390348    168976      2.09         0   2263448   2558520     31.57   2318751         8         0
```
```bash
sar -r 2 5
Linux 5.14.0-570.25.1.el9_6.x86_64 (rocky2)     08/14/25        _x86_64_        (2 CPU)

22:59:13    kbmemfree   kbavail kbmemused  %memused kbbuffers  kbcached  kbcommit   %commit  kbactive   kbinact   kbdirty
22:59:15      5492316   5390168    169144      2.09         0   2263452   2558524     31.57   2318708         8         0
22:59:17      5492064   5389916    169412      2.09         0   2263452   2558524     31.57   2318708         8         0
22:59:19      5492064   5389916    169412      2.09         0   2263452   2558524     31.57   2318768         8         0
22:59:21      5492316   5390168    169160      2.09         0   2263452   2558524     31.57   2318768         8         0
22:59:23      5492064   5389916    169412      2.09         0   2263452   2558524     31.57   2318768         8         0
Average:      5492165   5390017    169308      2.09         0   2263452   2558524     31.57   2318744         8         0
```
```bash
for file in `ls /var/log/sa/sa??`; do echo "reading this file $file"; done
```
```bash
for file in `ls /var/log/sa/sa?? | sort -n`; do sar -f $file ; done
```
```bash
for file in `ls /var/log/sa/sa?? | sort -n`; do sar -f $file | tee -a /tmp/sar_data_`hostname`; done
```
```bash
ls -l /tmp/sar_data*
-rw-r--r-- 1 root root 21462 Aug 14 23:05 /tmp/sar_data_rocky2
```
```bash
cat /tmp/sar_data_rocky2 | wc -l
272
```
```bash
ps -ef | grep -i cron
root         849       1  0 Aug13 ?        00:00:00 /usr/sbin/crond -n
root      870812  803369  0 23:08 pts/0    00:00:00 grep --color=auto -i cron
```
```bash
systemctl status crond
● crond.service - Command Scheduler
     Loaded: loaded (/usr/lib/systemd/system/crond.service; enabled; preset: enabled)
     Active: active (running) since Wed 2025-08-13 03:09:54 UTC; 1 day 19h ago
   Main PID: 849 (crond)
      Tasks: 1 (limit: 50204)
     Memory: 972.0K
        CPU: 2.586s
     CGroup: /system.slice/crond.service
             └─849 /usr/sbin/crond -n

Aug 14 21:01:01 rocky2 run-parts[828314]: (/etc/cron.hourly) starting 0anacron
Aug 14 21:01:01 rocky2 run-parts[828320]: (/etc/cron.hourly) finished 0anacron
Aug 14 21:01:01 rocky2 CROND[828310]: (root) CMDEND (run-parts /etc/cron.hourly)
Aug 14 22:01:01 rocky2 CROND[848521]: (root) CMD (run-parts /etc/cron.hourly)
Aug 14 22:01:01 rocky2 run-parts[848524]: (/etc/cron.hourly) starting 0anacron
Aug 14 22:01:01 rocky2 run-parts[848530]: (/etc/cron.hourly) finished 0anacron
Aug 14 22:01:01 rocky2 CROND[848520]: (root) CMDEND (run-parts /etc/cron.hourly)
Aug 14 23:01:01 rocky2 CROND[868354]: (root) CMD (run-parts /etc/cron.hourly)
Aug 14 23:01:01 rocky2 run-parts[868357]: (/etc/cron.hourly) starting 0anacron
Aug 14 23:01:01 rocky2 run-parts[868363]: (/etc/cron.hourly) finished 0anacron
```
```bash
ls -ld /etc/cron*
drwxr-xr-x 2 root root  60 Aug 13 03:09 /etc/cron.d
drwxr-xr-x 2 root root  40 May 11  2022 /etc/cron.daily
-rw-r--r-- 1 root root   0 Aug  5 18:08 /etc/cron.deny
drwxr-xr-x 2 root root  60 Aug 13 03:09 /etc/cron.hourly
drwxr-xr-x 2 root root  40 May 11  2022 /etc/cron.monthly
drwxr-xr-x 2 root root  40 May 11  2022 /etc/cron.weekly
-rw-r--r-- 1 root root 451 May 11  2022 /etc/crontab
```
```bash
crontab -e
no crontab for root - using an empty one
crontab: installing new crontab

Broadcast message from root@rocky2 (somewhere) (Thu Aug 14 23:11:02 2025):

this is my cronjob running at Thu Aug 14 23:11:02 UTC 2025
```


