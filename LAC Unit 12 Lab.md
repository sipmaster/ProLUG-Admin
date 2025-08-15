```bash
dnf install stress
dnf install iperf
```
```bash
systemctl cat sysstat-collect.timer
# /usr/lib/systemd/system/sysstat-collect.timer
# /usr/lib/systemd/system/sysstat-collect.timer
# (C) 2014 Tomasz Torcz <tomek@pipebreaker.pl>
#
# sysstat-12.5.4 systemd unit file:
#        Activates activity collector every 10 minutes

[Unit]
Description=Run system activity accounting tool every 10 minutes

[Timer]
OnCalendar=*:00/10

[Install]
WantedBy=sysstat.service
```
```bash
sar 2 10
Linux 5.14.0-570.25.1.el9_6.x86_64 (rocky2)     08/15/25        _x86_64_        (2 CPU)

15:43:22        CPU     %user     %nice   %system   %iowait    %steal     %idle
15:43:24        all      4.33      0.00      4.58      0.00      0.51     90.59
15:43:26        all      4.55      0.00      4.80      0.25      0.76     89.65
15:43:28        all      4.57      0.00      4.06      0.00      0.76     90.61
15:43:30        all      5.34      0.00      5.09      0.00      0.51     89.06
15:43:32        all      3.54      0.00      3.04      0.00      0.76     92.66
15:43:34        all      3.30      0.00      3.55      0.25      0.76     92.13
15:43:36        all      3.80      0.00      4.05      0.00      0.76     91.39
15:43:38        all      5.58      0.00      3.81      0.00      0.51     90.10
15:43:40        all      5.08      0.00      5.84      0.00      1.02     88.07
15:43:42        all      4.06      0.00      4.06      0.25      0.76     90.86
Average:        all      4.41      0.00      4.29      0.08      0.71     90.51
```
```bash
sar -r 2 10
Linux 5.14.0-570.25.1.el9_6.x86_64 (rocky2)     08/15/25        _x86_64_        (2 CPU)

15:43:58    kbmemfree   kbavail kbmemused  %memused kbbuffers  kbcached  kbcommit   %commit  kbactive   kbinact   kbdirty
15:44:00      3059272   2967060    965188     11.91         0   3814440   5685096     70.15   4636324       180         0
15:44:02      3059524   2967312    964940     11.91         0   3814440   5685096     70.15   4635188       180         0
15:44:04      3059524   2967312    964944     11.91         0   3814440   5685096     70.15   4634480       180         0
15:44:06      3061540   2969328    962924     11.88         0   3814440   5685096     70.15   4634928       180         0
15:44:08      3061540   2969328    962924     11.88         0   3814440   5685096     70.15   4638292       180         0
15:44:10      3061540   2969328    962920     11.88         0   3814440   5685096     70.15   4640020       180         0
15:44:12      3061540   2969328    962920     11.88         0   3814440   5685096     70.15   4634372       180         0
15:44:14      3061540   2969328    962920     11.88         0   3814440   5685096     70.15   4634440       180         0
15:44:16      3061540   2969328    962920     11.88         0   3814440   5685096     70.15   4634440       180         0
15:44:18      3061540   2969328    962924     11.88         0   3814440   5685096     70.15   4634692       180         0
Average:      3060910   2968698    963552     11.89         0   3814440   5685096     70.15   4635718       180         0
```
```bash
iostat
Linux 5.14.0-570.25.1.el9_6.x86_64 (rocky2)     08/15/25        _x86_64_        (2 CPU)

avg-cpu:  %user   %nice %system %iowait  %steal   %idle
           2.66    0.01    2.26    0.07    0.34   94.65

Device             tps    kB_read/s    kB_wrtn/s    kB_dscd/s    kB_read    kB_wrtn    kB_dscd
xvda              0.00         0.01         0.00         0.00       2828          0          0
xvdb              0.84        20.94        15.05         0.00    4568636    3283253          0
xvdc              0.84        35.38         0.78         0.00    7719198     169167          0
xvde              0.83        35.29         0.55         0.00    7699763     119527          0
```
```bash
iostat -c
Linux 5.14.0-570.25.1.el9_6.x86_64 (rocky2)     08/15/25        _x86_64_        (2 CPU)

avg-cpu:  %user   %nice %system %iowait  %steal   %idle
           2.66    0.01    2.26    0.07    0.34   94.65
```
```bash
iostat -d
Linux 5.14.0-570.25.1.el9_6.x86_64 (rocky2)     08/15/25        _x86_64_        (2 CPU)

Device             tps    kB_read/s    kB_wrtn/s    kB_dscd/s    kB_read    kB_wrtn    kB_dscd
xvda              0.00         0.01         0.00         0.00       2828          0          0
xvdb              0.84        20.93        15.04         0.00    4569020    3283253          0
xvdc              0.84        35.37         0.78         0.00    7719582     169167          0
xvde              0.83        35.28         0.55         0.00    7700147     119527          0
```
```bash
iostat -c 1 5
Linux 5.14.0-570.25.1.el9_6.x86_64 (rocky2)     08/15/25        _x86_64_        (2 CPU)

avg-cpu:  %user   %nice %system %iowait  %steal   %idle
           2.66    0.01    2.26    0.07    0.34   94.65



avg-cpu:  %user   %nice %system %iowait  %steal   %idle
           6.63    0.00    9.18    0.00    0.51   83.67



avg-cpu:  %user   %nice %system %iowait  %steal   %idle
           5.03    0.00    4.52    0.00    1.01   89.45



avg-cpu:  %user   %nice %system %iowait  %steal   %idle
           4.59    0.00    3.57    0.00    0.51   91.33



avg-cpu:  %user   %nice %system %iowait  %steal   %idle
           3.54    0.00    4.55    0.51    1.01   90.40
```
```bash
time iperf3 -c 192.168.200.101 -n 1G -P 128
Connecting to host 192.168.200.101, port 5201
[  5] local 192.168.200.52 port 39674 connected to 192.168.200.101 port 5201
[  7] local 192.168.200.52 port 39678 connected to 192.168.200.101 port 5201
[  9] local 192.168.200.52 port 39682 connected to 192.168.200.101 port 5201
[ 11] local 192.168.200.52 port 39694 connected to 192.168.200.101 port 5201
[ 13] local 192.168.200.52 port 39710 connected to 192.168.200.101 port 5201
[ 15] local 192.168.200.52 port 39714 connected to 192.168.200.101 port 5201
[ 17] local 192.168.200.52 port 39726 connected to 192.168.200.101 port 5201
[ 19] local 192.168.200.52 port 39730 connected to 192.168.200.101 port 5201
[ 21] local 192.168.200.52 port 39740 connected to 192.168.200.101 port 5201
[ 23] local 192.168.200.52 port 39752 connected to 192.168.200.101 port 5201
[ 25] local 192.168.200.52 port 39756 connected to 192.168.200.101 port 5201
[ 27] local 192.168.200.52 port 39768 connected to 192.168.200.101 port 5201
[ 29] local 192.168.200.52 port 39770 connected to 192.168.200.101 port 5201
[ 31] local 192.168.200.52 port 39772 connected to 192.168.200.101 port 5201
[ 33] local 192.168.200.52 port 39786 connected to 192.168.200.101 port 5201
[ 35] local 192.168.200.52 port 39802 connected to 192.168.200.101 port 5201
[ 37] local 192.168.200.52 port 39808 connected to 192.168.200.101 port 5201
[ 39] local 192.168.200.52 port 39814 connected to 192.168.200.101 port 5201
[ 41] local 192.168.200.52 port 39820 connected to 192.168.200.101 port 5201
[ 43] local 192.168.200.52 port 39830 connected to 192.168.200.101 port 5201
[ 45] local 192.168.200.52 port 39838 connected to 192.168.200.101 port 5201
[ 47] local 192.168.200.52 port 39850 connected to 192.168.200.101 port 5201
[ 49] local 192.168.200.52 port 39858 connected to 192.168.200.101 port 5201
[ 51] local 192.168.200.52 port 39864 connected to 192.168.200.101 port 5201
[ 53] local 192.168.200.52 port 39878 connected to 192.168.200.101 port 5201
[ 55] local 192.168.200.52 port 39894 connected to 192.168.200.101 port 5201
[ 57] local 192.168.200.52 port 39904 connected to 192.168.200.101 port 5201
[ 59] local 192.168.200.52 port 39916 connected to 192.168.200.101 port 5201
[ 61] local 192.168.200.52 port 39922 connected to 192.168.200.101 port 5201
[ 63] local 192.168.200.52 port 39934 connected to 192.168.200.101 port 5201
[ 65] local 192.168.200.52 port 39946 connected to 192.168.200.101 port 5201
[ 67] local 192.168.200.52 port 39952 connected to 192.168.200.101 port 5201
[ 69] local 192.168.200.52 port 39954 connected to 192.168.200.101 port 5201
[ 71] local 192.168.200.52 port 39956 connected to 192.168.200.101 port 5201
[ 73] local 192.168.200.52 port 39958 connected to 192.168.200.101 port 5201
[ 75] local 192.168.200.52 port 39962 connected to 192.168.200.101 port 5201
[ 77] local 192.168.200.52 port 39978 connected to 192.168.200.101 port 5201
[ 79] local 192.168.200.52 port 39990 connected to 192.168.200.101 port 5201
[ 81] local 192.168.200.52 port 40000 connected to 192.168.200.101 port 5201
[ 83] local 192.168.200.52 port 40004 connected to 192.168.200.101 port 5201
[ 85] local 192.168.200.52 port 40006 connected to 192.168.200.101 port 5201
[ 87] local 192.168.200.52 port 40014 connected to 192.168.200.101 port 5201
[ 89] local 192.168.200.52 port 40022 connected to 192.168.200.101 port 5201
[ 91] local 192.168.200.52 port 40026 connected to 192.168.200.101 port 5201
[ 93] local 192.168.200.52 port 40028 connected to 192.168.200.101 port 5201
[ 95] local 192.168.200.52 port 40044 connected to 192.168.200.101 port 5201
[ 97] local 192.168.200.52 port 40058 connected to 192.168.200.101 port 5201
[ 99] local 192.168.200.52 port 40064 connected to 192.168.200.101 port 5201
[101] local 192.168.200.52 port 40068 connected to 192.168.200.101 port 5201
[103] local 192.168.200.52 port 40078 connected to 192.168.200.101 port 5201
[105] local 192.168.200.52 port 40088 connected to 192.168.200.101 port 5201
[107] local 192.168.200.52 port 40094 connected to 192.168.200.101 port 5201
[109] local 192.168.200.52 port 40102 connected to 192.168.200.101 port 5201
[111] local 192.168.200.52 port 40110 connected to 192.168.200.101 port 5201
[113] local 192.168.200.52 port 40116 connected to 192.168.200.101 port 5201
[115] local 192.168.200.52 port 40128 connected to 192.168.200.101 port 5201
[117] local 192.168.200.52 port 40138 connected to 192.168.200.101 port 5201
[119] local 192.168.200.52 port 40152 connected to 192.168.200.101 port 5201
[121] local 192.168.200.52 port 40154 connected to 192.168.200.101 port 5201
[123] local 192.168.200.52 port 40166 connected to 192.168.200.101 port 5201
[125] local 192.168.200.52 port 40174 connected to 192.168.200.101 port 5201
[127] local 192.168.200.52 port 40184 connected to 192.168.200.101 port 5201
[129] local 192.168.200.52 port 40196 connected to 192.168.200.101 port 5201
[131] local 192.168.200.52 port 40208 connected to 192.168.200.101 port 5201
[133] local 192.168.200.52 port 40212 connected to 192.168.200.101 port 5201
[135] local 192.168.200.52 port 40222 connected to 192.168.200.101 port 5201
[137] local 192.168.200.52 port 40232 connected to 192.168.200.101 port 5201
[139] local 192.168.200.52 port 40248 connected to 192.168.200.101 port 5201
[141] local 192.168.200.52 port 40260 connected to 192.168.200.101 port 5201
[143] local 192.168.200.52 port 40264 connected to 192.168.200.101 port 5201
[145] local 192.168.200.52 port 40280 connected to 192.168.200.101 port 5201
[147] local 192.168.200.52 port 40284 connected to 192.168.200.101 port 5201
[149] local 192.168.200.52 port 40292 connected to 192.168.200.101 port 5201
[151] local 192.168.200.52 port 40302 connected to 192.168.200.101 port 5201
[153] local 192.168.200.52 port 40316 connected to 192.168.200.101 port 5201
[155] local 192.168.200.52 port 40330 connected to 192.168.200.101 port 5201
[157] local 192.168.200.52 port 40338 connected to 192.168.200.101 port 5201
[159] local 192.168.200.52 port 40342 connected to 192.168.200.101 port 5201
[161] local 192.168.200.52 port 40358 connected to 192.168.200.101 port 5201
[163] local 192.168.200.52 port 40362 connected to 192.168.200.101 port 5201
[165] local 192.168.200.52 port 40374 connected to 192.168.200.101 port 5201
[167] local 192.168.200.52 port 40376 connected to 192.168.200.101 port 5201
[169] local 192.168.200.52 port 40390 connected to 192.168.200.101 port 5201
[171] local 192.168.200.52 port 40406 connected to 192.168.200.101 port 5201
[173] local 192.168.200.52 port 40414 connected to 192.168.200.101 port 5201
[175] local 192.168.200.52 port 40424 connected to 192.168.200.101 port 5201
[177] local 192.168.200.52 port 40432 connected to 192.168.200.101 port 5201
[179] local 192.168.200.52 port 40446 connected to 192.168.200.101 port 5201
[181] local 192.168.200.52 port 40462 connected to 192.168.200.101 port 5201
[183] local 192.168.200.52 port 40470 connected to 192.168.200.101 port 5201
[185] local 192.168.200.52 port 40476 connected to 192.168.200.101 port 5201
[187] local 192.168.200.52 port 40486 connected to 192.168.200.101 port 5201
[189] local 192.168.200.52 port 40488 connected to 192.168.200.101 port 5201
[191] local 192.168.200.52 port 40494 connected to 192.168.200.101 port 5201
[193] local 192.168.200.52 port 40500 connected to 192.168.200.101 port 5201
[195] local 192.168.200.52 port 40510 connected to 192.168.200.101 port 5201
[197] local 192.168.200.52 port 40524 connected to 192.168.200.101 port 5201
[199] local 192.168.200.52 port 40538 connected to 192.168.200.101 port 5201
[201] local 192.168.200.52 port 40552 connected to 192.168.200.101 port 5201
[203] local 192.168.200.52 port 40566 connected to 192.168.200.101 port 5201
[205] local 192.168.200.52 port 40568 connected to 192.168.200.101 port 5201
[207] local 192.168.200.52 port 40574 connected to 192.168.200.101 port 5201
[209] local 192.168.200.52 port 40576 connected to 192.168.200.101 port 5201
[211] local 192.168.200.52 port 40590 connected to 192.168.200.101 port 5201
[213] local 192.168.200.52 port 40596 connected to 192.168.200.101 port 5201
[215] local 192.168.200.52 port 40600 connected to 192.168.200.101 port 5201
[217] local 192.168.200.52 port 40604 connected to 192.168.200.101 port 5201
[219] local 192.168.200.52 port 40612 connected to 192.168.200.101 port 5201
[221] local 192.168.200.52 port 40620 connected to 192.168.200.101 port 5201
[223] local 192.168.200.52 port 40634 connected to 192.168.200.101 port 5201
[225] local 192.168.200.52 port 40640 connected to 192.168.200.101 port 5201
[227] local 192.168.200.52 port 40654 connected to 192.168.200.101 port 5201
[229] local 192.168.200.52 port 40670 connected to 192.168.200.101 port 5201
[231] local 192.168.200.52 port 40684 connected to 192.168.200.101 port 5201
[233] local 192.168.200.52 port 40698 connected to 192.168.200.101 port 5201
[235] local 192.168.200.52 port 40702 connected to 192.168.200.101 port 5201
[237] local 192.168.200.52 port 40704 connected to 192.168.200.101 port 5201
[239] local 192.168.200.52 port 40716 connected to 192.168.200.101 port 5201
[241] local 192.168.200.52 port 40718 connected to 192.168.200.101 port 5201
[243] local 192.168.200.52 port 40722 connected to 192.168.200.101 port 5201
[245] local 192.168.200.52 port 40726 connected to 192.168.200.101 port 5201
[247] local 192.168.200.52 port 40734 connected to 192.168.200.101 port 5201
[249] local 192.168.200.52 port 40750 connected to 192.168.200.101 port 5201
[251] local 192.168.200.52 port 40758 connected to 192.168.200.101 port 5201
[253] local 192.168.200.52 port 40764 connected to 192.168.200.101 port 5201
[255] local 192.168.200.52 port 40778 connected to 192.168.200.101 port 5201
[257] local 192.168.200.52 port 40780 connected to 192.168.200.101 port 5201
[259] local 192.168.200.52 port 40794 connected to 192.168.200.101 port 5201
[ ID] Interval           Transfer     Bitrate         Retr  Cwnd
[  5]   0.00-1.03   sec  6.23 MBytes  50.5 Mbits/sec   65    164 KBytes
[  7]   0.00-1.03   sec  4.98 MBytes  40.4 Mbits/sec   78    137 KBytes
[  9]   0.00-1.03   sec  5.42 MBytes  43.9 Mbits/sec    1    208 KBytes
[ 11]   0.00-1.03   sec  3.73 MBytes  30.2 Mbits/sec   45   65.0 KBytes
[ 13]   0.00-1.03   sec  4.98 MBytes  40.4 Mbits/sec    0    321 KBytes
[ 15]   0.00-1.03   sec  6.16 MBytes  49.9 Mbits/sec   46    185 KBytes
[ 17]   0.00-1.03   sec  5.92 MBytes  48.0 Mbits/sec    1    339 KBytes
[ 19]   0.00-1.03   sec  4.98 MBytes  40.4 Mbits/sec    0    313 KBytes
[ 21]   0.00-1.03   sec  4.98 MBytes  40.4 Mbits/sec    2    291 KBytes
[ 23]   0.00-1.03   sec  4.98 MBytes  40.4 Mbits/sec   29    110 KBytes
[ 25]   0.00-1.03   sec  6.23 MBytes  50.5 Mbits/sec  124    156 KBytes
[ 27]   0.00-1.03   sec  6.23 MBytes  50.5 Mbits/sec   10    240 KBytes
[ 29]   0.00-1.04   sec  4.98 MBytes  40.4 Mbits/sec    0    315 KBytes
[ 31]   0.00-1.04   sec  4.98 MBytes  40.4 Mbits/sec    3    294 KBytes
[ 33]   0.00-1.04   sec  3.87 MBytes  31.4 Mbits/sec    1   1.41 KBytes
[ 35]   0.00-1.04   sec  4.98 MBytes  40.4 Mbits/sec    3    294 KBytes
[ 37]   0.00-1.04   sec  4.98 MBytes  40.4 Mbits/sec    2    267 KBytes
[ 39]   0.00-1.04   sec  5.00 MBytes  40.5 Mbits/sec   13    184 KBytes
[ 41]   0.00-1.04   sec  4.98 MBytes  40.4 Mbits/sec    2    294 KBytes
[ 43]   0.00-1.04   sec  4.98 MBytes  40.4 Mbits/sec    2    164 KBytes
[ 45]   0.00-1.04   sec  5.00 MBytes  40.5 Mbits/sec    3    297 KBytes
[ 47]   0.00-1.04   sec  5.85 MBytes  47.4 Mbits/sec    5    219 KBytes
[ 49]   0.00-1.04   sec  5.66 MBytes  45.9 Mbits/sec   65    148 KBytes
[ 51]   0.00-1.04   sec  5.99 MBytes  48.5 Mbits/sec   45    229 KBytes
[ 53]   0.00-1.04   sec  6.17 MBytes  50.0 Mbits/sec   61    102 KBytes
[ 55]   0.00-1.04   sec  5.00 MBytes  40.5 Mbits/sec    1    325 KBytes
[ 57]   0.00-1.04   sec  4.98 MBytes  40.4 Mbits/sec    0    339 KBytes
[ 59]   0.00-1.04   sec  6.19 MBytes  50.1 Mbits/sec   20    209 KBytes
[ 61]   0.00-1.04   sec  6.25 MBytes  50.6 Mbits/sec   48    198 KBytes
[ 63]   0.00-1.04   sec  5.79 MBytes  46.9 Mbits/sec    3    260 KBytes
[ 65]   0.00-1.04   sec  5.79 MBytes  46.9 Mbits/sec    5    219 KBytes
[ 67]   0.00-1.04   sec  5.79 MBytes  46.9 Mbits/sec    3    314 KBytes
[ 69]   0.00-1.04   sec  5.79 MBytes  46.9 Mbits/sec    6    206 KBytes
[ 71]   0.00-1.04   sec  5.20 MBytes  42.1 Mbits/sec   48    113 KBytes
[ 73]   0.00-1.04   sec  4.98 MBytes  40.3 Mbits/sec   39    182 KBytes
[ 75]   0.00-1.04   sec  4.78 MBytes  38.7 Mbits/sec   45    188 KBytes
[ 77]   0.00-1.04   sec  4.54 MBytes  36.8 Mbits/sec    2    294 KBytes
[ 79]   0.00-1.04   sec  5.92 MBytes  47.9 Mbits/sec    3    260 KBytes
[ 81]   0.00-1.04   sec  5.00 MBytes  40.5 Mbits/sec   45    208 KBytes
[ 83]   0.00-1.04   sec  4.98 MBytes  40.3 Mbits/sec   21    238 KBytes
[ 85]   0.00-1.04   sec  5.92 MBytes  47.9 Mbits/sec    3    314 KBytes
[ 87]   0.00-1.04   sec  4.42 MBytes  35.8 Mbits/sec    2    294 KBytes
[ 89]   0.00-1.04   sec  4.98 MBytes  40.3 Mbits/sec    0    324 KBytes
[ 91]   0.00-1.04   sec  4.98 MBytes  40.3 Mbits/sec    0    339 KBytes
[ 93]   0.00-1.04   sec  5.00 MBytes  40.5 Mbits/sec    1    313 KBytes
[ 95]   0.00-1.04   sec  6.23 MBytes  50.5 Mbits/sec    2    356 KBytes
[ 97]   0.00-1.04   sec  4.98 MBytes  40.3 Mbits/sec    1    339 KBytes
[ 99]   0.00-1.04   sec  6.23 MBytes  50.5 Mbits/sec   93    233 KBytes
[101]   0.00-1.04   sec  6.23 MBytes  50.5 Mbits/sec   66    136 KBytes
[103]   0.00-1.04   sec  6.23 MBytes  50.5 Mbits/sec   46    235 KBytes
[105]   0.00-1.04   sec  5.87 MBytes  47.6 Mbits/sec    3    310 KBytes
[107]   0.00-1.04   sec  6.25 MBytes  50.6 Mbits/sec    3    204 KBytes
[109]   0.00-1.04   sec  4.48 MBytes  36.3 Mbits/sec   66   93.3 KBytes
[111]   0.00-1.04   sec  4.50 MBytes  36.5 Mbits/sec    1    276 KBytes
[113]   0.00-1.04   sec  4.98 MBytes  40.3 Mbits/sec    4    206 KBytes
[115]   0.00-1.04   sec  4.98 MBytes  40.3 Mbits/sec    0    286 KBytes
[117]   0.00-1.04   sec  5.00 MBytes  40.5 Mbits/sec   23    102 KBytes
[119]   0.00-1.04   sec  5.92 MBytes  47.9 Mbits/sec    3    314 KBytes
[121]   0.00-1.04   sec  6.25 MBytes  50.6 Mbits/sec    1    407 KBytes
[123]   0.00-1.04   sec  4.98 MBytes  40.3 Mbits/sec    0    349 KBytes
[125]   0.00-1.04   sec  5.87 MBytes  47.6 Mbits/sec    4    315 KBytes
[127]   0.00-1.04   sec  5.79 MBytes  46.9 Mbits/sec    6   2.83 KBytes
[129]   0.00-1.04   sec  5.81 MBytes  47.1 Mbits/sec   48    181 KBytes
[131]   0.00-1.04   sec  6.23 MBytes  50.5 Mbits/sec    1    382 KBytes
[133]   0.00-1.04   sec  5.81 MBytes  47.1 Mbits/sec    4    315 KBytes
[135]   0.00-1.04   sec  4.98 MBytes  40.3 Mbits/sec    2    280 KBytes
[137]   0.00-1.04   sec  4.50 MBytes  36.5 Mbits/sec    2    139 KBytes
[139]   0.00-1.04   sec  5.92 MBytes  47.9 Mbits/sec   49    181 KBytes
[141]   0.00-1.04   sec  4.98 MBytes  40.3 Mbits/sec    3    314 KBytes
[143]   0.00-1.04   sec  5.92 MBytes  47.9 Mbits/sec    4    298 KBytes
[145]   0.00-1.04   sec  5.98 MBytes  48.4 Mbits/sec    4    283 KBytes
[147]   0.00-1.04   sec  4.98 MBytes  40.3 Mbits/sec    2    204 KBytes
[149]   0.00-1.04   sec  5.87 MBytes  47.6 Mbits/sec    3    259 KBytes
[151]   0.00-1.04   sec  4.72 MBytes  38.3 Mbits/sec   45   94.7 KBytes
[153]   0.00-1.04   sec  4.98 MBytes  40.3 Mbits/sec   93    139 KBytes
[155]   0.00-1.04   sec  5.81 MBytes  47.1 Mbits/sec    3    283 KBytes
[157]   0.00-1.04   sec  5.00 MBytes  40.5 Mbits/sec   48    132 KBytes
[159]   0.00-1.04   sec  4.48 MBytes  36.3 Mbits/sec    2    197 KBytes
[161]   0.00-1.04   sec  5.79 MBytes  46.9 Mbits/sec    3    280 KBytes
[163]   0.00-1.04   sec  5.00 MBytes  40.5 Mbits/sec   48    180 KBytes
[165]   0.00-1.04   sec  4.98 MBytes  40.3 Mbits/sec    1    223 KBytes
[167]   0.00-1.04   sec  5.00 MBytes  40.5 Mbits/sec    0    345 KBytes
[169]   0.00-1.04   sec  5.81 MBytes  47.1 Mbits/sec    3    245 KBytes
[171]   0.00-1.04   sec  4.98 MBytes  40.3 Mbits/sec    2    260 KBytes
[173]   0.00-1.04   sec  5.79 MBytes  46.9 Mbits/sec    5   2.83 KBytes
[175]   0.00-1.04   sec  5.00 MBytes  40.5 Mbits/sec    2    141 KBytes
[177]   0.00-1.04   sec  5.79 MBytes  46.9 Mbits/sec    3    222 KBytes
[179]   0.00-1.04   sec  4.98 MBytes  40.3 Mbits/sec   47    161 KBytes
[181]   0.00-1.04   sec  3.73 MBytes  30.2 Mbits/sec    3   2.83 KBytes
[183]   0.00-1.04   sec  4.50 MBytes  36.4 Mbits/sec    2    197 KBytes
[185]   0.00-1.04   sec  4.98 MBytes  40.3 Mbits/sec    2    280 KBytes
[187]   0.00-1.04   sec  6.23 MBytes  50.5 Mbits/sec    2    212 KBytes
[189]   0.00-1.04   sec  5.00 MBytes  40.5 Mbits/sec   48    187 KBytes
[191]   0.00-1.04   sec  5.00 MBytes  40.5 Mbits/sec   48    171 KBytes
[193]   0.00-1.04   sec  4.98 MBytes  40.3 Mbits/sec   47    195 KBytes
[195]   0.00-1.04   sec  4.98 MBytes  40.3 Mbits/sec    2    313 KBytes
[197]   0.00-1.04   sec  6.23 MBytes  50.5 Mbits/sec    1    339 KBytes
[199]   0.00-1.04   sec  4.98 MBytes  40.3 Mbits/sec    1    202 KBytes
[201]   0.00-1.04   sec  5.00 MBytes  40.5 Mbits/sec   47    198 KBytes
[203]   0.00-1.04   sec  4.54 MBytes  36.8 Mbits/sec    2    181 KBytes
[205]   0.00-1.04   sec  5.00 MBytes  40.5 Mbits/sec    2    260 KBytes
[207]   0.00-1.04   sec  4.98 MBytes  40.3 Mbits/sec    2    294 KBytes
[209]   0.00-1.04   sec  6.17 MBytes  50.0 Mbits/sec    1    337 KBytes
[211]   0.00-1.04   sec  4.98 MBytes  40.3 Mbits/sec    2    260 KBytes
[213]   0.00-1.04   sec  4.98 MBytes  40.3 Mbits/sec    2    279 KBytes
[215]   0.00-1.04   sec  6.17 MBytes  49.9 Mbits/sec    1    315 KBytes
[217]   0.00-1.04   sec  6.17 MBytes  50.0 Mbits/sec    1    315 KBytes
[219]   0.00-1.04   sec  4.98 MBytes  40.3 Mbits/sec    2    260 KBytes
[221]   0.00-1.04   sec  4.98 MBytes  40.3 Mbits/sec    1    338 KBytes
[223]   0.00-1.04   sec  6.17 MBytes  50.0 Mbits/sec    1    293 KBytes
[225]   0.00-1.04   sec  4.86 MBytes  39.4 Mbits/sec    0    173 KBytes
[227]   0.00-1.04   sec  4.86 MBytes  39.4 Mbits/sec    0    171 KBytes
[229]   0.00-1.04   sec  4.98 MBytes  40.3 Mbits/sec   48    103 KBytes
[231]   0.00-1.04   sec  4.71 MBytes  38.2 Mbits/sec    1   96.2 KBytes
[233]   0.00-1.04   sec  4.86 MBytes  39.3 Mbits/sec   29    100 KBytes
[235]   0.00-1.04   sec  4.86 MBytes  39.3 Mbits/sec   15   99.0 KBytes
[237]   0.00-1.04   sec  5.87 MBytes  47.6 Mbits/sec    1    167 KBytes
[239]   0.00-1.04   sec  4.60 MBytes  37.2 Mbits/sec   46   97.6 KBytes
[241]   0.00-1.04   sec  6.23 MBytes  50.5 Mbits/sec   45    226 KBytes
[243]   0.00-1.04   sec  4.86 MBytes  39.3 Mbits/sec    0    175 KBytes
[245]   0.00-1.04   sec  4.92 MBytes  39.8 Mbits/sec   92    103 KBytes
[247]   0.00-1.04   sec  4.92 MBytes  39.9 Mbits/sec    0    171 KBytes
[249]   0.00-1.04   sec  5.36 MBytes  43.4 Mbits/sec  115    100 KBytes
[251]   0.00-1.04   sec  4.98 MBytes  40.3 Mbits/sec   93    153 KBytes
[253]   0.00-1.04   sec  4.85 MBytes  39.3 Mbits/sec    0    293 KBytes
[255]   0.00-1.04   sec  5.89 MBytes  47.7 Mbits/sec    1    171 KBytes
[257]   0.00-1.04   sec  4.98 MBytes  40.3 Mbits/sec    0    342 KBytes
[259]   0.00-1.04   sec  3.50 MBytes  28.3 Mbits/sec    1    209 KBytes
[SUM]   0.00-1.03   sec   677 MBytes  5.49 Gbits/sec  2357
- - - - - - - - - - - - - - - - - - - - - - - - -
[  5]   1.03-2.12   sec  3.16 MBytes  24.5 Mbits/sec  1148    123 KBytes
[  7]   1.03-2.12   sec  2.75 MBytes  21.3 Mbits/sec  430    147 KBytes
[  9]   1.03-2.12   sec  2.43 MBytes  18.9 Mbits/sec  155    273 KBytes
[ 11]   1.03-2.12   sec  4.11 MBytes  31.9 Mbits/sec  222    182 KBytes
[ 13]   1.03-2.12   sec  3.54 MBytes  27.5 Mbits/sec  463    214 KBytes
[ 15]   1.03-2.12   sec  1.62 MBytes  12.6 Mbits/sec  602    139 KBytes
[ 17]   1.03-2.12   sec  2.88 MBytes  22.3 Mbits/sec  1129   99.0 KBytes
[ 19]   1.03-2.12   sec  3.58 MBytes  27.8 Mbits/sec    8    345 KBytes
[ 21]   1.03-2.12   sec  3.87 MBytes  30.0 Mbits/sec  638    173 KBytes
[ 23]   1.03-2.12   sec  2.54 MBytes  19.7 Mbits/sec  332    120 KBytes
[ 25]   1.03-2.12   sec  2.43 MBytes  18.9 Mbits/sec   11    158 KBytes
[ 27]   1.03-2.12   sec  2.18 MBytes  16.9 Mbits/sec  950    208 KBytes
[ 29]   1.04-2.12   sec  2.88 MBytes  22.3 Mbits/sec  458   39.6 KBytes
[ 31]   1.04-2.12   sec  3.49 MBytes  27.1 Mbits/sec   13    148 KBytes
[ 33]   1.04-2.12   sec  2.34 MBytes  18.2 Mbits/sec   46    141 KBytes
[ 35]   1.04-2.12   sec  3.49 MBytes  27.1 Mbits/sec   12    146 KBytes
[ 37]   1.04-2.12   sec  3.68 MBytes  28.6 Mbits/sec  1209    119 KBytes
[ 39]   1.04-2.12   sec  3.17 MBytes  24.6 Mbits/sec  139    158 KBytes
[ 41]   1.04-2.12   sec  3.87 MBytes  30.0 Mbits/sec  1297    113 KBytes
[ 43]   1.04-2.12   sec  3.24 MBytes  25.2 Mbits/sec  749    132 KBytes
[ 45]   1.04-2.12   sec  3.50 MBytes  27.1 Mbits/sec   11    150 KBytes
[ 47]   1.04-2.12   sec  2.50 MBytes  19.4 Mbits/sec   61   72.1 KBytes
[ 49]   1.04-2.12   sec  1.97 MBytes  15.3 Mbits/sec  613    157 KBytes
[ 51]   1.04-2.12   sec  1.67 MBytes  13.0 Mbits/sec  164   5.66 KBytes
[ 53]   1.04-2.12   sec  1.39 MBytes  10.8 Mbits/sec  325    201 KBytes
[ 55]   1.04-2.12   sec  3.43 MBytes  26.6 Mbits/sec  1082   79.2 KBytes
[ 57]   1.04-2.12   sec  3.55 MBytes  27.6 Mbits/sec  1244    163 KBytes
[ 59]   1.04-2.12   sec  1.49 MBytes  11.6 Mbits/sec    8    214 KBytes
[ 61]   1.04-2.12   sec  1.62 MBytes  12.6 Mbits/sec  491    132 KBytes
[ 63]   1.04-2.12   sec  2.87 MBytes  22.2 Mbits/sec  984    139 KBytes
[ 65]   1.04-2.12   sec  2.88 MBytes  22.3 Mbits/sec   41   9.90 KBytes
[ 67]   1.04-2.12   sec  2.88 MBytes  22.3 Mbits/sec  1148   91.9 KBytes
[ 69]   1.04-2.12   sec  2.88 MBytes  22.3 Mbits/sec   11    211 KBytes
[ 71]   1.04-2.12   sec  2.03 MBytes  15.8 Mbits/sec   49   67.9 KBytes
[ 73]   1.04-2.12   sec  3.46 MBytes  26.9 Mbits/sec  992    160 KBytes
[ 75]   1.04-2.12   sec  2.74 MBytes  21.2 Mbits/sec  296    124 KBytes
[ 77]   1.04-2.12   sec  4.12 MBytes  32.0 Mbits/sec  1077    105 KBytes
[ 79]   1.04-2.12   sec  2.75 MBytes  21.3 Mbits/sec  1079    119 KBytes
[ 81]   1.04-2.12   sec  3.87 MBytes  30.0 Mbits/sec  649    174 KBytes
[ 83]   1.04-2.12   sec  3.36 MBytes  26.1 Mbits/sec    9    249 KBytes
[ 85]   1.04-2.12   sec  2.75 MBytes  21.3 Mbits/sec  580   50.9 KBytes
[ 87]   1.04-2.12   sec  4.75 MBytes  36.9 Mbits/sec   11    375 KBytes
[ 89]   1.04-2.12   sec  3.47 MBytes  26.9 Mbits/sec  1158    181 KBytes
[ 91]   1.04-2.12   sec  3.49 MBytes  27.1 Mbits/sec  1262    137 KBytes
[ 93]   1.04-2.12   sec  3.43 MBytes  26.6 Mbits/sec  1165    116 KBytes
[ 95]   1.04-2.12   sec  2.38 MBytes  18.5 Mbits/sec  142   18.4 KBytes
[ 97]   1.04-2.12   sec  4.16 MBytes  32.3 Mbits/sec    9    379 KBytes
[ 99]   1.04-2.12   sec  2.50 MBytes  19.4 Mbits/sec  170   24.0 KBytes
[101]   1.04-2.12   sec  1.16 MBytes  9.04 Mbits/sec   60    150 KBytes
[103]   1.04-2.12   sec  2.36 MBytes  18.3 Mbits/sec  398    110 KBytes
[105]   1.04-2.12   sec  2.75 MBytes  21.3 Mbits/sec  1058   86.3 KBytes
[107]   1.04-2.12   sec  1.50 MBytes  11.6 Mbits/sec  359    126 KBytes
[109]   1.04-2.12   sec  2.05 MBytes  15.9 Mbits/sec    0    110 KBytes
[111]   1.04-2.12   sec  3.94 MBytes  30.5 Mbits/sec  646    181 KBytes
[113]   1.04-2.12   sec  3.20 MBytes  24.9 Mbits/sec   12    148 KBytes
[115]   1.04-2.12   sec  3.08 MBytes  23.9 Mbits/sec  250   8.48 KBytes
[117]   1.04-2.12   sec  1.65 MBytes  12.8 Mbits/sec    0    116 KBytes
[119]   1.04-2.12   sec  2.75 MBytes  21.3 Mbits/sec  226    288 KBytes
[121]   1.04-2.12   sec  2.50 MBytes  19.4 Mbits/sec  147   18.4 KBytes
[123]   1.04-2.12   sec  3.62 MBytes  28.1 Mbits/sec  1305    124 KBytes
[125]   1.04-2.12   sec  2.75 MBytes  21.3 Mbits/sec  164   77.8 KBytes
[127]   1.04-2.12   sec  2.92 MBytes  22.6 Mbits/sec   51    272 KBytes
[129]   1.04-2.12   sec  2.74 MBytes  21.3 Mbits/sec  1326    393 KBytes
[131]   1.04-2.12   sec  2.50 MBytes  19.4 Mbits/sec  161   18.4 KBytes
[133]   1.04-2.12   sec  2.75 MBytes  21.3 Mbits/sec   93    123 KBytes
[135]   1.04-2.12   sec  3.68 MBytes  28.5 Mbits/sec  1042   4.24 KBytes
[137]   1.04-2.12   sec  3.32 MBytes  25.7 Mbits/sec  104    130 KBytes
[139]   1.04-2.12   sec  2.37 MBytes  18.4 Mbits/sec  906    130 KBytes
[141]   1.04-2.12   sec  2.75 MBytes  21.3 Mbits/sec   11    223 KBytes
[143]   1.04-2.12   sec  2.50 MBytes  19.4 Mbits/sec  909    235 KBytes
[145]   1.04-2.12   sec  2.43 MBytes  18.8 Mbits/sec  913    137 KBytes
[147]   1.04-2.12   sec  2.59 MBytes  20.1 Mbits/sec  571    100 KBytes
[149]   1.04-2.12   sec  2.69 MBytes  20.9 Mbits/sec  862   94.7 KBytes
[151]   1.04-2.12   sec  1.62 MBytes  12.5 Mbits/sec    1    107 KBytes
[153]   1.04-2.12   sec  3.19 MBytes  24.8 Mbits/sec  159    100 KBytes
[155]   1.04-2.12   sec  2.75 MBytes  21.3 Mbits/sec  1424   91.9 KBytes
[157]   1.04-2.12   sec  3.18 MBytes  24.7 Mbits/sec  913    100 KBytes
[159]   1.04-2.12   sec  3.90 MBytes  30.2 Mbits/sec  332   9.90 KBytes
[161]   1.04-2.12   sec  2.75 MBytes  21.3 Mbits/sec  1431   90.5 KBytes
[163]   1.04-2.12   sec  3.55 MBytes  27.6 Mbits/sec  1038    148 KBytes
[165]   1.04-2.12   sec  2.75 MBytes  21.3 Mbits/sec  130   15.6 KBytes
[167]   1.04-2.12   sec  3.41 MBytes  26.5 Mbits/sec  1340    174 KBytes
[169]   1.04-2.12   sec  2.54 MBytes  19.7 Mbits/sec  113    124 KBytes
[171]   1.04-2.12   sec  3.55 MBytes  27.6 Mbits/sec  1082   2.83 KBytes
[173]   1.04-2.12   sec  2.11 MBytes  16.3 Mbits/sec  100    250 KBytes
[175]   1.04-2.12   sec  2.75 MBytes  21.3 Mbits/sec  324   74.9 KBytes
[177]   1.04-2.12   sec  2.48 MBytes  19.3 Mbits/sec    9    113 KBytes
[179]   1.04-2.12   sec  2.75 MBytes  21.3 Mbits/sec  568   93.3 KBytes
[181]   1.04-2.12   sec  2.99 MBytes  23.2 Mbits/sec   47    165 KBytes
[183]   1.04-2.12   sec  3.19 MBytes  24.7 Mbits/sec   14    141 KBytes
[185]   1.04-2.12   sec  3.68 MBytes  28.5 Mbits/sec  1353   2.83 KBytes
[187]   1.04-2.12   sec  2.11 MBytes  16.4 Mbits/sec  1064    143 KBytes
[189]   1.04-2.12   sec  3.55 MBytes  27.6 Mbits/sec  1026    148 KBytes
[191]   1.04-2.12   sec  3.34 MBytes  25.9 Mbits/sec   99   52.3 KBytes
[193]   1.04-2.12   sec  3.68 MBytes  28.5 Mbits/sec  1756    115 KBytes
[195]   1.04-2.12   sec  3.86 MBytes  30.0 Mbits/sec  1039    154 KBytes
[197]   1.04-2.12   sec  2.30 MBytes  17.8 Mbits/sec  118   15.6 KBytes
[199]   1.04-2.12   sec  2.42 MBytes  18.7 Mbits/sec  583    177 KBytes
[201]   1.04-2.12   sec  3.68 MBytes  28.5 Mbits/sec  1658    124 KBytes
[203]   1.04-2.12   sec  3.56 MBytes  27.6 Mbits/sec  828    158 KBytes
[205]   1.04-2.12   sec  3.55 MBytes  27.6 Mbits/sec  1009    148 KBytes
[207]   1.04-2.12   sec  3.74 MBytes  29.0 Mbits/sec  1058    153 KBytes
[209]   1.04-2.12   sec  2.30 MBytes  17.8 Mbits/sec  710   43.8 KBytes
[211]   1.04-2.12   sec  3.55 MBytes  27.6 Mbits/sec  1058    148 KBytes
[213]   1.04-2.12   sec  3.35 MBytes  26.0 Mbits/sec  221    242 KBytes
[215]   1.04-2.12   sec  2.29 MBytes  17.8 Mbits/sec  585    124 KBytes
[217]   1.04-2.12   sec  2.04 MBytes  15.9 Mbits/sec  1063    105 KBytes
[219]   1.04-2.12   sec  3.55 MBytes  27.6 Mbits/sec  1058    148 KBytes
[221]   1.04-2.12   sec  3.48 MBytes  27.0 Mbits/sec   10    378 KBytes
[223]   1.04-2.12   sec  2.09 MBytes  16.2 Mbits/sec  691   7.07 KBytes
[225]   1.04-2.12   sec  2.79 MBytes  21.6 Mbits/sec  303    189 KBytes
[227]   1.04-2.12   sec  2.78 MBytes  21.6 Mbits/sec  133    124 KBytes
[229]   1.04-2.12   sec  1.96 MBytes  15.2 Mbits/sec  222   94.7 KBytes
[231]   1.04-2.12   sec  1.48 MBytes  11.5 Mbits/sec    0    105 KBytes
[233]   1.04-2.12   sec  1.71 MBytes  13.3 Mbits/sec   19   79.2 KBytes
[235]   1.04-2.12   sec  1.71 MBytes  13.3 Mbits/sec    0    105 KBytes
[237]   1.04-2.12   sec  1.50 MBytes  11.6 Mbits/sec  613    136 KBytes
[239]   1.04-2.12   sec  1.49 MBytes  11.6 Mbits/sec    0    103 KBytes
[241]   1.04-2.12   sec  1.50 MBytes  11.6 Mbits/sec  563    163 KBytes
[243]   1.04-2.12   sec  2.90 MBytes  22.5 Mbits/sec  621    170 KBytes
[245]   1.04-2.12   sec  2.41 MBytes  18.7 Mbits/sec  259    132 KBytes
[247]   1.04-2.12   sec  2.78 MBytes  21.6 Mbits/sec  525   12.7 KBytes
[249]   1.04-2.12   sec  1.67 MBytes  13.0 Mbits/sec   68   50.9 KBytes
[251]   1.04-2.12   sec  3.18 MBytes  24.7 Mbits/sec  958    107 KBytes
[253]   1.04-2.12   sec  3.41 MBytes  26.5 Mbits/sec  1205   76.4 KBytes
[255]   1.04-2.12   sec  1.50 MBytes  11.6 Mbits/sec  629   96.2 KBytes
[257]   1.04-2.12   sec  2.40 MBytes  18.6 Mbits/sec  713    117 KBytes
[259]   1.04-2.12   sec  3.04 MBytes  23.6 Mbits/sec  228    119 KBytes
[SUM]   1.03-2.12   sec   361 MBytes  2.81 Gbits/sec  69487
- - - - - - - - - - - - - - - - - - - - - - - - -
[ ID] Interval           Transfer     Bitrate         Retr
[  5]   0.00-2.14   sec  9.39 MBytes  36.8 Mbits/sec  1213             sender
[  5]   0.00-2.33   sec  6.48 MBytes  23.4 Mbits/sec                  receiver
[  7]   0.00-2.14   sec  7.72 MBytes  30.2 Mbits/sec  508             sender
[  7]   0.00-2.33   sec  6.48 MBytes  23.4 Mbits/sec                  receiver
[  9]   0.00-2.14   sec  7.85 MBytes  30.7 Mbits/sec  156             sender
[  9]   0.00-2.33   sec  6.60 MBytes  23.8 Mbits/sec                  receiver
[ 11]   0.00-2.14   sec  7.84 MBytes  30.7 Mbits/sec  267             sender
[ 11]   0.00-2.33   sec  5.85 MBytes  21.1 Mbits/sec                  receiver
[ 13]   0.00-2.14   sec  8.52 MBytes  33.3 Mbits/sec  463             sender
[ 13]   0.00-2.33   sec  6.48 MBytes  23.4 Mbits/sec                  receiver
[ 15]   0.00-2.14   sec  7.78 MBytes  30.5 Mbits/sec  648             sender
[ 15]   0.00-2.33   sec  6.60 MBytes  23.8 Mbits/sec                  receiver
[ 17]   0.00-2.14   sec  8.79 MBytes  34.4 Mbits/sec  1131             sender
[ 17]   0.00-2.33   sec  6.60 MBytes  23.8 Mbits/sec                  receiver
[ 19]   0.00-2.14   sec  8.56 MBytes  33.5 Mbits/sec    8             sender
[ 19]   0.00-2.33   sec  6.48 MBytes  23.4 Mbits/sec                  receiver
[ 21]   0.00-2.14   sec  8.84 MBytes  34.6 Mbits/sec  669             sender
[ 21]   0.00-2.33   sec  6.48 MBytes  23.4 Mbits/sec                  receiver
[ 23]   0.00-2.14   sec  7.52 MBytes  29.4 Mbits/sec  361             sender
[ 23]   0.00-2.33   sec  6.48 MBytes  23.4 Mbits/sec                  receiver
[ 25]   0.00-2.14   sec  8.66 MBytes  33.9 Mbits/sec  135             sender
[ 25]   0.00-2.33   sec  6.60 MBytes  23.8 Mbits/sec                  receiver
[ 27]   0.00-2.14   sec  8.41 MBytes  32.9 Mbits/sec  960             sender
[ 27]   0.00-2.33   sec  6.60 MBytes  23.8 Mbits/sec                  receiver
[ 29]   0.00-2.14   sec  7.85 MBytes  30.8 Mbits/sec  489             sender
[ 29]   0.00-2.33   sec  6.48 MBytes  23.4 Mbits/sec                  receiver
[ 31]   0.00-2.14   sec  8.47 MBytes  33.2 Mbits/sec   16             sender
[ 31]   0.00-2.33   sec  6.48 MBytes  23.4 Mbits/sec                  receiver
[ 33]   0.00-2.14   sec  6.22 MBytes  24.3 Mbits/sec   47             sender
[ 33]   0.00-2.33   sec  5.94 MBytes  21.4 Mbits/sec                  receiver
[ 35]   0.00-2.14   sec  8.47 MBytes  33.2 Mbits/sec   15             sender
[ 35]   0.00-2.33   sec  6.48 MBytes  23.4 Mbits/sec                  receiver
[ 37]   0.00-2.14   sec  8.66 MBytes  33.9 Mbits/sec  1211             sender
[ 37]   0.00-2.33   sec  6.48 MBytes  23.4 Mbits/sec                  receiver
[ 39]   0.00-2.14   sec  8.17 MBytes  32.0 Mbits/sec  152             sender
[ 39]   0.00-2.33   sec  6.50 MBytes  23.4 Mbits/sec                  receiver
[ 41]   0.00-2.14   sec  8.84 MBytes  34.6 Mbits/sec  1299             sender
[ 41]   0.00-2.33   sec  6.48 MBytes  23.4 Mbits/sec                  receiver
[ 43]   0.00-2.14   sec  8.22 MBytes  32.2 Mbits/sec  751             sender
[ 43]   0.00-2.33   sec  6.48 MBytes  23.4 Mbits/sec                  receiver
[ 45]   0.00-2.14   sec  8.50 MBytes  33.3 Mbits/sec   14             sender
[ 45]   0.00-2.33   sec  6.50 MBytes  23.4 Mbits/sec                  receiver
[ 47]   0.00-2.14   sec  8.35 MBytes  32.7 Mbits/sec   66             sender
[ 47]   0.00-2.33   sec  6.60 MBytes  23.8 Mbits/sec                  receiver
[ 49]   0.00-2.14   sec  7.64 MBytes  29.9 Mbits/sec  678             sender
[ 49]   0.00-2.33   sec  6.48 MBytes  23.4 Mbits/sec                  receiver
[ 51]   0.00-2.14   sec  7.66 MBytes  30.0 Mbits/sec  209             sender
[ 51]   0.00-2.33   sec  6.50 MBytes  23.4 Mbits/sec                  receiver
[ 53]   0.00-2.14   sec  7.56 MBytes  29.6 Mbits/sec  386             sender
[ 53]   0.00-2.33   sec  6.48 MBytes  23.4 Mbits/sec                  receiver
[ 55]   0.00-2.14   sec  8.43 MBytes  33.0 Mbits/sec  1083             sender
[ 55]   0.00-2.33   sec  6.50 MBytes  23.4 Mbits/sec                  receiver
[ 57]   0.00-2.14   sec  8.53 MBytes  33.4 Mbits/sec  1244             sender
[ 57]   0.00-2.33   sec  6.48 MBytes  23.4 Mbits/sec                  receiver
[ 59]   0.00-2.14   sec  7.68 MBytes  30.1 Mbits/sec   28             sender
[ 59]   0.00-2.33   sec  6.38 MBytes  23.0 Mbits/sec                  receiver
[ 61]   0.00-2.14   sec  7.87 MBytes  30.8 Mbits/sec  539             sender
[ 61]   0.00-2.33   sec  6.50 MBytes  23.4 Mbits/sec                  receiver
[ 63]   0.00-2.14   sec  8.66 MBytes  33.9 Mbits/sec  1127             sender
[ 63]   0.00-2.33   sec  6.48 MBytes  23.4 Mbits/sec                  receiver
[ 65]   0.00-2.14   sec  8.67 MBytes  33.9 Mbits/sec   46             sender
[ 65]   0.00-2.33   sec  6.48 MBytes  23.4 Mbits/sec                  receiver
[ 67]   0.00-2.14   sec  8.67 MBytes  33.9 Mbits/sec  1151             sender
[ 67]   0.00-2.33   sec  6.48 MBytes  23.4 Mbits/sec                  receiver
[ 69]   0.00-2.14   sec  8.67 MBytes  33.9 Mbits/sec   17             sender
[ 69]   0.00-2.33   sec  6.48 MBytes  23.4 Mbits/sec                  receiver
[ 71]   0.00-2.14   sec  7.23 MBytes  28.3 Mbits/sec   97             sender
[ 71]   0.00-2.33   sec  6.48 MBytes  23.4 Mbits/sec                  receiver
[ 73]   0.00-2.14   sec  8.44 MBytes  33.0 Mbits/sec  1285             sender
[ 73]   0.00-2.33   sec  6.48 MBytes  23.4 Mbits/sec                  receiver
[ 75]   0.00-2.14   sec  7.51 MBytes  29.4 Mbits/sec  341             sender
[ 75]   0.00-2.33   sec  6.35 MBytes  22.9 Mbits/sec                  receiver
[ 77]   0.00-2.14   sec  8.67 MBytes  33.9 Mbits/sec  1142             sender
[ 77]   0.00-2.33   sec  6.48 MBytes  23.4 Mbits/sec                  receiver
[ 79]   0.00-2.14   sec  8.66 MBytes  33.9 Mbits/sec  1249             sender
[ 79]   0.00-2.33   sec  6.48 MBytes  23.4 Mbits/sec                  receiver
[ 81]   0.00-2.14   sec  8.86 MBytes  34.7 Mbits/sec  723             sender
[ 81]   0.00-2.33   sec  6.50 MBytes  23.4 Mbits/sec                  receiver
[ 83]   0.00-2.14   sec  8.34 MBytes  32.6 Mbits/sec   30             sender
[ 83]   0.00-2.33   sec  6.48 MBytes  23.4 Mbits/sec                  receiver
[ 85]   0.00-2.14   sec  8.67 MBytes  33.9 Mbits/sec  583             sender
[ 85]   0.00-2.33   sec  6.48 MBytes  23.4 Mbits/sec                  receiver
[ 87]   0.00-2.14   sec  9.17 MBytes  35.9 Mbits/sec   13             sender
[ 87]   0.00-2.33   sec  6.48 MBytes  23.4 Mbits/sec                  receiver
[ 89]   0.00-2.14   sec  8.45 MBytes  33.1 Mbits/sec  1158             sender
[ 89]   0.00-2.33   sec  6.48 MBytes  23.4 Mbits/sec                  receiver
[ 91]   0.00-2.14   sec  8.47 MBytes  33.2 Mbits/sec  1262             sender
[ 91]   0.00-2.33   sec  6.48 MBytes  23.4 Mbits/sec                  receiver
[ 93]   0.00-2.14   sec  8.43 MBytes  33.0 Mbits/sec  1166             sender
[ 93]   0.00-2.33   sec  6.50 MBytes  23.4 Mbits/sec                  receiver
[ 95]   0.00-2.14   sec  8.61 MBytes  33.7 Mbits/sec  157             sender
[ 95]   0.00-2.33   sec  6.48 MBytes  23.4 Mbits/sec                  receiver
[ 97]   0.00-2.14   sec  9.14 MBytes  35.8 Mbits/sec   11             sender
[ 97]   0.00-2.33   sec  6.48 MBytes  23.4 Mbits/sec                  receiver
[ 99]   0.00-2.14   sec  8.73 MBytes  34.2 Mbits/sec  263             sender
[ 99]   0.00-2.33   sec  6.48 MBytes  23.4 Mbits/sec                  receiver
[101]   0.00-2.14   sec  7.39 MBytes  28.9 Mbits/sec  126             sender
[101]   0.00-2.33   sec  6.48 MBytes  23.4 Mbits/sec                  receiver
[103]   0.00-2.14   sec  8.59 MBytes  33.6 Mbits/sec  444             sender
[103]   0.00-2.33   sec  6.48 MBytes  23.4 Mbits/sec                  receiver
[105]   0.00-2.14   sec  8.62 MBytes  33.8 Mbits/sec  1061             sender
[105]   0.00-2.33   sec  6.50 MBytes  23.4 Mbits/sec                  receiver
[107]   0.00-2.14   sec  7.75 MBytes  30.3 Mbits/sec  362             sender
[107]   0.00-2.33   sec  6.50 MBytes  23.4 Mbits/sec                  receiver
[109]   0.00-2.14   sec  6.53 MBytes  25.6 Mbits/sec   66             sender
[109]   0.00-2.33   sec  6.35 MBytes  22.9 Mbits/sec                  receiver
[111]   0.00-2.14   sec  8.43 MBytes  33.0 Mbits/sec  647             sender
[111]   0.00-2.33   sec  6.50 MBytes  23.4 Mbits/sec                  receiver
[113]   0.00-2.14   sec  8.18 MBytes  32.0 Mbits/sec   16             sender
[113]   0.00-2.33   sec  6.48 MBytes  23.4 Mbits/sec                  receiver
[115]   0.00-2.14   sec  8.06 MBytes  31.5 Mbits/sec  250             sender
[115]   0.00-2.33   sec  6.48 MBytes  23.4 Mbits/sec                  receiver
[117]   0.00-2.14   sec  6.65 MBytes  26.0 Mbits/sec   23             sender
[117]   0.00-2.33   sec  6.03 MBytes  21.8 Mbits/sec                  receiver
[119]   0.00-2.14   sec  8.67 MBytes  33.9 Mbits/sec  229             sender
[119]   0.00-2.33   sec  6.48 MBytes  23.4 Mbits/sec                  receiver
[121]   0.00-2.14   sec  8.75 MBytes  34.3 Mbits/sec  161             sender
[121]   0.00-2.33   sec  6.50 MBytes  23.4 Mbits/sec                  receiver
[123]   0.00-2.14   sec  8.59 MBytes  33.7 Mbits/sec  1305             sender
[123]   0.00-2.33   sec  6.48 MBytes  23.4 Mbits/sec                  receiver
[125]   0.00-2.14   sec  8.62 MBytes  33.8 Mbits/sec  168             sender
[125]   0.00-2.33   sec  6.50 MBytes  23.4 Mbits/sec                  receiver
[127]   0.00-2.14   sec  8.71 MBytes  34.1 Mbits/sec   57             sender
[127]   0.00-2.33   sec  6.48 MBytes  23.4 Mbits/sec                  receiver
[129]   0.00-2.14   sec  8.55 MBytes  33.5 Mbits/sec  1374             sender
[129]   0.00-2.33   sec  6.50 MBytes  23.4 Mbits/sec                  receiver
[131]   0.00-2.14   sec  8.73 MBytes  34.2 Mbits/sec  176             sender
[131]   0.00-2.33   sec  6.48 MBytes  23.4 Mbits/sec                  receiver
[133]   0.00-2.14   sec  8.56 MBytes  33.5 Mbits/sec   97             sender
[133]   0.00-2.33   sec  6.50 MBytes  23.4 Mbits/sec                  receiver
[135]   0.00-2.14   sec  8.66 MBytes  33.9 Mbits/sec  1266             sender
[135]   0.00-2.33   sec  6.48 MBytes  23.4 Mbits/sec                  receiver
[137]   0.00-2.14   sec  7.82 MBytes  30.6 Mbits/sec  106             sender
[137]   0.00-2.33   sec  6.50 MBytes  23.4 Mbits/sec                  receiver
[139]   0.00-2.14   sec  8.28 MBytes  32.4 Mbits/sec  955             sender
[139]   0.00-2.33   sec  6.48 MBytes  23.4 Mbits/sec                  receiver
[141]   0.00-2.14   sec  7.73 MBytes  30.3 Mbits/sec   14             sender
[141]   0.00-2.33   sec  6.48 MBytes  23.4 Mbits/sec                  receiver
[143]   0.00-2.14   sec  8.42 MBytes  33.0 Mbits/sec  913             sender
[143]   0.00-2.33   sec  6.48 MBytes  23.4 Mbits/sec                  receiver
[145]   0.00-2.14   sec  8.41 MBytes  32.9 Mbits/sec  917             sender
[145]   0.00-2.33   sec  6.48 MBytes  23.4 Mbits/sec                  receiver
[147]   0.00-2.14   sec  7.57 MBytes  29.6 Mbits/sec  573             sender
[147]   0.00-2.33   sec  6.48 MBytes  23.4 Mbits/sec                  receiver
[149]   0.00-2.14   sec  8.56 MBytes  33.5 Mbits/sec  865             sender
[149]   0.00-2.33   sec  6.50 MBytes  23.4 Mbits/sec                  receiver
[151]   0.00-2.14   sec  6.34 MBytes  24.8 Mbits/sec   46             sender
[151]   0.00-2.33   sec  6.21 MBytes  22.4 Mbits/sec                  receiver
[153]   0.00-2.14   sec  8.17 MBytes  32.0 Mbits/sec  252             sender
[153]   0.00-2.33   sec  6.48 MBytes  23.4 Mbits/sec                  receiver
[155]   0.00-2.14   sec  8.56 MBytes  33.5 Mbits/sec  1427             sender
[155]   0.00-2.33   sec  6.50 MBytes  23.4 Mbits/sec                  receiver
[157]   0.00-2.14   sec  8.18 MBytes  32.0 Mbits/sec  961             sender
[157]   0.00-2.33   sec  6.50 MBytes  23.4 Mbits/sec                  receiver
[159]   0.00-2.14   sec  8.37 MBytes  32.8 Mbits/sec  342             sender
[159]   0.00-2.33   sec  6.48 MBytes  23.4 Mbits/sec                  receiver
[161]   0.00-2.14   sec  8.54 MBytes  33.4 Mbits/sec  1434             sender
[161]   0.00-2.33   sec  6.48 MBytes  23.4 Mbits/sec                  receiver
[163]   0.00-2.14   sec  8.55 MBytes  33.5 Mbits/sec  1086             sender
[163]   0.00-2.33   sec  6.50 MBytes  23.4 Mbits/sec                  receiver
[165]   0.00-2.14   sec  7.73 MBytes  30.3 Mbits/sec  131             sender
[165]   0.00-2.33   sec  6.48 MBytes  23.4 Mbits/sec                  receiver
[167]   0.00-2.14   sec  8.41 MBytes  32.9 Mbits/sec  1340             sender
[167]   0.00-2.33   sec  6.38 MBytes  23.0 Mbits/sec                  receiver
[169]   0.00-2.14   sec  8.35 MBytes  32.7 Mbits/sec  116             sender
[169]   0.00-2.33   sec  6.50 MBytes  23.4 Mbits/sec                  receiver
[171]   0.00-2.14   sec  8.53 MBytes  33.4 Mbits/sec  1085             sender
[171]   0.00-2.33   sec  6.48 MBytes  23.4 Mbits/sec                  receiver
[173]   0.00-2.14   sec  7.90 MBytes  30.9 Mbits/sec  105             sender
[173]   0.00-2.33   sec  6.48 MBytes  23.4 Mbits/sec                  receiver
[175]   0.00-2.14   sec  7.75 MBytes  30.3 Mbits/sec  327             sender
[175]   0.00-2.33   sec  6.50 MBytes  23.4 Mbits/sec                  receiver
[177]   0.00-2.14   sec  8.28 MBytes  32.4 Mbits/sec   12             sender
[177]   0.00-2.33   sec  6.48 MBytes  23.4 Mbits/sec                  receiver
[179]   0.00-2.14   sec  7.73 MBytes  30.3 Mbits/sec  615             sender
[179]   0.00-2.33   sec  6.35 MBytes  22.9 Mbits/sec                  receiver
[181]   0.00-2.14   sec  6.72 MBytes  26.3 Mbits/sec   50             sender
[181]   0.00-2.33   sec  5.79 MBytes  20.9 Mbits/sec                  receiver
[183]   0.00-2.14   sec  7.68 MBytes  30.1 Mbits/sec   16             sender
[183]   0.00-2.33   sec  6.50 MBytes  23.4 Mbits/sec                  receiver
[185]   0.00-2.14   sec  8.66 MBytes  33.9 Mbits/sec  1355             sender
[185]   0.00-2.33   sec  6.48 MBytes  23.4 Mbits/sec                  receiver
[187]   0.00-2.14   sec  8.34 MBytes  32.7 Mbits/sec  1066             sender
[187]   0.00-2.33   sec  6.48 MBytes  23.4 Mbits/sec                  receiver
[189]   0.00-2.14   sec  8.55 MBytes  33.5 Mbits/sec  1074             sender
[189]   0.00-2.33   sec  6.50 MBytes  23.4 Mbits/sec                  receiver
[191]   0.00-2.14   sec  8.34 MBytes  32.7 Mbits/sec  147             sender
[191]   0.00-2.33   sec  6.50 MBytes  23.4 Mbits/sec                  receiver
[193]   0.00-2.14   sec  8.66 MBytes  33.9 Mbits/sec  1803             sender
[193]   0.00-2.33   sec  6.48 MBytes  23.4 Mbits/sec                  receiver
[195]   0.00-2.14   sec  8.84 MBytes  34.6 Mbits/sec  1265             sender
[195]   0.00-2.33   sec  6.48 MBytes  23.4 Mbits/sec                  receiver
[197]   0.00-2.14   sec  8.53 MBytes  33.4 Mbits/sec  131             sender
[197]   0.00-2.33   sec  6.48 MBytes  23.4 Mbits/sec                  receiver
[199]   0.00-2.14   sec  7.40 MBytes  29.0 Mbits/sec  584             sender
[199]   0.00-2.33   sec  6.48 MBytes  23.4 Mbits/sec                  receiver
[201]   0.00-2.14   sec  8.68 MBytes  34.0 Mbits/sec  1705             sender
[201]   0.00-2.33   sec  6.50 MBytes  23.4 Mbits/sec                  receiver
[203]   0.00-2.14   sec  8.10 MBytes  31.7 Mbits/sec  830             sender
[203]   0.00-2.33   sec  6.50 MBytes  23.4 Mbits/sec                  receiver
[205]   0.00-2.14   sec  8.55 MBytes  33.5 Mbits/sec  1011             sender
[205]   0.00-2.33   sec  6.50 MBytes  23.4 Mbits/sec                  receiver
[207]   0.00-2.14   sec  8.72 MBytes  34.1 Mbits/sec  1296             sender
[207]   0.00-2.33   sec  6.48 MBytes  23.4 Mbits/sec                  receiver
[209]   0.00-2.14   sec  8.46 MBytes  33.1 Mbits/sec  711             sender
[209]   0.00-2.33   sec  6.48 MBytes  23.4 Mbits/sec                  receiver
[211]   0.00-2.14   sec  8.53 MBytes  33.4 Mbits/sec  1060             sender
[211]   0.00-2.33   sec  6.48 MBytes  23.4 Mbits/sec                  receiver
[213]   0.00-2.14   sec  8.33 MBytes  32.6 Mbits/sec  223             sender
[213]   0.00-2.33   sec  6.48 MBytes  23.4 Mbits/sec                  receiver
[215]   0.00-2.14   sec  8.46 MBytes  33.1 Mbits/sec  586             sender
[215]   0.00-2.33   sec  6.48 MBytes  23.4 Mbits/sec                  receiver
[217]   0.00-2.14   sec  8.21 MBytes  32.2 Mbits/sec  1064             sender
[217]   0.00-2.33   sec  6.48 MBytes  23.4 Mbits/sec                  receiver
[219]   0.00-2.14   sec  8.53 MBytes  33.4 Mbits/sec  1060             sender
[219]   0.00-2.33   sec  6.48 MBytes  23.4 Mbits/sec                  receiver
[221]   0.00-2.14   sec  8.46 MBytes  33.1 Mbits/sec   11             sender
[221]   0.00-2.33   sec  6.42 MBytes  23.1 Mbits/sec                  receiver
[223]   0.00-2.14   sec  8.26 MBytes  32.3 Mbits/sec  698             sender
[223]   0.00-2.33   sec  6.48 MBytes  23.4 Mbits/sec                  receiver
[225]   0.00-2.14   sec  7.65 MBytes  29.9 Mbits/sec  303             sender
[225]   0.00-2.33   sec  6.42 MBytes  23.1 Mbits/sec                  receiver
[227]   0.00-2.14   sec  7.64 MBytes  29.9 Mbits/sec  133             sender
[227]   0.00-2.33   sec  6.35 MBytes  22.9 Mbits/sec                  receiver
[229]   0.00-2.14   sec  6.94 MBytes  27.2 Mbits/sec  270             sender
[229]   0.00-2.33   sec  6.35 MBytes  22.9 Mbits/sec                  receiver
[231]   0.00-2.14   sec  6.19 MBytes  24.2 Mbits/sec    1             sender
[231]   0.00-2.33   sec  6.06 MBytes  21.8 Mbits/sec                  receiver
[233]   0.00-2.14   sec  6.57 MBytes  25.7 Mbits/sec   48             sender
[233]   0.00-2.33   sec  6.35 MBytes  22.9 Mbits/sec                  receiver
[235]   0.00-2.14   sec  6.57 MBytes  25.7 Mbits/sec   15             sender
[235]   0.00-2.33   sec  6.35 MBytes  22.9 Mbits/sec                  receiver
[237]   0.00-2.14   sec  7.37 MBytes  28.9 Mbits/sec  614             sender
[237]   0.00-2.33   sec  6.50 MBytes  23.4 Mbits/sec                  receiver
[239]   0.00-2.14   sec  6.09 MBytes  23.8 Mbits/sec   47             sender
[239]   0.00-2.33   sec  5.96 MBytes  21.5 Mbits/sec                  receiver
[241]   0.00-2.14   sec  7.73 MBytes  30.3 Mbits/sec  608             sender
[241]   0.00-2.33   sec  6.35 MBytes  22.9 Mbits/sec                  receiver
[243]   0.00-2.14   sec  7.75 MBytes  30.4 Mbits/sec  621             sender
[243]   0.00-2.33   sec  6.35 MBytes  22.9 Mbits/sec                  receiver
[245]   0.00-2.14   sec  7.32 MBytes  28.7 Mbits/sec  351             sender
[245]   0.00-2.33   sec  6.35 MBytes  22.9 Mbits/sec                  receiver
[247]   0.00-2.14   sec  7.71 MBytes  30.2 Mbits/sec  525             sender
[247]   0.00-2.33   sec  6.35 MBytes  22.9 Mbits/sec                  receiver
[249]   0.00-2.14   sec  7.03 MBytes  27.5 Mbits/sec  183             sender
[249]   0.00-2.33   sec  6.23 MBytes  22.5 Mbits/sec                  receiver
[251]   0.00-2.14   sec  8.16 MBytes  32.0 Mbits/sec  1051             sender
[251]   0.00-2.33   sec  6.35 MBytes  22.9 Mbits/sec                  receiver
[253]   0.00-2.14   sec  8.27 MBytes  32.4 Mbits/sec  1205             sender
[253]   0.00-2.33   sec  6.35 MBytes  22.9 Mbits/sec                  receiver
[255]   0.00-2.14   sec  7.39 MBytes  28.9 Mbits/sec  630             sender
[255]   0.00-2.33   sec  6.50 MBytes  23.4 Mbits/sec                  receiver
[257]   0.00-2.14   sec  7.38 MBytes  28.9 Mbits/sec  713             sender
[257]   0.00-2.33   sec  5.35 MBytes  19.3 Mbits/sec                  receiver
[259]   0.00-2.14   sec  6.54 MBytes  25.6 Mbits/sec  229             sender
[259]   0.00-2.33   sec  5.10 MBytes  18.4 Mbits/sec                  receiver
[SUM]   0.00-2.14   sec  1.01 GBytes  4.07 Gbits/sec  73310             sender
[SUM]   0.00-2.33   sec   823 MBytes  2.97 Gbits/sec                  receiver

iperf Done.

real    0m3.055s
user    0m0.055s
sys     0m1.447s```
```bash
time iperf3 -c 192.168.200.101 -u -n 1G -P 128
Connecting to host 192.168.200.101, port 5201
[  5] local 192.168.200.52 port 59916 connected to 192.168.200.101 port 5201
[  7] local 192.168.200.52 port 42723 connected to 192.168.200.101 port 5201
[  9] local 192.168.200.52 port 54891 connected to 192.168.200.101 port 5201
[ 11] local 192.168.200.52 port 50951 connected to 192.168.200.101 port 5201
[ 13] local 192.168.200.52 port 54551 connected to 192.168.200.101 port 5201
[ 15] local 192.168.200.52 port 45919 connected to 192.168.200.101 port 5201
[ 17] local 192.168.200.52 port 45980 connected to 192.168.200.101 port 5201
[ 19] local 192.168.200.52 port 54354 connected to 192.168.200.101 port 5201
[ 21] local 192.168.200.52 port 55053 connected to 192.168.200.101 port 5201
[ 23] local 192.168.200.52 port 58476 connected to 192.168.200.101 port 5201
[ 25] local 192.168.200.52 port 33221 connected to 192.168.200.101 port 5201
[ 27] local 192.168.200.52 port 60642 connected to 192.168.200.101 port 5201
[ 29] local 192.168.200.52 port 56050 connected to 192.168.200.101 port 5201
[ 31] local 192.168.200.52 port 57742 connected to 192.168.200.101 port 5201
[ 33] local 192.168.200.52 port 32871 connected to 192.168.200.101 port 5201
[ 35] local 192.168.200.52 port 35888 connected to 192.168.200.101 port 5201
[ 37] local 192.168.200.52 port 47750 connected to 192.168.200.101 port 5201
[ 39] local 192.168.200.52 port 58543 connected to 192.168.200.101 port 5201
[ 41] local 192.168.200.52 port 36344 connected to 192.168.200.101 port 5201
[ 43] local 192.168.200.52 port 48085 connected to 192.168.200.101 port 5201
[ 45] local 192.168.200.52 port 44153 connected to 192.168.200.101 port 5201
[ 47] local 192.168.200.52 port 37745 connected to 192.168.200.101 port 5201
[ 49] local 192.168.200.52 port 38321 connected to 192.168.200.101 port 5201
[ 51] local 192.168.200.52 port 53896 connected to 192.168.200.101 port 5201
[ 53] local 192.168.200.52 port 41404 connected to 192.168.200.101 port 5201
[ 55] local 192.168.200.52 port 34402 connected to 192.168.200.101 port 5201
[ 57] local 192.168.200.52 port 50171 connected to 192.168.200.101 port 5201
[ 59] local 192.168.200.52 port 50087 connected to 192.168.200.101 port 5201
[ 61] local 192.168.200.52 port 36007 connected to 192.168.200.101 port 5201
[ 63] local 192.168.200.52 port 37543 connected to 192.168.200.101 port 5201
[ 65] local 192.168.200.52 port 41108 connected to 192.168.200.101 port 5201
[ 67] local 192.168.200.52 port 45710 connected to 192.168.200.101 port 5201
[ 69] local 192.168.200.52 port 59818 connected to 192.168.200.101 port 5201
[ 71] local 192.168.200.52 port 46657 connected to 192.168.200.101 port 5201
[ 73] local 192.168.200.52 port 33316 connected to 192.168.200.101 port 5201
[ 75] local 192.168.200.52 port 42589 connected to 192.168.200.101 port 5201
[ 77] local 192.168.200.52 port 37762 connected to 192.168.200.101 port 5201
[ 79] local 192.168.200.52 port 40436 connected to 192.168.200.101 port 5201
[ 81] local 192.168.200.52 port 40390 connected to 192.168.200.101 port 5201
[ 83] local 192.168.200.52 port 36850 connected to 192.168.200.101 port 5201
[ 85] local 192.168.200.52 port 42445 connected to 192.168.200.101 port 5201
[ 87] local 192.168.200.52 port 60283 connected to 192.168.200.101 port 5201
[ 89] local 192.168.200.52 port 48879 connected to 192.168.200.101 port 5201
[ 91] local 192.168.200.52 port 36322 connected to 192.168.200.101 port 5201
[ 93] local 192.168.200.52 port 35925 connected to 192.168.200.101 port 5201
[ 95] local 192.168.200.52 port 39118 connected to 192.168.200.101 port 5201
[ 97] local 192.168.200.52 port 54802 connected to 192.168.200.101 port 5201
[ 99] local 192.168.200.52 port 33412 connected to 192.168.200.101 port 5201
[101] local 192.168.200.52 port 39567 connected to 192.168.200.101 port 5201
[103] local 192.168.200.52 port 56401 connected to 192.168.200.101 port 5201
[105] local 192.168.200.52 port 59370 connected to 192.168.200.101 port 5201
[107] local 192.168.200.52 port 51221 connected to 192.168.200.101 port 5201
[109] local 192.168.200.52 port 52724 connected to 192.168.200.101 port 5201
[111] local 192.168.200.52 port 35057 connected to 192.168.200.101 port 5201
[113] local 192.168.200.52 port 34672 connected to 192.168.200.101 port 5201
[115] local 192.168.200.52 port 51697 connected to 192.168.200.101 port 5201
[117] local 192.168.200.52 port 44060 connected to 192.168.200.101 port 5201
[119] local 192.168.200.52 port 55739 connected to 192.168.200.101 port 5201
[121] local 192.168.200.52 port 59949 connected to 192.168.200.101 port 5201
[123] local 192.168.200.52 port 52798 connected to 192.168.200.101 port 5201
[125] local 192.168.200.52 port 47439 connected to 192.168.200.101 port 5201
[127] local 192.168.200.52 port 45251 connected to 192.168.200.101 port 5201
[129] local 192.168.200.52 port 56131 connected to 192.168.200.101 port 5201
[131] local 192.168.200.52 port 45221 connected to 192.168.200.101 port 5201
[133] local 192.168.200.52 port 37859 connected to 192.168.200.101 port 5201
[135] local 192.168.200.52 port 55812 connected to 192.168.200.101 port 5201
[137] local 192.168.200.52 port 60437 connected to 192.168.200.101 port 5201
[139] local 192.168.200.52 port 53114 connected to 192.168.200.101 port 5201
[141] local 192.168.200.52 port 45082 connected to 192.168.200.101 port 5201
[143] local 192.168.200.52 port 52472 connected to 192.168.200.101 port 5201
[145] local 192.168.200.52 port 46713 connected to 192.168.200.101 port 5201
[147] local 192.168.200.52 port 44365 connected to 192.168.200.101 port 5201
[149] local 192.168.200.52 port 58393 connected to 192.168.200.101 port 5201
[151] local 192.168.200.52 port 60336 connected to 192.168.200.101 port 5201
[153] local 192.168.200.52 port 58590 connected to 192.168.200.101 port 5201
[155] local 192.168.200.52 port 48910 connected to 192.168.200.101 port 5201
[157] local 192.168.200.52 port 34654 connected to 192.168.200.101 port 5201
[159] local 192.168.200.52 port 38036 connected to 192.168.200.101 port 5201
[161] local 192.168.200.52 port 45668 connected to 192.168.200.101 port 5201
[163] local 192.168.200.52 port 60566 connected to 192.168.200.101 port 5201
[165] local 192.168.200.52 port 50696 connected to 192.168.200.101 port 5201
[167] local 192.168.200.52 port 44601 connected to 192.168.200.101 port 5201
[169] local 192.168.200.52 port 49554 connected to 192.168.200.101 port 5201
[171] local 192.168.200.52 port 54022 connected to 192.168.200.101 port 5201
[173] local 192.168.200.52 port 56380 connected to 192.168.200.101 port 5201
[175] local 192.168.200.52 port 33246 connected to 192.168.200.101 port 5201
[177] local 192.168.200.52 port 57046 connected to 192.168.200.101 port 5201
[179] local 192.168.200.52 port 33984 connected to 192.168.200.101 port 5201
[181] local 192.168.200.52 port 43534 connected to 192.168.200.101 port 5201
[183] local 192.168.200.52 port 40518 connected to 192.168.200.101 port 5201
[185] local 192.168.200.52 port 45046 connected to 192.168.200.101 port 5201
[187] local 192.168.200.52 port 32830 connected to 192.168.200.101 port 5201
[189] local 192.168.200.52 port 35221 connected to 192.168.200.101 port 5201
[191] local 192.168.200.52 port 38763 connected to 192.168.200.101 port 5201
[193] local 192.168.200.52 port 34009 connected to 192.168.200.101 port 5201
[195] local 192.168.200.52 port 43947 connected to 192.168.200.101 port 5201
[197] local 192.168.200.52 port 36566 connected to 192.168.200.101 port 5201
[199] local 192.168.200.52 port 33991 connected to 192.168.200.101 port 5201
[201] local 192.168.200.52 port 33016 connected to 192.168.200.101 port 5201
[203] local 192.168.200.52 port 40578 connected to 192.168.200.101 port 5201
[205] local 192.168.200.52 port 59804 connected to 192.168.200.101 port 5201
[207] local 192.168.200.52 port 44918 connected to 192.168.200.101 port 5201
[209] local 192.168.200.52 port 49034 connected to 192.168.200.101 port 5201
[211] local 192.168.200.52 port 51980 connected to 192.168.200.101 port 5201
[213] local 192.168.200.52 port 48874 connected to 192.168.200.101 port 5201
[215] local 192.168.200.52 port 34462 connected to 192.168.200.101 port 5201
[217] local 192.168.200.52 port 43413 connected to 192.168.200.101 port 5201
[219] local 192.168.200.52 port 34421 connected to 192.168.200.101 port 5201
[221] local 192.168.200.52 port 37903 connected to 192.168.200.101 port 5201
[223] local 192.168.200.52 port 44090 connected to 192.168.200.101 port 5201
[225] local 192.168.200.52 port 49716 connected to 192.168.200.101 port 5201
[227] local 192.168.200.52 port 35271 connected to 192.168.200.101 port 5201
[229] local 192.168.200.52 port 33368 connected to 192.168.200.101 port 5201
[231] local 192.168.200.52 port 38242 connected to 192.168.200.101 port 5201
[233] local 192.168.200.52 port 39909 connected to 192.168.200.101 port 5201
[235] local 192.168.200.52 port 36938 connected to 192.168.200.101 port 5201
[237] local 192.168.200.52 port 53594 connected to 192.168.200.101 port 5201
[239] local 192.168.200.52 port 55286 connected to 192.168.200.101 port 5201
[241] local 192.168.200.52 port 53061 connected to 192.168.200.101 port 5201
[243] local 192.168.200.52 port 34797 connected to 192.168.200.101 port 5201
[245] local 192.168.200.52 port 51054 connected to 192.168.200.101 port 5201
[247] local 192.168.200.52 port 44108 connected to 192.168.200.101 port 5201
[249] local 192.168.200.52 port 45835 connected to 192.168.200.101 port 5201
[251] local 192.168.200.52 port 54457 connected to 192.168.200.101 port 5201
[253] local 192.168.200.52 port 58471 connected to 192.168.200.101 port 5201
[255] local 192.168.200.52 port 44632 connected to 192.168.200.101 port 5201
[257] local 192.168.200.52 port 51291 connected to 192.168.200.101 port 5201
[259] local 192.168.200.52 port 41889 connected to 192.168.200.101 port 5201
[ ID] Interval           Transfer     Bitrate         Total Datagrams
[  5]   0.00-1.00   sec   129 KBytes  1.05 Mbits/sec  91
[  7]   0.00-1.00   sec   129 KBytes  1.05 Mbits/sec  91
[  9]   0.00-1.00   sec   129 KBytes  1.05 Mbits/sec  91
[ 11]   0.00-1.00   sec   129 KBytes  1.05 Mbits/sec  91
[ 13]   0.00-1.00   sec   129 KBytes  1.05 Mbits/sec  91
[ 15]   0.00-1.00   sec   129 KBytes  1.05 Mbits/sec  91
[ 17]   0.00-1.00   sec   129 KBytes  1.05 Mbits/sec  91
[ 19]   0.00-1.00   sec   129 KBytes  1.05 Mbits/sec  91
[ 21]   0.00-1.00   sec   129 KBytes  1.05 Mbits/sec  91
[ 23]   0.00-1.00   sec   129 KBytes  1.05 Mbits/sec  91
[ 25]   0.00-1.00   sec   129 KBytes  1.05 Mbits/sec  91
[ 27]   0.00-1.00   sec   129 KBytes  1.05 Mbits/sec  91
[ 29]   0.00-1.00   sec   129 KBytes  1.05 Mbits/sec  91
[ 31]   0.00-1.00   sec   129 KBytes  1.05 Mbits/sec  91
[ 33]   0.00-1.00   sec   129 KBytes  1.05 Mbits/sec  91
[ 35]   0.00-1.00   sec   129 KBytes  1.05 Mbits/sec  91
[ 37]   0.00-1.00   sec   129 KBytes  1.05 Mbits/sec  91
[ 39]   0.00-1.00   sec   129 KBytes  1.05 Mbits/sec  91
[ 41]   0.00-1.00   sec   129 KBytes  1.05 Mbits/sec  91
[ 43]   0.00-1.00   sec   129 KBytes  1.05 Mbits/sec  91
[ 45]   0.00-1.00   sec   129 KBytes  1.05 Mbits/sec  91
[ 47]   0.00-1.00   sec   129 KBytes  1.05 Mbits/sec  91
[ 49]   0.00-1.00   sec   129 KBytes  1.05 Mbits/sec  91
[ 51]   0.00-1.00   sec   129 KBytes  1.05 Mbits/sec  91
[ 53]   0.00-1.00   sec   129 KBytes  1.05 Mbits/sec  91
[ 55]   0.00-1.00   sec   129 KBytes  1.05 Mbits/sec  91
[ 57]   0.00-1.00   sec   129 KBytes  1.05 Mbits/sec  91
[ 59]   0.00-1.00   sec   129 KBytes  1.05 Mbits/sec  91
[ 61]   0.00-1.00   sec   129 KBytes  1.05 Mbits/sec  91
[ 63]   0.00-1.00   sec   129 KBytes  1.05 Mbits/sec  91
[ 65]   0.00-1.00   sec   129 KBytes  1.05 Mbits/sec  91
[ 67]   0.00-1.00   sec   129 KBytes  1.05 Mbits/sec  91
[ 69]   0.00-1.00   sec   129 KBytes  1.05 Mbits/sec  91
[ 71]   0.00-1.00   sec   129 KBytes  1.05 Mbits/sec  91
[ 73]   0.00-1.00   sec   129 KBytes  1.05 Mbits/sec  91
[ 75]   0.00-1.00   sec   129 KBytes  1.05 Mbits/sec  91
[ 77]   0.00-1.00   sec   129 KBytes  1.05 Mbits/sec  91
[ 79]   0.00-1.00   sec   129 KBytes  1.05 Mbits/sec  91
[ 81]   0.00-1.00   sec   129 KBytes  1.05 Mbits/sec  91
[ 83]   0.00-1.00   sec   129 KBytes  1.05 Mbits/sec  91
[ 85]   0.00-1.00   sec   129 KBytes  1.05 Mbits/sec  91
[ 87]   0.00-1.00   sec   129 KBytes  1.05 Mbits/sec  91
[ 89]   0.00-1.00   sec   129 KBytes  1.05 Mbits/sec  91
[ 91]   0.00-1.00   sec   129 KBytes  1.05 Mbits/sec  91
[ 93]   0.00-1.00   sec   129 KBytes  1.05 Mbits/sec  91
[ 95]   0.00-1.00   sec   129 KBytes  1.05 Mbits/sec  91
[ 97]   0.00-1.00   sec   129 KBytes  1.05 Mbits/sec  91
[ 99]   0.00-1.00   sec   129 KBytes  1.05 Mbits/sec  91
[101]   0.00-1.00   sec   129 KBytes  1.05 Mbits/sec  91
[103]   0.00-1.00   sec   129 KBytes  1.05 Mbits/sec  91
[105]   0.00-1.00   sec   129 KBytes  1.05 Mbits/sec  91
[107]   0.00-1.00   sec   129 KBytes  1.05 Mbits/sec  91
[109]   0.00-1.00   sec   129 KBytes  1.05 Mbits/sec  91
[111]   0.00-1.00   sec   129 KBytes  1.05 Mbits/sec  91
[113]   0.00-1.00   sec   129 KBytes  1.05 Mbits/sec  91
[115]   0.00-1.00   sec   129 KBytes  1.05 Mbits/sec  91
[117]   0.00-1.00   sec   129 KBytes  1.05 Mbits/sec  91
[119]   0.00-1.00   sec   129 KBytes  1.05 Mbits/sec  91
[121]   0.00-1.00   sec   129 KBytes  1.05 Mbits/sec  91
[123]   0.00-1.00   sec   129 KBytes  1.05 Mbits/sec  91
[125]   0.00-1.00   sec   129 KBytes  1.05 Mbits/sec  91
[127]   0.00-1.00   sec   129 KBytes  1.05 Mbits/sec  91
[129]   0.00-1.00   sec   129 KBytes  1.05 Mbits/sec  91
[131]   0.00-1.00   sec   129 KBytes  1.05 Mbits/sec  91
[133]   0.00-1.00   sec   129 KBytes  1.05 Mbits/sec  91
[135]   0.00-1.00   sec   129 KBytes  1.05 Mbits/sec  91
[137]   0.00-1.00   sec   129 KBytes  1.05 Mbits/sec  91
[139]   0.00-1.00   sec   129 KBytes  1.05 Mbits/sec  91
[141]   0.00-1.00   sec   129 KBytes  1.05 Mbits/sec  91
[143]   0.00-1.00   sec   129 KBytes  1.05 Mbits/sec  91
[145]   0.00-1.00   sec   129 KBytes  1.05 Mbits/sec  91
[147]   0.00-1.00   sec   129 KBytes  1.05 Mbits/sec  91
[149]   0.00-1.00   sec   129 KBytes  1.05 Mbits/sec  91
[151]   0.00-1.00   sec   129 KBytes  1.05 Mbits/sec  91
[153]   0.00-1.00   sec   129 KBytes  1.05 Mbits/sec  91
[155]   0.00-1.00   sec   129 KBytes  1.05 Mbits/sec  91
[157]   0.00-1.00   sec   129 KBytes  1.05 Mbits/sec  91
[159]   0.00-1.00   sec   129 KBytes  1.05 Mbits/sec  91
[161]   0.00-1.00   sec   129 KBytes  1.05 Mbits/sec  91
[163]   0.00-1.00   sec   129 KBytes  1.05 Mbits/sec  91
[165]   0.00-1.00   sec   129 KBytes  1.05 Mbits/sec  91
[167]   0.00-1.00   sec   129 KBytes  1.05 Mbits/sec  91
[169]   0.00-1.00   sec   129 KBytes  1.05 Mbits/sec  91
[171]   0.00-1.00   sec   129 KBytes  1.05 Mbits/sec  91
[173]   0.00-1.00   sec   129 KBytes  1.05 Mbits/sec  91
[175]   0.00-1.00   sec   129 KBytes  1.05 Mbits/sec  91
[177]   0.00-1.00   sec   129 KBytes  1.05 Mbits/sec  91
[179]   0.00-1.00   sec   129 KBytes  1.05 Mbits/sec  91
[181]   0.00-1.00   sec   129 KBytes  1.05 Mbits/sec  91
[183]   0.00-1.00   sec   129 KBytes  1.05 Mbits/sec  91
[185]   0.00-1.00   sec   129 KBytes  1.05 Mbits/sec  91
[187]   0.00-1.00   sec   129 KBytes  1.05 Mbits/sec  91
[189]   0.00-1.00   sec   129 KBytes  1.05 Mbits/sec  91
[191]   0.00-1.00   sec   129 KBytes  1.05 Mbits/sec  91
[193]   0.00-1.00   sec   129 KBytes  1.05 Mbits/sec  91
[195]   0.00-1.00   sec   129 KBytes  1.05 Mbits/sec  91
[197]   0.00-1.00   sec   129 KBytes  1.05 Mbits/sec  91
[199]   0.00-1.00   sec   129 KBytes  1.05 Mbits/sec  91
[201]   0.00-1.00   sec   129 KBytes  1.05 Mbits/sec  91
[203]   0.00-1.00   sec   129 KBytes  1.05 Mbits/sec  91
[205]   0.00-1.00   sec   129 KBytes  1.05 Mbits/sec  91
[207]   0.00-1.00   sec   129 KBytes  1.05 Mbits/sec  91
[209]   0.00-1.00   sec   129 KBytes  1.05 Mbits/sec  91
[211]   0.00-1.00   sec   129 KBytes  1.05 Mbits/sec  91
[213]   0.00-1.00   sec   129 KBytes  1.05 Mbits/sec  91
[215]   0.00-1.00   sec   129 KBytes  1.05 Mbits/sec  91
[217]   0.00-1.00   sec   129 KBytes  1.05 Mbits/sec  91
[219]   0.00-1.00   sec   129 KBytes  1.05 Mbits/sec  91
[221]   0.00-1.00   sec   129 KBytes  1.05 Mbits/sec  91
[223]   0.00-1.00   sec   129 KBytes  1.05 Mbits/sec  91
[225]   0.00-1.00   sec   129 KBytes  1.05 Mbits/sec  91
[227]   0.00-1.00   sec   129 KBytes  1.05 Mbits/sec  91
[229]   0.00-1.00   sec   129 KBytes  1.05 Mbits/sec  91
[231]   0.00-1.00   sec   129 KBytes  1.05 Mbits/sec  91
[233]   0.00-1.00   sec   129 KBytes  1.05 Mbits/sec  91
[235]   0.00-1.00   sec   129 KBytes  1.05 Mbits/sec  91
[237]   0.00-1.00   sec   129 KBytes  1.05 Mbits/sec  91
[239]   0.00-1.00   sec   129 KBytes  1.05 Mbits/sec  91
[241]   0.00-1.00   sec   129 KBytes  1.05 Mbits/sec  91
[243]   0.00-1.00   sec   129 KBytes  1.05 Mbits/sec  91
[245]   0.00-1.00   sec   129 KBytes  1.05 Mbits/sec  91
[247]   0.00-1.00   sec   129 KBytes  1.05 Mbits/sec  91
[249]   0.00-1.00   sec   129 KBytes  1.05 Mbits/sec  91
[251]   0.00-1.00   sec   129 KBytes  1.05 Mbits/sec  91
[253]   0.00-1.00   sec   129 KBytes  1.05 Mbits/sec  91
[255]   0.00-1.00   sec   129 KBytes  1.05 Mbits/sec  91
[257]   0.00-1.00   sec   129 KBytes  1.05 Mbits/sec  91
[259]   0.00-1.00   sec   129 KBytes  1.05 Mbits/sec  91
[SUM]   0.00-1.00   sec  16.1 MBytes   135 Mbits/sec  11648
- - - - - - - - - - - - - - - - - - - - - - - - -
[ ID] Interval           Transfer     Bitrate         Jitter    Lost/Total Datagrams
[  5]   0.00-30.28  sec  3.79 MBytes  1.05 Mbits/sec  0.000 ms  0/2742 (0%)  sender
[  5]   0.00-30.28  sec  0.00 Bytes  0.00 bits/sec  0.000 ms  0/0 (0%)  receiver
[  7]   0.00-30.28  sec  3.79 MBytes  1.05 Mbits/sec  0.000 ms  0/2742 (0%)  sender
[  7]   0.00-30.28  sec  0.00 Bytes  0.00 bits/sec  0.000 ms  0/0 (0%)  receiver
[  9]   0.00-30.28  sec  3.79 MBytes  1.05 Mbits/sec  0.000 ms  0/2742 (0%)  sender
[  9]   0.00-30.28  sec  0.00 Bytes  0.00 bits/sec  0.000 ms  0/0 (0%)  receiver
[ 11]   0.00-30.28  sec  3.79 MBytes  1.05 Mbits/sec  0.000 ms  0/2742 (0%)  sender
[ 11]   0.00-30.28  sec  0.00 Bytes  0.00 bits/sec  0.000 ms  0/0 (0%)  receiver
[ 13]   0.00-30.28  sec  3.79 MBytes  1.05 Mbits/sec  0.000 ms  0/2742 (0%)  sender
[ 13]   0.00-30.28  sec  0.00 Bytes  0.00 bits/sec  0.000 ms  0/0 (0%)  receiver
[ 15]   0.00-30.28  sec  3.79 MBytes  1.05 Mbits/sec  0.000 ms  0/2742 (0%)  sender
[ 15]   0.00-30.28  sec  0.00 Bytes  0.00 bits/sec  0.000 ms  0/0 (0%)  receiver
[ 17]   0.00-30.28  sec  3.79 MBytes  1.05 Mbits/sec  0.000 ms  0/2742 (0%)  sender
[ 17]   0.00-30.28  sec  0.00 Bytes  0.00 bits/sec  0.000 ms  0/0 (0%)  receiver
[ 19]   0.00-30.28  sec  3.79 MBytes  1.05 Mbits/sec  0.000 ms  0/2742 (0%)  sender
[ 19]   0.00-30.28  sec  0.00 Bytes  0.00 bits/sec  0.000 ms  0/0 (0%)  receiver
[ 21]   0.00-30.28  sec  3.79 MBytes  1.05 Mbits/sec  0.000 ms  0/2742 (0%)  sender
[ 21]   0.00-30.28  sec  0.00 Bytes  0.00 bits/sec  0.000 ms  0/0 (0%)  receiver
[ 23]   0.00-30.28  sec  3.79 MBytes  1.05 Mbits/sec  0.000 ms  0/2742 (0%)  sender
[ 23]   0.00-30.28  sec  0.00 Bytes  0.00 bits/sec  0.000 ms  0/0 (0%)  receiver
[ 25]   0.00-30.28  sec  3.79 MBytes  1.05 Mbits/sec  0.000 ms  0/2742 (0%)  sender
[ 25]   0.00-30.28  sec  0.00 Bytes  0.00 bits/sec  0.000 ms  0/0 (0%)  receiver
[ 27]   0.00-30.28  sec  3.79 MBytes  1.05 Mbits/sec  0.000 ms  0/2742 (0%)  sender
[ 27]   0.00-30.28  sec  0.00 Bytes  0.00 bits/sec  0.000 ms  0/0 (0%)  receiver
[ 29]   0.00-30.28  sec  3.79 MBytes  1.05 Mbits/sec  0.000 ms  0/2742 (0%)  sender
[ 29]   0.00-30.28  sec  0.00 Bytes  0.00 bits/sec  0.000 ms  0/0 (0%)  receiver
[ 31]   0.00-30.28  sec  3.79 MBytes  1.05 Mbits/sec  0.000 ms  0/2742 (0%)  sender
[ 31]   0.00-30.28  sec  0.00 Bytes  0.00 bits/sec  0.000 ms  0/0 (0%)  receiver
[ 33]   0.00-30.28  sec  3.79 MBytes  1.05 Mbits/sec  0.000 ms  0/2742 (0%)  sender
[ 33]   0.00-30.28  sec  0.00 Bytes  0.00 bits/sec  0.000 ms  0/0 (0%)  receiver
[ 35]   0.00-30.28  sec  3.79 MBytes  1.05 Mbits/sec  0.000 ms  0/2742 (0%)  sender
[ 35]   0.00-30.28  sec  0.00 Bytes  0.00 bits/sec  0.000 ms  0/0 (0%)  receiver
[ 37]   0.00-30.28  sec  3.79 MBytes  1.05 Mbits/sec  0.000 ms  0/2742 (0%)  sender
[ 37]   0.00-30.28  sec  0.00 Bytes  0.00 bits/sec  0.000 ms  0/0 (0%)  receiver
[ 39]   0.00-30.28  sec  3.79 MBytes  1.05 Mbits/sec  0.000 ms  0/2742 (0%)  sender
[ 39]   0.00-30.28  sec  0.00 Bytes  0.00 bits/sec  0.000 ms  0/0 (0%)  receiver
[ 41]   0.00-30.28  sec  3.79 MBytes  1.05 Mbits/sec  0.000 ms  0/2742 (0%)  sender
[ 41]   0.00-30.28  sec  0.00 Bytes  0.00 bits/sec  0.000 ms  0/0 (0%)  receiver
[ 43]   0.00-30.28  sec  3.79 MBytes  1.05 Mbits/sec  0.000 ms  0/2742 (0%)  sender
[ 43]   0.00-30.28  sec  0.00 Bytes  0.00 bits/sec  0.000 ms  0/0 (0%)  receiver
[ 45]   0.00-30.28  sec  3.79 MBytes  1.05 Mbits/sec  0.000 ms  0/2742 (0%)  sender
[ 45]   0.00-30.28  sec  0.00 Bytes  0.00 bits/sec  0.000 ms  0/0 (0%)  receiver
[ 47]   0.00-30.28  sec  3.79 MBytes  1.05 Mbits/sec  0.000 ms  0/2742 (0%)  sender
[ 47]   0.00-30.28  sec  0.00 Bytes  0.00 bits/sec  0.000 ms  0/0 (0%)  receiver
[ 49]   0.00-30.28  sec  3.79 MBytes  1.05 Mbits/sec  0.000 ms  0/2742 (0%)  sender
[ 49]   0.00-30.28  sec  0.00 Bytes  0.00 bits/sec  0.000 ms  0/0 (0%)  receiver
[ 51]   0.00-30.28  sec  3.79 MBytes  1.05 Mbits/sec  0.000 ms  0/2742 (0%)  sender
[ 51]   0.00-30.28  sec  0.00 Bytes  0.00 bits/sec  0.000 ms  0/0 (0%)  receiver
[ 53]   0.00-30.28  sec  3.79 MBytes  1.05 Mbits/sec  0.000 ms  0/2742 (0%)  sender
[ 53]   0.00-30.28  sec  0.00 Bytes  0.00 bits/sec  0.000 ms  0/0 (0%)  receiver
[ 55]   0.00-30.28  sec  3.79 MBytes  1.05 Mbits/sec  0.000 ms  0/2742 (0%)  sender
[ 55]   0.00-30.28  sec  0.00 Bytes  0.00 bits/sec  0.000 ms  0/0 (0%)  receiver
[ 57]   0.00-30.28  sec  3.79 MBytes  1.05 Mbits/sec  0.000 ms  0/2742 (0%)  sender
[ 57]   0.00-30.28  sec  0.00 Bytes  0.00 bits/sec  0.000 ms  0/0 (0%)  receiver
[ 59]   0.00-30.28  sec  3.79 MBytes  1.05 Mbits/sec  0.000 ms  0/2742 (0%)  sender
[ 59]   0.00-30.28  sec  0.00 Bytes  0.00 bits/sec  0.000 ms  0/0 (0%)  receiver
[ 61]   0.00-30.28  sec  3.79 MBytes  1.05 Mbits/sec  0.000 ms  0/2742 (0%)  sender
[ 61]   0.00-30.28  sec  0.00 Bytes  0.00 bits/sec  0.000 ms  0/0 (0%)  receiver
[ 63]   0.00-30.28  sec  3.79 MBytes  1.05 Mbits/sec  0.000 ms  0/2742 (0%)  sender
[ 63]   0.00-30.28  sec  0.00 Bytes  0.00 bits/sec  0.000 ms  0/0 (0%)  receiver
[ 65]   0.00-30.28  sec  3.79 MBytes  1.05 Mbits/sec  0.000 ms  0/2742 (0%)  sender
[ 65]   0.00-30.28  sec  0.00 Bytes  0.00 bits/sec  0.000 ms  0/0 (0%)  receiver
[ 67]   0.00-30.28  sec  3.79 MBytes  1.05 Mbits/sec  0.000 ms  0/2742 (0%)  sender
[ 67]   0.00-30.28  sec  0.00 Bytes  0.00 bits/sec  0.000 ms  0/0 (0%)  receiver
[ 69]   0.00-30.28  sec  3.79 MBytes  1.05 Mbits/sec  0.000 ms  0/2742 (0%)  sender
[ 69]   0.00-30.28  sec  0.00 Bytes  0.00 bits/sec  0.000 ms  0/0 (0%)  receiver
[ 71]   0.00-30.28  sec  3.79 MBytes  1.05 Mbits/sec  0.000 ms  0/2742 (0%)  sender
[ 71]   0.00-30.28  sec  0.00 Bytes  0.00 bits/sec  0.000 ms  0/0 (0%)  receiver
[ 73]   0.00-30.28  sec  3.79 MBytes  1.05 Mbits/sec  0.000 ms  0/2742 (0%)  sender
[ 73]   0.00-30.28  sec  0.00 Bytes  0.00 bits/sec  0.000 ms  0/0 (0%)  receiver
[ 75]   0.00-30.28  sec  3.79 MBytes  1.05 Mbits/sec  0.000 ms  0/2742 (0%)  sender
[ 75]   0.00-30.28  sec  0.00 Bytes  0.00 bits/sec  0.000 ms  0/0 (0%)  receiver
[ 77]   0.00-30.28  sec  3.79 MBytes  1.05 Mbits/sec  0.000 ms  0/2742 (0%)  sender
[ 77]   0.00-30.28  sec  0.00 Bytes  0.00 bits/sec  0.000 ms  0/0 (0%)  receiver
[ 79]   0.00-30.28  sec  3.79 MBytes  1.05 Mbits/sec  0.000 ms  0/2742 (0%)  sender
[ 79]   0.00-30.28  sec  0.00 Bytes  0.00 bits/sec  0.000 ms  0/0 (0%)  receiver
[ 81]   0.00-30.28  sec  3.79 MBytes  1.05 Mbits/sec  0.000 ms  0/2742 (0%)  sender
[ 81]   0.00-30.28  sec  0.00 Bytes  0.00 bits/sec  0.000 ms  0/0 (0%)  receiver
[ 83]   0.00-30.28  sec  3.79 MBytes  1.05 Mbits/sec  0.000 ms  0/2742 (0%)  sender
[ 83]   0.00-30.28  sec  0.00 Bytes  0.00 bits/sec  0.000 ms  0/0 (0%)  receiver
[ 85]   0.00-30.28  sec  3.79 MBytes  1.05 Mbits/sec  0.000 ms  0/2742 (0%)  sender
[ 85]   0.00-30.28  sec  0.00 Bytes  0.00 bits/sec  0.000 ms  0/0 (0%)  receiver
[ 87]   0.00-30.28  sec  3.79 MBytes  1.05 Mbits/sec  0.000 ms  0/2742 (0%)  sender
[ 87]   0.00-30.28  sec  0.00 Bytes  0.00 bits/sec  0.000 ms  0/0 (0%)  receiver
[ 89]   0.00-30.28  sec  3.79 MBytes  1.05 Mbits/sec  0.000 ms  0/2742 (0%)  sender
[ 89]   0.00-30.28  sec  0.00 Bytes  0.00 bits/sec  0.000 ms  0/0 (0%)  receiver
[ 91]   0.00-30.28  sec  3.79 MBytes  1.05 Mbits/sec  0.000 ms  0/2742 (0%)  sender
[ 91]   0.00-30.28  sec  0.00 Bytes  0.00 bits/sec  0.000 ms  0/0 (0%)  receiver
[ 93]   0.00-30.28  sec  3.79 MBytes  1.05 Mbits/sec  0.000 ms  0/2742 (0%)  sender
[ 93]   0.00-30.28  sec  0.00 Bytes  0.00 bits/sec  0.000 ms  0/0 (0%)  receiver
[ 95]   0.00-30.28  sec  3.79 MBytes  1.05 Mbits/sec  0.000 ms  0/2742 (0%)  sender
[ 95]   0.00-30.28  sec  0.00 Bytes  0.00 bits/sec  0.000 ms  0/0 (0%)  receiver
[ 97]   0.00-30.28  sec  3.79 MBytes  1.05 Mbits/sec  0.000 ms  0/2742 (0%)  sender
[ 97]   0.00-30.28  sec  0.00 Bytes  0.00 bits/sec  0.000 ms  0/0 (0%)  receiver
[ 99]   0.00-30.28  sec  3.79 MBytes  1.05 Mbits/sec  0.000 ms  0/2742 (0%)  sender
[ 99]   0.00-30.28  sec  0.00 Bytes  0.00 bits/sec  0.000 ms  0/0 (0%)  receiver
[101]   0.00-30.28  sec  3.79 MBytes  1.05 Mbits/sec  0.000 ms  0/2742 (0%)  sender
[101]   0.00-30.28  sec  0.00 Bytes  0.00 bits/sec  0.000 ms  0/0 (0%)  receiver
[103]   0.00-30.28  sec  3.79 MBytes  1.05 Mbits/sec  0.000 ms  0/2742 (0%)  sender
[103]   0.00-30.28  sec  0.00 Bytes  0.00 bits/sec  0.000 ms  0/0 (0%)  receiver
[105]   0.00-30.28  sec  3.79 MBytes  1.05 Mbits/sec  0.000 ms  0/2741 (0%)  sender
[105]   0.00-30.28  sec  0.00 Bytes  0.00 bits/sec  0.000 ms  0/0 (0%)  receiver
[107]   0.00-30.28  sec  3.79 MBytes  1.05 Mbits/sec  0.000 ms  0/2741 (0%)  sender
[107]   0.00-30.28  sec  0.00 Bytes  0.00 bits/sec  0.000 ms  0/0 (0%)  receiver
[109]   0.00-30.28  sec  3.79 MBytes  1.05 Mbits/sec  0.000 ms  0/2741 (0%)  sender
[109]   0.00-30.28  sec  0.00 Bytes  0.00 bits/sec  0.000 ms  0/0 (0%)  receiver
[111]   0.00-30.28  sec  3.79 MBytes  1.05 Mbits/sec  0.000 ms  0/2741 (0%)  sender
[111]   0.00-30.28  sec  0.00 Bytes  0.00 bits/sec  0.000 ms  0/0 (0%)  receiver
[113]   0.00-30.28  sec  3.79 MBytes  1.05 Mbits/sec  0.000 ms  0/2741 (0%)  sender
[113]   0.00-30.28  sec  0.00 Bytes  0.00 bits/sec  0.000 ms  0/0 (0%)  receiver
[115]   0.00-30.28  sec  3.79 MBytes  1.05 Mbits/sec  0.000 ms  0/2741 (0%)  sender
[115]   0.00-30.28  sec  0.00 Bytes  0.00 bits/sec  0.000 ms  0/0 (0%)  receiver
[117]   0.00-30.28  sec  3.79 MBytes  1.05 Mbits/sec  0.000 ms  0/2741 (0%)  sender
[117]   0.00-30.28  sec  0.00 Bytes  0.00 bits/sec  0.000 ms  0/0 (0%)  receiver
[119]   0.00-30.28  sec  3.79 MBytes  1.05 Mbits/sec  0.000 ms  0/2741 (0%)  sender
[119]   0.00-30.28  sec  0.00 Bytes  0.00 bits/sec  0.000 ms  0/0 (0%)  receiver
[121]   0.00-30.28  sec  3.79 MBytes  1.05 Mbits/sec  0.000 ms  0/2741 (0%)  sender
[121]   0.00-30.28  sec  0.00 Bytes  0.00 bits/sec  0.000 ms  0/0 (0%)  receiver
[123]   0.00-30.28  sec  3.79 MBytes  1.05 Mbits/sec  0.000 ms  0/2741 (0%)  sender
[123]   0.00-30.28  sec  0.00 Bytes  0.00 bits/sec  0.000 ms  0/0 (0%)  receiver
[125]   0.00-30.28  sec  3.79 MBytes  1.05 Mbits/sec  0.000 ms  0/2741 (0%)  sender
[125]   0.00-30.28  sec  0.00 Bytes  0.00 bits/sec  0.000 ms  0/0 (0%)  receiver
[127]   0.00-30.28  sec  3.79 MBytes  1.05 Mbits/sec  0.000 ms  0/2741 (0%)  sender
[127]   0.00-30.28  sec  0.00 Bytes  0.00 bits/sec  0.000 ms  0/0 (0%)  receiver
[129]   0.00-30.28  sec  3.79 MBytes  1.05 Mbits/sec  0.000 ms  0/2741 (0%)  sender
[129]   0.00-30.28  sec  0.00 Bytes  0.00 bits/sec  0.000 ms  0/0 (0%)  receiver
[131]   0.00-30.28  sec  3.79 MBytes  1.05 Mbits/sec  0.000 ms  0/2741 (0%)  sender
[131]   0.00-30.28  sec  0.00 Bytes  0.00 bits/sec  0.000 ms  0/0 (0%)  receiver
[133]   0.00-30.28  sec  3.79 MBytes  1.05 Mbits/sec  0.000 ms  0/2741 (0%)  sender
[133]   0.00-30.28  sec  0.00 Bytes  0.00 bits/sec  0.000 ms  0/0 (0%)  receiver
[135]   0.00-30.28  sec  3.79 MBytes  1.05 Mbits/sec  0.000 ms  0/2741 (0%)  sender
[135]   0.00-30.28  sec  0.00 Bytes  0.00 bits/sec  0.000 ms  0/0 (0%)  receiver
[137]   0.00-30.28  sec  3.79 MBytes  1.05 Mbits/sec  0.000 ms  0/2741 (0%)  sender
[137]   0.00-30.28  sec  0.00 Bytes  0.00 bits/sec  0.000 ms  0/0 (0%)  receiver
[139]   0.00-30.28  sec  3.79 MBytes  1.05 Mbits/sec  0.000 ms  0/2741 (0%)  sender
[139]   0.00-30.28  sec  0.00 Bytes  0.00 bits/sec  0.000 ms  0/0 (0%)  receiver
[141]   0.00-30.28  sec  3.79 MBytes  1.05 Mbits/sec  0.000 ms  0/2741 (0%)  sender
[141]   0.00-30.28  sec  0.00 Bytes  0.00 bits/sec  0.000 ms  0/0 (0%)  receiver
[143]   0.00-30.28  sec  3.79 MBytes  1.05 Mbits/sec  0.000 ms  0/2741 (0%)  sender
[143]   0.00-30.28  sec  0.00 Bytes  0.00 bits/sec  0.000 ms  0/0 (0%)  receiver
[145]   0.00-30.28  sec  3.79 MBytes  1.05 Mbits/sec  0.000 ms  0/2741 (0%)  sender
[145]   0.00-30.28  sec  0.00 Bytes  0.00 bits/sec  0.000 ms  0/0 (0%)  receiver
[147]   0.00-30.28  sec  3.79 MBytes  1.05 Mbits/sec  0.000 ms  0/2741 (0%)  sender
[147]   0.00-30.28  sec  0.00 Bytes  0.00 bits/sec  0.000 ms  0/0 (0%)  receiver
[149]   0.00-30.28  sec  3.79 MBytes  1.05 Mbits/sec  0.000 ms  0/2741 (0%)  sender
[149]   0.00-30.28  sec  0.00 Bytes  0.00 bits/sec  0.000 ms  0/0 (0%)  receiver
[151]   0.00-30.28  sec  3.79 MBytes  1.05 Mbits/sec  0.000 ms  0/2741 (0%)  sender
[151]   0.00-30.28  sec  0.00 Bytes  0.00 bits/sec  0.000 ms  0/0 (0%)  receiver
[153]   0.00-30.28  sec  3.79 MBytes  1.05 Mbits/sec  0.000 ms  0/2741 (0%)  sender
[153]   0.00-30.28  sec  0.00 Bytes  0.00 bits/sec  0.000 ms  0/0 (0%)  receiver
[155]   0.00-30.28  sec  3.79 MBytes  1.05 Mbits/sec  0.000 ms  0/2741 (0%)  sender
[155]   0.00-30.28  sec  0.00 Bytes  0.00 bits/sec  0.000 ms  0/0 (0%)  receiver
[157]   0.00-30.28  sec  3.79 MBytes  1.05 Mbits/sec  0.000 ms  0/2741 (0%)  sender
[157]   0.00-30.28  sec  0.00 Bytes  0.00 bits/sec  0.000 ms  0/0 (0%)  receiver
[159]   0.00-30.28  sec  3.79 MBytes  1.05 Mbits/sec  0.000 ms  0/2741 (0%)  sender
[159]   0.00-30.28  sec  0.00 Bytes  0.00 bits/sec  0.000 ms  0/0 (0%)  receiver
[161]   0.00-30.28  sec  3.79 MBytes  1.05 Mbits/sec  0.000 ms  0/2741 (0%)  sender
[161]   0.00-30.28  sec  0.00 Bytes  0.00 bits/sec  0.000 ms  0/0 (0%)  receiver
[163]   0.00-30.28  sec  3.79 MBytes  1.05 Mbits/sec  0.000 ms  0/2741 (0%)  sender
[163]   0.00-30.28  sec  0.00 Bytes  0.00 bits/sec  0.000 ms  0/0 (0%)  receiver
[165]   0.00-30.28  sec  3.79 MBytes  1.05 Mbits/sec  0.000 ms  0/2741 (0%)  sender
[165]   0.00-30.28  sec  0.00 Bytes  0.00 bits/sec  0.000 ms  0/0 (0%)  receiver
[167]   0.00-30.28  sec  3.79 MBytes  1.05 Mbits/sec  0.000 ms  0/2741 (0%)  sender
[167]   0.00-30.28  sec  0.00 Bytes  0.00 bits/sec  0.000 ms  0/0 (0%)  receiver
[169]   0.00-30.28  sec  3.79 MBytes  1.05 Mbits/sec  0.000 ms  0/2741 (0%)  sender
[169]   0.00-30.28  sec  0.00 Bytes  0.00 bits/sec  0.000 ms  0/0 (0%)  receiver
[171]   0.00-30.28  sec  3.79 MBytes  1.05 Mbits/sec  0.000 ms  0/2741 (0%)  sender
[171]   0.00-30.28  sec  0.00 Bytes  0.00 bits/sec  0.000 ms  0/0 (0%)  receiver
[173]   0.00-30.28  sec  3.79 MBytes  1.05 Mbits/sec  0.000 ms  0/2741 (0%)  sender
[173]   0.00-30.28  sec  0.00 Bytes  0.00 bits/sec  0.000 ms  0/0 (0%)  receiver
[175]   0.00-30.28  sec  3.79 MBytes  1.05 Mbits/sec  0.000 ms  0/2741 (0%)  sender
[175]   0.00-30.28  sec  0.00 Bytes  0.00 bits/sec  0.000 ms  0/0 (0%)  receiver
[177]   0.00-30.28  sec  3.79 MBytes  1.05 Mbits/sec  0.000 ms  0/2741 (0%)  sender
[177]   0.00-30.28  sec  0.00 Bytes  0.00 bits/sec  0.000 ms  0/0 (0%)  receiver
[179]   0.00-30.28  sec  3.79 MBytes  1.05 Mbits/sec  0.000 ms  0/2741 (0%)  sender
[179]   0.00-30.28  sec  0.00 Bytes  0.00 bits/sec  0.000 ms  0/0 (0%)  receiver
[181]   0.00-30.28  sec  3.79 MBytes  1.05 Mbits/sec  0.000 ms  0/2741 (0%)  sender
[181]   0.00-30.28  sec  0.00 Bytes  0.00 bits/sec  0.000 ms  0/0 (0%)  receiver
[183]   0.00-30.28  sec  3.79 MBytes  1.05 Mbits/sec  0.000 ms  0/2741 (0%)  sender
[183]   0.00-30.28  sec  0.00 Bytes  0.00 bits/sec  0.000 ms  0/0 (0%)  receiver
[185]   0.00-30.28  sec  3.79 MBytes  1.05 Mbits/sec  0.000 ms  0/2741 (0%)  sender
[185]   0.00-30.28  sec  0.00 Bytes  0.00 bits/sec  0.000 ms  0/0 (0%)  receiver
[187]   0.00-30.28  sec  3.79 MBytes  1.05 Mbits/sec  0.000 ms  0/2741 (0%)  sender
[187]   0.00-30.28  sec  0.00 Bytes  0.00 bits/sec  0.000 ms  0/0 (0%)  receiver
[189]   0.00-30.28  sec  3.79 MBytes  1.05 Mbits/sec  0.000 ms  0/2741 (0%)  sender
[189]   0.00-30.28  sec  0.00 Bytes  0.00 bits/sec  0.000 ms  0/0 (0%)  receiver
[191]   0.00-30.28  sec  3.79 MBytes  1.05 Mbits/sec  0.000 ms  0/2741 (0%)  sender
[191]   0.00-30.28  sec  0.00 Bytes  0.00 bits/sec  0.000 ms  0/0 (0%)  receiver
[193]   0.00-30.28  sec  3.79 MBytes  1.05 Mbits/sec  0.000 ms  0/2741 (0%)  sender
[193]   0.00-30.28  sec  0.00 Bytes  0.00 bits/sec  0.000 ms  0/0 (0%)  receiver
[195]   0.00-30.28  sec  3.79 MBytes  1.05 Mbits/sec  0.000 ms  0/2741 (0%)  sender
[195]   0.00-30.28  sec  0.00 Bytes  0.00 bits/sec  0.000 ms  0/0 (0%)  receiver
[197]   0.00-30.28  sec  3.79 MBytes  1.05 Mbits/sec  0.000 ms  0/2741 (0%)  sender
[197]   0.00-30.28  sec  0.00 Bytes  0.00 bits/sec  0.000 ms  0/0 (0%)  receiver
[199]   0.00-30.28  sec  3.79 MBytes  1.05 Mbits/sec  0.000 ms  0/2741 (0%)  sender
[199]   0.00-30.28  sec  0.00 Bytes  0.00 bits/sec  0.000 ms  0/0 (0%)  receiver
[201]   0.00-30.28  sec  3.79 MBytes  1.05 Mbits/sec  0.000 ms  0/2741 (0%)  sender
[201]   0.00-30.28  sec  0.00 Bytes  0.00 bits/sec  0.000 ms  0/0 (0%)  receiver
[203]   0.00-30.28  sec  3.79 MBytes  1.05 Mbits/sec  0.000 ms  0/2741 (0%)  sender
[203]   0.00-30.28  sec  0.00 Bytes  0.00 bits/sec  0.000 ms  0/0 (0%)  receiver
[205]   0.00-30.28  sec  3.79 MBytes  1.05 Mbits/sec  0.000 ms  0/2741 (0%)  sender
[205]   0.00-30.28  sec  0.00 Bytes  0.00 bits/sec  0.000 ms  0/0 (0%)  receiver
[207]   0.00-30.28  sec  3.79 MBytes  1.05 Mbits/sec  0.000 ms  0/2741 (0%)  sender
[207]   0.00-30.28  sec  0.00 Bytes  0.00 bits/sec  0.000 ms  0/0 (0%)  receiver
[209]   0.00-30.28  sec  3.79 MBytes  1.05 Mbits/sec  0.000 ms  0/2741 (0%)  sender
[209]   0.00-30.28  sec  0.00 Bytes  0.00 bits/sec  0.000 ms  0/0 (0%)  receiver
[211]   0.00-30.28  sec  3.79 MBytes  1.05 Mbits/sec  0.000 ms  0/2741 (0%)  sender
[211]   0.00-30.28  sec  0.00 Bytes  0.00 bits/sec  0.000 ms  0/0 (0%)  receiver
[213]   0.00-30.28  sec  3.79 MBytes  1.05 Mbits/sec  0.000 ms  0/2741 (0%)  sender
[213]   0.00-30.28  sec  0.00 Bytes  0.00 bits/sec  0.000 ms  0/0 (0%)  receiver
[215]   0.00-30.28  sec  3.79 MBytes  1.05 Mbits/sec  0.000 ms  0/2741 (0%)  sender
[215]   0.00-30.28  sec  0.00 Bytes  0.00 bits/sec  0.000 ms  0/0 (0%)  receiver
[217]   0.00-30.28  sec  3.79 MBytes  1.05 Mbits/sec  0.000 ms  0/2741 (0%)  sender
[217]   0.00-30.28  sec  0.00 Bytes  0.00 bits/sec  0.000 ms  0/0 (0%)  receiver
[219]   0.00-30.28  sec  3.79 MBytes  1.05 Mbits/sec  0.000 ms  0/2741 (0%)  sender
[219]   0.00-30.28  sec  0.00 Bytes  0.00 bits/sec  0.000 ms  0/0 (0%)  receiver
[221]   0.00-30.28  sec  3.79 MBytes  1.05 Mbits/sec  0.000 ms  0/2741 (0%)  sender
[221]   0.00-30.28  sec  0.00 Bytes  0.00 bits/sec  0.000 ms  0/0 (0%)  receiver
[223]   0.00-30.28  sec  3.79 MBytes  1.05 Mbits/sec  0.000 ms  0/2741 (0%)  sender
[223]   0.00-30.28  sec  0.00 Bytes  0.00 bits/sec  0.000 ms  0/0 (0%)  receiver
[225]   0.00-30.28  sec  3.79 MBytes  1.05 Mbits/sec  0.000 ms  0/2741 (0%)  sender
[225]   0.00-30.28  sec  0.00 Bytes  0.00 bits/sec  0.000 ms  0/0 (0%)  receiver
[227]   0.00-30.28  sec  3.79 MBytes  1.05 Mbits/sec  0.000 ms  0/2741 (0%)  sender
[227]   0.00-30.28  sec  0.00 Bytes  0.00 bits/sec  0.000 ms  0/0 (0%)  receiver
[229]   0.00-30.28  sec  3.79 MBytes  1.05 Mbits/sec  0.000 ms  0/2741 (0%)  sender
[229]   0.00-30.28  sec  0.00 Bytes  0.00 bits/sec  0.000 ms  0/0 (0%)  receiver
[231]   0.00-30.28  sec  3.79 MBytes  1.05 Mbits/sec  0.000 ms  0/2741 (0%)  sender
[231]   0.00-30.28  sec  0.00 Bytes  0.00 bits/sec  0.000 ms  0/0 (0%)  receiver
[233]   0.00-30.28  sec  3.79 MBytes  1.05 Mbits/sec  0.000 ms  0/2741 (0%)  sender
[233]   0.00-30.28  sec  0.00 Bytes  0.00 bits/sec  0.000 ms  0/0 (0%)  receiver
[235]   0.00-30.28  sec  3.79 MBytes  1.05 Mbits/sec  0.000 ms  0/2741 (0%)  sender
[235]   0.00-30.28  sec  0.00 Bytes  0.00 bits/sec  0.000 ms  0/0 (0%)  receiver
[237]   0.00-30.28  sec  3.79 MBytes  1.05 Mbits/sec  0.000 ms  0/2741 (0%)  sender
[237]   0.00-30.28  sec  0.00 Bytes  0.00 bits/sec  0.000 ms  0/0 (0%)  receiver
[239]   0.00-30.28  sec  3.79 MBytes  1.05 Mbits/sec  0.000 ms  0/2741 (0%)  sender
[239]   0.00-30.28  sec  0.00 Bytes  0.00 bits/sec  0.000 ms  0/0 (0%)  receiver
[241]   0.00-30.28  sec  3.79 MBytes  1.05 Mbits/sec  0.000 ms  0/2741 (0%)  sender
[241]   0.00-30.28  sec  0.00 Bytes  0.00 bits/sec  0.000 ms  0/0 (0%)  receiver
[243]   0.00-30.28  sec  3.79 MBytes  1.05 Mbits/sec  0.000 ms  0/2741 (0%)  sender
[243]   0.00-30.28  sec  0.00 Bytes  0.00 bits/sec  0.000 ms  0/0 (0%)  receiver
[245]   0.00-30.28  sec  3.79 MBytes  1.05 Mbits/sec  0.000 ms  0/2741 (0%)  sender
[245]   0.00-30.28  sec  0.00 Bytes  0.00 bits/sec  0.000 ms  0/0 (0%)  receiver
[247]   0.00-30.28  sec  3.79 MBytes  1.05 Mbits/sec  0.000 ms  0/2741 (0%)  sender
[247]   0.00-30.28  sec  0.00 Bytes  0.00 bits/sec  0.000 ms  0/0 (0%)  receiver
[249]   0.00-30.28  sec  3.79 MBytes  1.05 Mbits/sec  0.000 ms  0/2741 (0%)  sender
[249]   0.00-30.28  sec  0.00 Bytes  0.00 bits/sec  0.000 ms  0/0 (0%)  receiver
[251]   0.00-30.28  sec  3.79 MBytes  1.05 Mbits/sec  0.000 ms  0/2741 (0%)  sender
[251]   0.00-30.28  sec  0.00 Bytes  0.00 bits/sec  0.000 ms  0/0 (0%)  receiver
[253]   0.00-30.28  sec  3.79 MBytes  1.05 Mbits/sec  0.000 ms  0/2741 (0%)  sender
[253]   0.00-30.28  sec  0.00 Bytes  0.00 bits/sec  0.000 ms  0/0 (0%)  receiver
[255]   0.00-30.28  sec  3.79 MBytes  1.05 Mbits/sec  0.000 ms  0/2741 (0%)  sender
[255]   0.00-30.28  sec  0.00 Bytes  0.00 bits/sec  0.000 ms  0/0 (0%)  receiver
[257]   0.00-30.28  sec  3.79 MBytes  1.05 Mbits/sec  0.000 ms  0/2741 (0%)  sender
[257]   0.00-30.28  sec  0.00 Bytes  0.00 bits/sec  0.000 ms  0/0 (0%)  receiver
[259]   0.00-30.28  sec  3.79 MBytes  1.05 Mbits/sec  0.000 ms  0/2741 (0%)  sender
[259]   0.00-30.28  sec  0.00 Bytes  0.00 bits/sec  0.000 ms  0/0 (0%)  receiver
[SUM]   0.00-30.28  sec   485 MBytes   134 Mbits/sec  0.000 ms  0/350898 (0%)  sender
[SUM]   0.00-30.28  sec  0.00 Bytes  0.00 bits/sec  0.000 ms  0/0 (0%)  receiver
iperf3: interrupt - the client has terminated

real    0m30.551s
user    0m4.006s
sys     0m9.785s
```
```bash
time for i in `seq 1 3000`; do touch testfile$i; done

real    0m7.034s
user    0m2.332s
sys     0m4.769s

time for i in `seq 1 3000`; do rm -rf testfile$i; done

real    0m8.194s
user    0m2.558s
sys     0m5.693s
```

Unfortunately, the server is running out of disk space when trying to run the load and stress tests.


