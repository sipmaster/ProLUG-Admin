```bash
[root@rocky14 ~]# mkdir c_practice

[root@rocky14 ~]# cd c_practice

[root@rocky14 c_practice]# vi a.c

[root@rocky14 c_practice]# gcc a.c

-bash: gcc: command not found

[root@rocky14 c_practice]# dnf install -y gcc

Last metadata expiration check: 0:30:34 ago on Thu May 22 11:03:19 2025.

Dependencies resolved.

==============================================================================================================================================================================================================

Package                                                                                                    Architecture                                                          Version                                                                                                    Repository                                                                      Size

==============================================================================================================================================================================================================

Installing:

gcc                                                                                                          x86_64                                                                      11.5.0-5.el9_5                                                                                      appstream                                                                        32 M

Upgrading:

glibc                                                                                                      x86_64                                                                      2.34-125.el9_5.8                                                                                  baseos                                                                            1.9 M

glibc-common                                                                                        x86_64                                                                      2.34-125.el9_5.8                                                                                  baseos                                                                            290 k

glibc-minimal-langpack                                                                    x86_64                                                                      2.34-125.el9_5.8                                                                                  baseos                                                                              16 k

libgcc                                                                                                    x86_64                                                                      11.5.0-5.el9_5                                                                                      baseos                                                                              84 k

libgomp                                                                                                  x86_64                                                                      11.5.0-5.el9_5                                                                                      baseos                                                                            260 k

Installing dependencies:

cpp                                                                                                          x86_64                                                                      11.5.0-5.el9_5                                                                                      appstream                                                                        11 M

glibc-devel                                                                                          x86_64                                                                      2.34-125.el9_5.8                                                                                  appstream                                                                        25 k

glibc-headers                                                                                      x86_64                                                                      2.34-125.el9_5.8                                                                                  appstream                                                                      429 k

kernel-headers                                                                                    x86_64                                                                      5.14.0-503.40.1.el9_5                                                                        appstream                                                                      3.5 M

libmpc                                                                                                    x86_64                                                                      1.2.1-4.el9                                                                                            appstream                                                                        61 k

libpkgconf                                                                                            x86_64                                                                      1.7.3-10.el9                                                                                          baseos                                                                              35 k

libxcrypt-devel                                                                                  x86_64                                                                      4.4.18-3.el9                                                                                          appstream                                                                        28 k

pkgconf                                                                                                  x86_64                                                                      1.7.3-10.el9                                                                                          baseos                                                                              40 k

pkgconf-m4                                                                                            noarch                                                                      1.7.3-10.el9                                                                                          baseos                                                                              14 k

pkgconf-pkg-config                                                                            x86_64                                                                      1.7.3-10.el9                                                                                          baseos                                                                              10 k

  

Transaction Summary

==============================================================================================================================================================================================================

Install    11 Packages

Upgrade      5 Packages

  

Total download size: 50 M

Downloading Packages:

(1/16): pkgconf-pkg-config-1.7.3-10.el9.x86_64.rpm                                                                                                                                                                                                                                                          50 kB/s |    10 kB          00:00

(2/16): pkgconf-m4-1.7.3-10.el9.noarch.rpm                                                                                                                                                                                                                                                                          50 kB/s |    14 kB          00:00

(3/16): pkgconf-1.7.3-10.el9.x86_64.rpm                                                                                                                                                                                                                                                                              116 kB/s |    40 kB          00:00

(4/16): libpkgconf-1.7.3-10.el9.x86_64.rpm                                                                                                                                                                                                                                                                        191 kB/s |    35 kB          00:00

(5/16): libxcrypt-devel-4.4.18-3.el9.x86_64.rpm                                                                                                                                                                                                                                                              116 kB/s |    28 kB          00:00

(6/16): libmpc-1.2.1-4.el9.x86_64.rpm                                                                                                                                                                                                                                                                                  201 kB/s |    61 kB          00:00

(7/16): glibc-headers-2.34-125.el9_5.8.x86_64.rpm                                                                                                                                                                                                                                                          1.5 MB/s | 429 kB          00:00

(8/16): glibc-devel-2.34-125.el9_5.8.x86_64.rpm                                                                                                                                                                                                                                                              225 kB/s |    25 kB          00:00

(9/16): cpp-11.5.0-5.el9_5.x86_64.rpm                                                                                                                                                                                                                                                                                    12 MB/s |    11 MB          00:00

(10/16): kernel-headers-5.14.0-503.40.1.el9_5.x86_64.rpm                                                                                                                                                                                                                                            5.9 MB/s | 3.5 MB          00:00

(11/16): libgomp-11.5.0-5.el9_5.x86_64.rpm                                                                                                                                                                                                                                                                        737 kB/s | 260 kB          00:00

(12/16): libgcc-11.5.0-5.el9_5.x86_64.rpm                                                                                                                                                                                                                                                                          319 kB/s |    84 kB          00:00

(13/16): gcc-11.5.0-5.el9_5.x86_64.rpm                                                                                                                                                                                                                                                                                  17 MB/s |    32 MB          00:01

(14/16): glibc-minimal-langpack-2.34-125.el9_5.8.x86_64.rpm                                                                                                                                                                                                                                        39 kB/s |    16 kB          00:00

(15/16): glibc-common-2.34-125.el9_5.8.x86_64.rpm                                                                                                                                                                                                                                                          712 kB/s | 290 kB          00:00

(16/16): glibc-2.34-125.el9_5.8.x86_64.rpm                                                                                                                                                                                                                                                                        5.1 MB/s | 1.9 MB          00:00

--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

Total                                                                                                                                                                                                                                                                                                                                                    17 MB/s |    50 MB          00:02

Running transaction check

Transaction check succeeded.

Running transaction test

Transaction test succeeded.

Running transaction

    Preparing                :                                                                                                                                                                                                                                                                                                                                                                            1/1

    Upgrading                : libgcc-11.5.0-5.el9_5.x86_64                                                                                                                                                                                                                                                                                                                1/21

    Running scriptlet: libgcc-11.5.0-5.el9_5.x86_64                                                                                                                                                                                                                                                                                                                1/21

    Upgrading                : glibc-minimal-langpack-2.34-125.el9_5.8.x86_64                                                                                                                                                                                                                                                                            2/21

    Upgrading                : glibc-common-2.34-125.el9_5.8.x86_64                                                                                                                                                                                                                                                                                                3/21

    Running scriptlet: glibc-2.34-125.el9_5.8.x86_64                                                                                                                                                                                                                                                                                                              4/21

    Upgrading                : glibc-2.34-125.el9_5.8.x86_64                                                                                                                                                                                                                                                                                                              4/21

    Running scriptlet: glibc-2.34-125.el9_5.8.x86_64                                                                                                                                                                                                                                                                                                              4/21

    Installing              : libmpc-1.2.1-4.el9.x86_64                                                                                                                                                                                                                                                                                                                      5/21

    Installing              : cpp-11.5.0-5.el9_5.x86_64                                                                                                                                                                                                                                                                                                                      6/21

    Installing              : libpkgconf-1.7.3-10.el9.x86_64                                                                                                                                                                                                                                                                                                            7/21

    Installing              : pkgconf-1.7.3-10.el9.x86_64                                                                                                                                                                                                                                                                                                                  8/21

    Installing              : glibc-headers-2.34-125.el9_5.8.x86_64                                                                                                                                                                                                                                                                                              9/21

    Upgrading                : libgomp-11.5.0-5.el9_5.x86_64                                                                                                                                                                                                                                                                                                            10/21

    Installing              : kernel-headers-5.14.0-503.40.1.el9_5.x86_64                                                                                                                                                                                                                                                                                11/21

    Installing              : pkgconf-m4-1.7.3-10.el9.noarch                                                                                                                                                                                                                                                                                                          12/21

    Installing              : pkgconf-pkg-config-1.7.3-10.el9.x86_64                                                                                                                                                                                                                                                                                          13/21

    Installing              : glibc-devel-2.34-125.el9_5.8.x86_64                                                                                                                                                                                                                                                                                                14/21

    Installing              : libxcrypt-devel-4.4.18-3.el9.x86_64                                                                                                                                                                                                                                                                                                15/21

    Installing              : gcc-11.5.0-5.el9_5.x86_64                                                                                                                                                                                                                                                                                                                    16/21

    Cleanup                    : libgomp-11.5.0-2.el9.x86_64                                                                                                                                                                                                                                                                                                                17/21

    Cleanup                    : glibc-common-2.34-125.el9_5.1.x86_64                                                                                                                                                                                                                                                                                              18/21

    Cleanup                    : glibc-minimal-langpack-2.34-125.el9_5.1.x86_64                                                                                                                                                                                                                                                                          19/21

    Cleanup                    : glibc-2.34-125.el9_5.1.x86_64                                                                                                                                                                                                                                                                                                            20/21

    Cleanup                    : libgcc-11.5.0-2.el9.x86_64                                                                                                                                                                                                                                                                                                                  21/21

    Running scriptlet: libgcc-11.5.0-2.el9.x86_64                                                                                                                                                                                                                                                                                                                  21/21

    Verifying                : pkgconf-pkg-config-1.7.3-10.el9.x86_64                                                                                                                                                                                                                                                                                            1/21

    Verifying                : pkgconf-m4-1.7.3-10.el9.noarch                                                                                                                                                                                                                                                                                                            2/21

    Verifying                : pkgconf-1.7.3-10.el9.x86_64                                                                                                                                                                                                                                                                                                                  3/21

    Verifying                : libpkgconf-1.7.3-10.el9.x86_64                                                                                                                                                                                                                                                                                                            4/21

    Verifying                : libmpc-1.2.1-4.el9.x86_64                                                                                                                                                                                                                                                                                                                      5/21

    Verifying                : libxcrypt-devel-4.4.18-3.el9.x86_64                                                                                                                                                                                                                                                                                                  6/21

    Verifying                : gcc-11.5.0-5.el9_5.x86_64                                                                                                                                                                                                                                                                                                                      7/21

    Verifying                : cpp-11.5.0-5.el9_5.x86_64                                                                                                                                                                                                                                                                                                                      8/21

    Verifying                : glibc-headers-2.34-125.el9_5.8.x86_64                                                                                                                                                                                                                                                                                              9/21

    Verifying                : glibc-devel-2.34-125.el9_5.8.x86_64                                                                                                                                                                                                                                                                                                10/21

    Verifying                : kernel-headers-5.14.0-503.40.1.el9_5.x86_64                                                                                                                                                                                                                                                                                11/21

    Verifying                : libgomp-11.5.0-5.el9_5.x86_64                                                                                                                                                                                                                                                                                                            12/21

    Verifying                : libgomp-11.5.0-2.el9.x86_64                                                                                                                                                                                                                                                                                                                13/21

    Verifying                : libgcc-11.5.0-5.el9_5.x86_64                                                                                                                                                                                                                                                                                                              14/21

    Verifying                : libgcc-11.5.0-2.el9.x86_64                                                                                                                                                                                                                                                                                                                  15/21

    Verifying                : glibc-minimal-langpack-2.34-125.el9_5.8.x86_64                                                                                                                                                                                                                                                                          16/21

    Verifying                : glibc-minimal-langpack-2.34-125.el9_5.1.x86_64                                                                                                                                                                                                                                                                          17/21

    Verifying                : glibc-common-2.34-125.el9_5.8.x86_64                                                                                                                                                                                                                                                                                              18/21

    Verifying                : glibc-common-2.34-125.el9_5.1.x86_64                                                                                                                                                                                                                                                                                              19/21

    Verifying                : glibc-2.34-125.el9_5.8.x86_64                                                                                                                                                                                                                                                                                                            20/21

    Verifying                : glibc-2.34-125.el9_5.1.x86_64                                                                                                                                                                                                                                                                                                            21/21

  

Upgraded:

    glibc-2.34-125.el9_5.8.x86_64              glibc-common-2.34-125.el9_5.8.x86_64              glibc-minimal-langpack-2.34-125.el9_5.8.x86_64              libgcc-11.5.0-5.el9_5.x86_64              libgomp-11.5.0-5.el9_5.x86_64

Installed:

    cpp-11.5.0-5.el9_5.x86_64                                  gcc-11.5.0-5.el9_5.x86_64                  glibc-devel-2.34-125.el9_5.8.x86_64        glibc-headers-2.34-125.el9_5.8.x86_64        kernel-headers-5.14.0-503.40.1.el9_5.x86_64

    libmpc-1.2.1-4.el9.x86_64                                  libpkgconf-1.7.3-10.el9.x86_64        libxcrypt-devel-4.4.18-3.el9.x86_64        pkgconf-1.7.3-10.el9.x86_64                            pkgconf-m4-1.7.3-10.el9.noarch

    pkgconf-pkg-config-1.7.3-10.el9.x86_64

  

Complete!

[root@rocky14 c_practice]# gcc a.c

**a.c:3:1:** warning: return type defaults to ‘**int**’ [-Wimplicit-int]

        3 | main()

            | ^~~~

[root@rocky14 c_practice]# gcc -o firstprogram a.c

**a.c:3:1:** warning: return type defaults to ‘**int**’ [-Wimplicit-int]

        3 | main()

            | ^~~~

[root@rocky14 c_practice]# ls -salh

total 44K

      0 drwxr-xr-x. 2 root root 100 May 22 11:34 .

      0 drwxr-xr-x. 5 root root 380 May 22 11:33 ..

4.0K -rw-r--r--. 1 root root    84 May 22 11:33 a.c

20K -rwxr-xr-x. 1 root root 18K May 22 11:34 a.out

20K -rwxr-xr-x. 1 root root 18K May 22 11:34 firstprogram

[root@rocky14 c_practice]# ./a.out

My first compiled program

[root@rocky14 c_practice]# ./firstprogram

My first compiled program

[root@rocky14 c_practice]# strace ./a.out

execve("./a.out", ["./a.out"], 0x7ffce9db9260 /* 32 vars */) = 0

brk(NULL)                                                              = 0x19af000

arch_prctl(0x3001 /* ARCH_??? */, 0x7fff48c39190) = -1 EINVAL (Invalid argument)

access("/etc/ld.so.preload", R_OK)            = -1 ENOENT (No such file or directory)

openat(AT_FDCWD, "/etc/ld.so.cache", O_RDONLY|O_CLOEXEC) = 3

fstat(3, {st_mode=S_IFREG|0644, st_size=16027, ...}) = 0

mmap(NULL, 16027, PROT_READ, MAP_PRIVATE, 3, 0) = 0x7f4bf1e0b000

close(3)                                                                = 0

openat(AT_FDCWD, "/lib64/libc.so.6", O_RDONLY|O_CLOEXEC) = 3

read(3, "\177ELF\2\1\1\3\0\0\0\0\0\0\0\0\3\0>\0\1\0\0\0\220\227\2\0\0\0\0\0"..., 832) = 832

pread64(3, "\6\0\0\0\4\0\0\0@\0\0\0\0\0\0\0@\0\0\0\0\0\0\0@\0\0\0\0\0\0\0"..., 784, 64) = 784

pread64(3, "\4\0\0\0 \0\0\0\5\0\0\0GNU\0\2\0\0\300\4\0\0\0\3\0\0\0\0\0\0\0"..., 48, 848) = 48

pread64(3, "\4\0\0\0\24\0\0\0\3\0\0\0GNU\0\374F\274A\223g\0=\16N9\234\276\"\252\336"..., 68, 896) = 68

fstat(3, {st_mode=S_IFREG|0755, st_size=2539928, ...}) = 0

mmap(NULL, 8192, PROT_READ|PROT_WRITE, MAP_PRIVATE|MAP_ANONYMOUS, -1, 0) = 0x7f4bf1e09000

pread64(3, "\6\0\0\0\4\0\0\0@\0\0\0\0\0\0\0@\0\0\0\0\0\0\0@\0\0\0\0\0\0\0"..., 784, 64) = 784

mmap(NULL, 2125744, PROT_READ, MAP_PRIVATE|MAP_DENYWRITE, 3, 0) = 0x7f4bf1c02000

mmap(0x7f4bf1c2a000, 1523712, PROT_READ|PROT_EXEC, MAP_PRIVATE|MAP_FIXED|MAP_DENYWRITE, 3, 0x28000) = 0x7f4bf1c2a000

mmap(0x7f4bf1d9e000, 360448, PROT_READ, MAP_PRIVATE|MAP_FIXED|MAP_DENYWRITE, 3, 0x19c000) = 0x7f4bf1d9e000

mmap(0x7f4bf1df6000, 24576, PROT_READ|PROT_WRITE, MAP_PRIVATE|MAP_FIXED|MAP_DENYWRITE, 3, 0x1f4000) = 0x7f4bf1df6000

mmap(0x7f4bf1dfc000, 53168, PROT_READ|PROT_WRITE, MAP_PRIVATE|MAP_FIXED|MAP_ANONYMOUS, -1, 0) = 0x7f4bf1dfc000

close(3)                                                                = 0

mmap(NULL, 8192, PROT_READ|PROT_WRITE, MAP_PRIVATE|MAP_ANONYMOUS, -1, 0) = 0x7f4bf1c00000

arch_prctl(ARCH_SET_FS, 0x7f4bf1e0a600) = 0

set_tid_address(0x7f4bf1e0a8d0)                  = 12822

set_robust_list(0x7f4bf1e0a8e0, 24)          = 0

rseq(0x7f4bf1e0afa0, 0x20, 0, 0x53053053) = 0

mprotect(0x7f4bf1df6000, 16384, PROT_READ) = 0

mprotect(0x403000, 4096, PROT_READ)          = 0

mprotect(0x7f4bf1e43000, 8192, PROT_READ) = 0

prlimit64(0, RLIMIT_STACK, NULL, {rlim_cur=8192*1024, rlim_max=RLIM64_INFINITY}) = 0

munmap(0x7f4bf1e0b000, 16027)                      = 0

fstat(1, {st_mode=S_IFCHR|0620, st_rdev=makedev(0x88, 0), ...}) = 0

getrandom("\x25\xd0\xd7\x2b\xd2\x12\xa9\xbd", 8, GRND_NONBLOCK) = 8

brk(NULL)                                                              = 0x19af000

brk(0x19d0000)                                                    = 0x19d0000

write(1, "My first compiled program \n", 27My first compiled program

) = 27

exit_group(0)                                                      = ?

+++ exited with 0 +++

[root@rocky14 c_practice]# strace ./firstprogram

execve("./firstprogram", ["./firstprogram"], 0x7fff21827de0 /* 32 vars */) = 0

brk(NULL)                                                              = 0x16dd000

arch_prctl(0x3001 /* ARCH_??? */, 0x7fffe4c60870) = -1 EINVAL (Invalid argument)

access("/etc/ld.so.preload", R_OK)            = -1 ENOENT (No such file or directory)

openat(AT_FDCWD, "/etc/ld.so.cache", O_RDONLY|O_CLOEXEC) = 3

fstat(3, {st_mode=S_IFREG|0644, st_size=16027, ...}) = 0

mmap(NULL, 16027, PROT_READ, MAP_PRIVATE, 3, 0) = 0x7f11d643a000

close(3)                                                                = 0

openat(AT_FDCWD, "/lib64/libc.so.6", O_RDONLY|O_CLOEXEC) = 3

read(3, "\177ELF\2\1\1\3\0\0\0\0\0\0\0\0\3\0>\0\1\0\0\0\220\227\2\0\0\0\0\0"..., 832) = 832

pread64(3, "\6\0\0\0\4\0\0\0@\0\0\0\0\0\0\0@\0\0\0\0\0\0\0@\0\0\0\0\0\0\0"..., 784, 64) = 784

pread64(3, "\4\0\0\0 \0\0\0\5\0\0\0GNU\0\2\0\0\300\4\0\0\0\3\0\0\0\0\0\0\0"..., 48, 848) = 48

pread64(3, "\4\0\0\0\24\0\0\0\3\0\0\0GNU\0\374F\274A\223g\0=\16N9\234\276\"\252\336"..., 68, 896) = 68

fstat(3, {st_mode=S_IFREG|0755, st_size=2539928, ...}) = 0

mmap(NULL, 8192, PROT_READ|PROT_WRITE, MAP_PRIVATE|MAP_ANONYMOUS, -1, 0) = 0x7f11d6438000

pread64(3, "\6\0\0\0\4\0\0\0@\0\0\0\0\0\0\0@\0\0\0\0\0\0\0@\0\0\0\0\0\0\0"..., 784, 64) = 784

mmap(NULL, 2125744, PROT_READ, MAP_PRIVATE|MAP_DENYWRITE, 3, 0) = 0x7f11d6231000

mmap(0x7f11d6259000, 1523712, PROT_READ|PROT_EXEC, MAP_PRIVATE|MAP_FIXED|MAP_DENYWRITE, 3, 0x28000) = 0x7f11d6259000

mmap(0x7f11d63cd000, 360448, PROT_READ, MAP_PRIVATE|MAP_FIXED|MAP_DENYWRITE, 3, 0x19c000) = 0x7f11d63cd000

mmap(0x7f11d6425000, 24576, PROT_READ|PROT_WRITE, MAP_PRIVATE|MAP_FIXED|MAP_DENYWRITE, 3, 0x1f4000) = 0x7f11d6425000

mmap(0x7f11d642b000, 53168, PROT_READ|PROT_WRITE, MAP_PRIVATE|MAP_FIXED|MAP_ANONYMOUS, -1, 0) = 0x7f11d642b000

close(3)                                                                = 0

mmap(NULL, 8192, PROT_READ|PROT_WRITE, MAP_PRIVATE|MAP_ANONYMOUS, -1, 0) = 0x7f11d622f000

arch_prctl(ARCH_SET_FS, 0x7f11d6439600) = 0

set_tid_address(0x7f11d64398d0)                  = 12826

set_robust_list(0x7f11d64398e0, 24)          = 0

rseq(0x7f11d6439fa0, 0x20, 0, 0x53053053) = 0

mprotect(0x7f11d6425000, 16384, PROT_READ) = 0

mprotect(0x403000, 4096, PROT_READ)          = 0

mprotect(0x7f11d6472000, 8192, PROT_READ) = 0

prlimit64(0, RLIMIT_STACK, NULL, {rlim_cur=8192*1024, rlim_max=RLIM64_INFINITY}) = 0

munmap(0x7f11d643a000, 16027)                      = 0

fstat(1, {st_mode=S_IFCHR|0620, st_rdev=makedev(0x88, 0), ...}) = 0

getrandom("\xe6\x02\x5b\x05\xc3\xaa\x8e\x43", 8, GRND_NONBLOCK) = 8

brk(NULL)                                                              = 0x16dd000

brk(0x16fe000)                                                    = 0x16fe000

write(1, "My first compiled program \n", 27My first compiled program

) = 27

exit_group(0)                                                      = ?

+++ exited with 0 +++
```
```bash
[root@rocky14 c_practice]# echo $name

  

[root@rocky14 c_practice]# uname

Linux

[root@rocky14 c_practice]# name=`uname`

[root@rocky14 c_practice]# echo $name

Linux

[root@rocky14 c_practice]# echo $kernel

  

[root@rocky14 c_practice]# uname -r

5.14.0-427.42.1.el9_4.x86_64

[root@rocky14 c_practice]# kernel=`uname -r`

[root@rocky14 c_practice]# echo $kernel

5.14.0-427.42.1.el9_4.x86_64

[root@rocky14 c_practice]# echo $PATH

/root/.local/bin:/root/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin

[root@rocky14 c_practice]# printenv | more

SHELL=/bin/bash

HISTCONTROL=ignoredups

HISTSIZE=1000

HOSTNAME=rocky14

PWD=/root/c_practice

LOGNAME=root

XDG_SESSION_TYPE=tty

MOTD_SHOWN=pam

HOME=/root

LANG=C.UTF-8

LS_COLORS=rs=0:di=01;34:ln=01;36:mh=00:pi=40;33:so=01;35:do=01;35:bd=40;33;01:cd=40;33;01:or=40;31;01:mi=01;37;41:su=37;41:sg=30;43:ca=30;41:tw=30;42:ow=34;42:st=37;44:ex=01;32:*.tar=01;31:*.tgz=01;31:*.arc

=01;31:*.arj=01;31:*.taz=01;31:*.lha=01;31:*.lz4=01;31:*.lzh=01;31:*.lzma=01;31:*.tlz=01;31:*.txz=01;31:*.tzo=01;31:*.t7z=01;31:*.zip=01;31:*.z=01;31:*.dz=01;31:*.gz=01;31:*.lrz=01;31:*.lz=01;31:*.lzo=01;31

:*.xz=01;31:*.zst=01;31:*.tzst=01;31:*.bz2=01;31:*.bz=01;31:*.tbz=01;31:*.tbz2=01;31:*.tz=01;31:*.deb=01;31:*.rpm=01;31:*.jar=01;31:*.war=01;31:*.ear=01;31:*.sar=01;31:*.rar=01;31:*.alz=01;31:*.ace=01;31:*.

zoo=01;31:*.cpio=01;31:*.7z=01;31:*.rz=01;31:*.cab=01;31:*.wim=01;31:*.swm=01;31:*.dwm=01;31:*.esd=01;31:*.jpg=01;35:*.jpeg=01;35:*.mjpg=01;35:*.mjpeg=01;35:*.gif=01;35:*.bmp=01;35:*.pbm=01;35:*.pgm=01;35:*

.ppm=01;35:*.tga=01;35:*.xbm=01;35:*.xpm=01;35:*.tif=01;35:*.tiff=01;35:*.png=01;35:*.svg=01;35:*.svgz=01;35:*.mng=01;35:*.pcx=01;35:*.mov=01;35:*.mpg=01;35:*.mpeg=01;35:*.m2v=01;35:*.mkv=01;35:*.webm=01;35

:*.webp=01;35:*.ogm=01;35:*.mp4=01;35:*.m4v=01;35:*.mp4v=01;35:*.vob=01;35:*.qt=01;35:*.nuv=01;35:*.wmv=01;35:*.asf=01;35:*.rm=01;35:*.rmvb=01;35:*.flc=01;35:*.avi=01;35:*.fli=01;35:*.flv=01;35:*.gl=01;35:*

.dl=01;35:*.xcf=01;35:*.xwd=01;35:*.yuv=01;35:*.cgm=01;35:*.emf=01;35:*.ogv=01;35:*.ogx=01;35:*.aac=01;36:*.au=01;36:*.flac=01;36:*.m4a=01;36:*.mid=01;36:*.midi=01;36:*.mka=01;36:*.mp3=01;36:*.mpc=01;36:*.o

gg=01;36:*.ra=01;36:*.wav=01;36:*.oga=01;36:*.opus=01;36:*.spx=01;36:*.xspf=01;36:

SSH_CONNECTION=192.168.11.245 56504 192.168.200.64 22

XDG_SESSION_CLASS=user

SELINUX_ROLE_REQUESTED=

TERM=xterm

LESSOPEN=||/usr/bin/lesspipe.sh %s

USER=root

SELINUX_USE_CURRENT_RANGE=

SHLVL=1

XDG_SESSION_ID=7

XDG_RUNTIME_DIR=/run/user/0

S_COLORS=auto

SSH_CLIENT=192.168.11.245 56504 22

which_declare=declare -f

PATH=/root/.local/bin:/root/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin

SELINUX_LEVEL_REQUESTED=

DBUS_SESSION_BUS_ADDRESS=unix:path=/run/user/0/bus

MAIL=/var/spool/mail/root

SSH_TTY=/dev/pts/0

BASH_FUNC_which%%=() {    ( alias;

eval ${which_declare} ) | /usr/bin/which --tty-only --read-alias --read-functions --show-tilde --show-dot $@

}

_=/usr/bin/printenv

OLDPWD=/root

[root@rocky14 c_practice]# cat /proc/cpuinfo

processor              : 0

vendor_id              : GenuineIntel

cpu family            : 6

model                      : 45

model name            : Intel(R) Xeon(R) CPU E5-2665 0 @ 2.40GHz

stepping                : 7

microcode              : 0x71a

cpu MHz                  : 2400.018

cache size            : 20480 KB

physical id          : 0

siblings                : 1

core id                  : 0

cpu cores              : 1

apicid                    : 0

initial apicid    : 0

fpu                          : yes

fpu_exception      : yes

cpuid level          : 13

wp                            : yes

flags                      : fpu vme de pse tsc msr pae mce cx8 apic sep mtrr pge mca cmov pat pse36 clflush acpi mmx fxsr sse sse2 ss ht syscall nx pdpe1gb rdtscp lm constant_tsc rep_good nopl cpuid tsc_known_freq pni pclmulqdq ssse3 cx16 pcid sse4_1 sse4_2 x2apic popcnt tsc_deadline_timer aes xsave avx hypervisor lahf_lm cpuid_fault pti ssbd ibrs ibpb stibp xsaveopt md_clear flush_l1d

bugs                        : cpu_meltdown spectre_v1 spectre_v2 spec_store_bypass l1tf mds swapgs itlb_multihit mmio_unknown bhi

bogomips                : 4800.03

clflush size        : 64

cache_alignment : 64

address sizes      : 46 bits physical, 48 bits virtual

power management:

  

processor              : 1

vendor_id              : GenuineIntel

cpu family            : 6

model                      : 45

model name            : Intel(R) Xeon(R) CPU E5-2665 0 @ 2.40GHz

stepping                : 7

microcode              : 0x71a

cpu MHz                  : 2400.018

cache size            : 20480 KB

physical id          : 1

siblings                : 1

core id                  : 0

cpu cores              : 1

apicid                    : 2

initial apicid    : 2

fpu                          : yes

fpu_exception      : yes

cpuid level          : 13

wp                            : yes

flags                      : fpu vme de pse tsc msr pae mce cx8 apic sep mtrr pge mca cmov pat pse36 clflush acpi mmx fxsr sse sse2 ss ht syscall nx pdpe1gb rdtscp lm constant_tsc rep_good nopl cpuid tsc_known_freq pni pclmulqdq ssse3 cx16 pcid sse4_1 sse4_2 x2apic popcnt tsc_deadline_timer aes xsave avx hypervisor lahf_lm cpuid_fault pti ssbd ibrs ibpb stibp xsaveopt md_clear flush_l1d

bugs                        : cpu_meltdown spectre_v1 spectre_v2 spec_store_bypass l1tf mds swapgs itlb_multihit mmio_unknown bhi

bogomips                : 4800.03

clflush size        : 64

cache_alignment : 64

address sizes      : 46 bits physical, 48 bits virtual

power management:

  

[root@rocky14 c_practice]# cat /proc/cpuinfo | grep -i proc

processor              : 0

processor              : 1

[root@rocky14 c_practice]# cat /proc/cpuinfo | grep -i proc | wc -l

2

[root@rocky14 c_practice]# numProc=`cat /proc/cpuinfo | grep -i proc | wc -l`

[root@rocky14 c_practice]# echo $numProc

2

[root@rocky14 c_practice]# free -m

                              total                used                free            shared    buff/cache      available

Mem:                        3892                2629                1346                2163                2224                1262

Swap:                            0                      0                      0

[root@rocky14 c_practice]# free -mh

                              total                used                free            shared    buff/cache      available

Mem:                      3.8Gi              2.6Gi              1.3Gi              2.1Gi              2.2Gi              1.2Gi

Swap:                          0B                    0B                    0B

[root@rocky14 c_practice]# free -h

                              total                used                free            shared    buff/cache      available

Mem:                      3.8Gi              2.6Gi              1.3Gi              2.1Gi              2.2Gi              1.2Gi

Swap:                          0B                    0B                    0B

[root@rocky14 c_practice]# free -m | grep -i mem

Mem:                        3892                2629                1346                2163                2224                1262

[root@rocky14 c_practice]# free -m | grep -i mem | awk '{print $2}'

3892

[root@rocky14 c_practice]# memSize=`free -m | grep -i mem | awk '{print $2}'`

[root@rocky14 c_practice]# echo $memSize

3892
```
```bash
[root@rocky14 c_practice]# ps -ef | grep -i httpd | grep -v grep

[root@rocky14 c_practice]# echo $?

1

[root@rocky14 c_practice]# ps -ef | grep -i httpd

root              12870      12412    0 11:56 pts/0        00:00:00 grep --color=auto -i httpd

[root@rocky14 c_practice]# echo $?

0

[root@rocky14 c_practice]# rpm -qa | grep -i superprogram

[root@rocky14 c_practice]# echo $?

1

[root@rocky14 c_practice]# rpm -qa | grep -i gcc

libgcc-11.5.0-5.el9_5.x86_64

gcc-11.5.0-5.el9_5.x86_64

[root@rocky14 c_practice]# echo $?

0

[root@rocky14 c_practice]# rpm -qa | grep -i superprogram

[root@rocky14 c_practice]# superCheck=$?

[root@rocky14 c_practice]# rpm -qa | grep -i gcc

libgcc-11.5.0-5.el9_5.x86_64

gcc-11.5.0-5.el9_5.x86_64

[root@rocky14 c_practice]# gccCheck=$?

[root@rocky14 c_practice]# echo $superCheck

1

[root@rocky14 c_practice]# echo $gccCheck

0
```
```bash
[root@rocky14 c_practice]# if [ $superCheck -eq "0" ]; then echo "super exists"; fi

[root@rocky14 c_practice]# if [ $gccCheck -eq "0" ]; then echo "gcc exists"; fi

gcc exists

[root@rocky14 c_practice]# if [ $superCheck -eq "0" ]; then echo "super exists"; else echo "super does not exist"; fi

super does not exist

[root@rocky14 c_practice]# if [ $gccCheck -eq "0" ]; then echo "gcc exists"; else echo "gcc does not exist"; fi

gcc exists

[root@rocky14 c_practice]# superCheck=4 if [ $superCheck -eq "0" ]; then echo "super exists"; elif [ $superCheck -gt "1" ]; then echo "something is really wrong"; else echo "super does not exist"; fi

-bash: syntax error near unexpected token `then'

[root@rocky14 c_practice]# superCheck=4 if [ $superCheck -eq "0" ]; then echo "super exists"; elif [ $superCheck -gt "1" ]; then echo "something is really wrong"; else echo "super does not exist"; fi

-bash: syntax error near unexpected token `then'

[root@rocky14 c_practice]# superCheck=4 if [ $superCheck -eq "0" ]; then echo "super exists"; elif [ $superCheck -gt "1" ]; echo "something is really wrong"; else echo "super does not exist"; fi

-bash: syntax error near unexpected token `then'

[root@rocky14 c_practice]# superCheck=4; if [ $superCheck -eq "0" ]; then echo "super exists"; elif [ $superCheck -gt "1" ]; then echo "something is really wrong"; else echo "super does not exist"; fi

something is really wrong

[root@rocky14 c_practice]# gccCheck=5; if [ $gccCheck -eq "0" ]; then echo "gcc exists"; elif [ $gccCheck -gt "1" ]; then echo "something is really wrong"; else echo "gcc does not exist"; fi

something is really wrong

[root@rocky14 c_practice]# gccCheck=1; if [ $gccCheck -eq "0" ]; then echo "gcc exists"; elif [ $gccCheck -gt "1" ]; then echo "something is really wrong"; else echo "gcc does not exist"; fi

gcc does not exist

[root@rocky14 c_practice]# gccCheck=0; if [ $gccCheck -eq "0" ]; then echo "gcc exists"; elif [ $gccCheck -gt "1" ]; then echo "something is really wrong"; else echo "gcc does not exist"; fi

gcc exists

[root@rocky14 c_practice]# if [ $gccCheck -eq "0" -a $superCheck -eq "1" ]; then echo "We can install someprogram"; else echo "We can't install someprogram"; fi

We can't install someprogram

[root@rocky14 c_practice]# if [ $gccCheck -eq "0" -o $superCheck -eq "1" ]; then echo "We can install someprogram"; else echo "We can't install someprogram"; fi

We can install someprogram

[root@rocky14 c_practice]# superCheck=1

[root@rocky14 c_practice]# if [ $gccCheck -eq "0" -a $superCheck -eq "1" ]; then echo "We can install someprogram"; else echo "We can't install someprogram"; fi

We can install someprogram

[root@rocky14 c_practice]# if [ $gccCheck -eq "0" -o $superCheck -eq "1" ]; then echo "We can install someprogram"; else echo "We can't install someprogram"; fi

We can install someprogram
```
```bash
[root@rocky14 c_practice]# for i in 1 2 3 4 5; do echo "the value now is $i"; done

the value now is 1

the value now is 2

the value now is 3

the value now is 4

the value now is 5

[root@rocky14 c_practice]# for dessert in pie cake icecream sugar soda; do echo "this is my favorite $dessert"; done

this is my favorite pie

this is my favorite cake

this is my favorite icecream

this is my favorite sugar

this is my favorite soda

[root@rocky14 c_practice]# seq 100

1

2

3

4

5

6

7

8

9

10

11

12

13

14

15

16

17

18

19

20

21

22

23

24

25

26

27

28

29

30

31

32

33

34

35

36

37

38

39

40

41

42

43

44

45

46

47

48

49

50

51

52

53

54

55

56

57

58

59

60

61

62

63

64

65

66

67

68

69

70

71

72

73

74

75

76

77

78

79

80

81

82

83

84

85

86

87

88

89

90

91

92

93

94

95

96

97

98

99

100

[root@rocky14 c_practice]# seq 4 100

4

5

6

7

8

9

10

11

12

13

14

15

16

17

18

19

20

21

22

23

24

25

26

27

28

29

30

31

32

33

34

35

36

37

38

39

40

41

42

43

44

45

46

47

48

49

50

51

52

53

54

55

56

57

58

59

60

61

62

63

64

65

66

67

68

69

70

71

72

73

74

75

76

77

78

79

80

81

82

83

84

85

86

87

88

89

90

91

92

93

94

95

96

97

98

99

100

[root@rocky14 c_practice]# seq 6 2 100

6

8

10

12

14

16

18

20

22

24

26

28

30

32

34

36

38

40

42

44

46

48

50

52

54

56

58

60

62

64

66

68

70

72

74

76

78

80

82

84

86

88

90

92

94

96

98

100

[root@rocky14 c_practice]# counter=0 while [[ $counter -lt 100 ]]; do echo "counter is at $counter"; (( counter++ )); done

-bash: syntax error near unexpected token `do'

[root@rocky14 c_practice]# counter=0; while [[ $counter -lt 100 ]]; do echo "counter is at $counter"; (( counter++ )); done

counter is at 0

counter is at 1

counter is at 2

counter is at 3

counter is at 4

counter is at 5

counter is at 6

counter is at 7

counter is at 8

counter is at 9

counter is at 10

counter is at 11

counter is at 12

counter is at 13

counter is at 14

counter is at 15

counter is at 16

counter is at 17

counter is at 18

counter is at 19

counter is at 20

counter is at 21

counter is at 22

counter is at 23

counter is at 24

counter is at 25

counter is at 26

counter is at 27

counter is at 28

counter is at 29

counter is at 30

counter is at 31

counter is at 32

counter is at 33

counter is at 34

counter is at 35

counter is at 36

counter is at 37

counter is at 38

counter is at 39

counter is at 40

counter is at 41

counter is at 42

counter is at 43

counter is at 44

counter is at 45

counter is at 46

counter is at 47

counter is at 48

counter is at 49

counter is at 50

counter is at 51

counter is at 52

counter is at 53

counter is at 54

counter is at 55

counter is at 56

counter is at 57

counter is at 58

counter is at 59

counter is at 60

counter is at 61

counter is at 62

counter is at 63

counter is at 64

counter is at 65

counter is at 66

counter is at 67

counter is at 68

counter is at 69

counter is at 70

counter is at 71

counter is at 72

counter is at 73

counter is at 74

counter is at 75

counter is at 76

counter is at 77

counter is at 78

counter is at 79

counter is at 80

counter is at 81

counter is at 82

counter is at 83

counter is at 84

counter is at 85

counter is at 86

counter is at 87

counter is at 88

counter is at 89

counter is at 90

counter is at 91

counter is at 92

counter is at 93

counter is at 94

counter is at 95

counter is at 96

counter is at 97

counter is at 98

counter is at 99

[root@rocky14 c_practice]# while [[ $counter -lt 100 ]]; do echo "counter is at $counter"; (( counter++ )); done

[root@rocky14 c_practice]# counter=0; while [[ $counter -lt 100 ]]; do echo "counter is at $counter"; (( counter++ )); done

counter is at 0

counter is at 1

counter is at 2

counter is at 3

counter is at 4

counter is at 5

counter is at 6

counter is at 7

counter is at 8

counter is at 9

counter is at 10

counter is at 11

counter is at 12

counter is at 13

counter is at 14

counter is at 15

counter is at 16

counter is at 17

counter is at 18

counter is at 19

counter is at 20

counter is at 21

counter is at 22

counter is at 23

counter is at 24

counter is at 25

counter is at 26

counter is at 27

counter is at 28

counter is at 29

counter is at 30

counter is at 31

counter is at 32

counter is at 33

counter is at 34

counter is at 35

counter is at 36

counter is at 37

counter is at 38

counter is at 39

counter is at 40

counter is at 41

counter is at 42

counter is at 43

counter is at 44

counter is at 45

counter is at 46

counter is at 47

counter is at 48

counter is at 49

counter is at 50

counter is at 51

counter is at 52

counter is at 53

counter is at 54

counter is at 55

counter is at 56

counter is at 57

counter is at 58

counter is at 59

counter is at 60

counter is at 61

counter is at 62

counter is at 63

counter is at 64

counter is at 65

counter is at 66

counter is at 67

counter is at 68

counter is at 69

counter is at 70

counter is at 71

counter is at 72

counter is at 73

counter is at 74

counter is at 75

counter is at 76

counter is at 77

counter is at 78

counter is at 79

counter is at 80

counter is at 81

counter is at 82

counter is at 83

counter is at 84

counter is at 85

counter is at 86

counter is at 87

counter is at 88

counter is at 89

counter is at 90

counter is at 91

counter is at 92

counter is at 93

counter is at 94

counter is at 95

counter is at 96

counter is at 97

counter is at 98

counter is at 99

[root@rocky14 c_practice]# counter=3; while [[ $counter -lt 252 ]]; do echo "counter is at $counter"; (( counter++ )); done

counter is at 3

counter is at 4

counter is at 5

counter is at 6

counter is at 7

counter is at 8

counter is at 9

counter is at 10

counter is at 11

counter is at 12

counter is at 13

counter is at 14

counter is at 15

counter is at 16

counter is at 17

counter is at 18

counter is at 19

counter is at 20

counter is at 21

counter is at 22

counter is at 23

counter is at 24

counter is at 25

counter is at 26

counter is at 27

counter is at 28

counter is at 29

counter is at 30

counter is at 31

counter is at 32

counter is at 33

counter is at 34

counter is at 35

counter is at 36

counter is at 37

counter is at 38

counter is at 39

counter is at 40

counter is at 41

counter is at 42

counter is at 43

counter is at 44

counter is at 45

counter is at 46

counter is at 47

counter is at 48

counter is at 49

counter is at 50

counter is at 51

counter is at 52

counter is at 53

counter is at 54

counter is at 55

counter is at 56

counter is at 57

counter is at 58

counter is at 59

counter is at 60

counter is at 61

counter is at 62

counter is at 63

counter is at 64

counter is at 65

counter is at 66

counter is at 67

counter is at 68

counter is at 69

counter is at 70

counter is at 71

counter is at 72

counter is at 73

counter is at 74

counter is at 75

counter is at 76

counter is at 77

counter is at 78

counter is at 79

counter is at 80

counter is at 81

counter is at 82

counter is at 83

counter is at 84

counter is at 85

counter is at 86

counter is at 87

counter is at 88

counter is at 89

counter is at 90

counter is at 91

counter is at 92

counter is at 93

counter is at 94

counter is at 95

counter is at 96

counter is at 97

counter is at 98

counter is at 99

counter is at 100

counter is at 101

counter is at 102

counter is at 103

counter is at 104

counter is at 105

counter is at 106

counter is at 107

counter is at 108

counter is at 109

counter is at 110

counter is at 111

counter is at 112

counter is at 113

counter is at 114

counter is at 115

counter is at 116

counter is at 117

counter is at 118

counter is at 119

counter is at 120

counter is at 121

counter is at 122

counter is at 123

counter is at 124

counter is at 125

counter is at 126

counter is at 127

counter is at 128

counter is at 129

counter is at 130

counter is at 131

counter is at 132

counter is at 133

counter is at 134

counter is at 135

counter is at 136

counter is at 137

counter is at 138

counter is at 139

counter is at 140

counter is at 141

counter is at 142

counter is at 143

counter is at 144

counter is at 145

counter is at 146

counter is at 147

counter is at 148

counter is at 149

counter is at 150

counter is at 151

counter is at 152

counter is at 153

counter is at 154

counter is at 155

counter is at 156

counter is at 157

counter is at 158

counter is at 159

counter is at 160

counter is at 161

counter is at 162

counter is at 163

counter is at 164

counter is at 165

counter is at 166

counter is at 167

counter is at 168

counter is at 169

counter is at 170

counter is at 171

counter is at 172

counter is at 173

counter is at 174

counter is at 175

counter is at 176

counter is at 177

counter is at 178

counter is at 179

counter is at 180

counter is at 181

counter is at 182

counter is at 183

counter is at 184

counter is at 185

counter is at 186

counter is at 187

counter is at 188

counter is at 189

counter is at 190

counter is at 191

counter is at 192

counter is at 193

counter is at 194

counter is at 195

counter is at 196

counter is at 197

counter is at 198

counter is at 199

counter is at 200

counter is at 201

counter is at 202

counter is at 203

counter is at 204

counter is at 205

counter is at 206

counter is at 207

counter is at 208

counter is at 209

counter is at 210

counter is at 211

counter is at 212

counter is at 213

counter is at 214

counter is at 215

counter is at 216

counter is at 217

counter is at 218

counter is at 219

counter is at 220

counter is at 221

counter is at 222

counter is at 223

counter is at 224

counter is at 225

counter is at 226

counter is at 227

counter is at 228

counter is at 229

counter is at 230

counter is at 231

counter is at 232

counter is at 233

counter is at 234

counter is at 235

counter is at 236

counter is at 237

counter is at 238

counter is at 239

counter is at 240

counter is at 241

counter is at 242

counter is at 243

counter is at 244

counter is at 245

counter is at 246

counter is at 247

counter is at 248

counter is at 249

counter is at 250

counter is at 251

[root@rocky14 c_practice]# memFree=free -m | grep -i mem | awk '{print $2}'

-bash: -m: command not found

[root@rocky14 c_practice]# memFree=`free -m | grep -i mem | awk '{print $2}'`

[root@rocky14 c_practice]# counter=0

[root@rocky14 c_practice]# while [[ $counter -lt $memFree ]]; do echo "counter is at $counter"; (( counter++ )); done

counter is at 0

counter is at 1

counter is at 2

counter is at 3

counter is at 4

counter is at 5

counter is at 6

counter is at 7

counter is at 8

counter is at 9

counter is at 10

counter is at 11

counter is at 12

counter is at 13

counter is at 14

counter is at 15

counter is at 16

counter is at 17

counter is at 18

counter is at 19

counter is at 20

counter is at 21

counter is at 22

counter is at 23

counter is at 24

counter is at 25

counter is at 26

counter is at 27

counter is at 28

counter is at 29

counter is at 30

counter is at 31

counter is at 32

counter is at 33

counter is at 34

counter is at 35

counter is at 36

counter is at 37

counter is at 38

counter is at 39

counter is at 40

counter is at 41

counter is at 42

counter is at 43

counter is at 44

counter is at 45

counter is at 46

counter is at 47

counter is at 48

counter is at 49

counter is at 50

counter is at 51

counter is at 52

counter is at 53

counter is at 54

counter is at 55

counter is at 56

counter is at 57

counter is at 58

counter is at 59

counter is at 60

counter is at 61

counter is at 62

counter is at 63

counter is at 64

counter is at 65

counter is at 66

counter is at 67

counter is at 68

counter is at 69

counter is at 70

counter is at 71

counter is at 72

counter is at 73

counter is at 74

counter is at 75

counter is at 76

counter is at 77

counter is at 78

counter is at 79

counter is at 80

counter is at 81

counter is at 82

counter is at 83

counter is at 84

counter is at 85

counter is at 86

counter is at 87

counter is at 88

counter is at 89

counter is at 90

counter is at 91

counter is at 92

counter is at 93

counter is at 94

counter is at 95

counter is at 96

counter is at 97

counter is at 98

counter is at 99

counter is at 100

counter is at 101

counter is at 102

counter is at 103

counter is at 104

counter is at 105

counter is at 106

counter is at 107

counter is at 108

counter is at 109

counter is at 110

counter is at 111

counter is at 112

counter is at 113

counter is at 114

counter is at 115

counter is at 116

counter is at 117

counter is at 118

counter is at 119

counter is at 120

counter is at 121

counter is at 122

counter is at 123

counter is at 124

counter is at 125

counter is at 126

counter is at 127

counter is at 128

counter is at 129

counter is at 130

counter is at 131

counter is at 132

counter is at 133

counter is at 134

counter is at 135

counter is at 136

counter is at 137

counter is at 138

counter is at 139

counter is at 140

counter is at 141

counter is at 142

counter is at 143

counter is at 144

counter is at 145

counter is at 146

counter is at 147

counter is at 148

counter is at 149

counter is at 150

counter is at 151

counter is at 152

counter is at 153

counter is at 154

counter is at 155

counter is at 156

counter is at 157

counter is at 158

counter is at 159

counter is at 160

counter is at 161

counter is at 162

counter is at 163

counter is at 164

counter is at 165

counter is at 166

counter is at 167

counter is at 168

counter is at 169

counter is at 170

counter is at 171

counter is at 172

counter is at 173

counter is at 174

counter is at 175

counter is at 176

counter is at 177

counter is at 178

counter is at 179

counter is at 180

counter is at 181

counter is at 182

counter is at 183

counter is at 184

counter is at 185

counter is at 186

counter is at 187

counter is at 188

counter is at 189

counter is at 190

counter is at 191

counter is at 192

counter is at 193

counter is at 194

counter is at 195

counter is at 196

counter is at 197

counter is at 198

counter is at 199

counter is at 200

counter is at 201

counter is at 202

counter is at 203

counter is at 204

counter is at 205

counter is at 206

counter is at 207

counter is at 208

counter is at 209

counter is at 210

counter is at 211

counter is at 212

counter is at 213

counter is at 214

counter is at 215

counter is at 216

counter is at 217

counter is at 218

counter is at 219

counter is at 220

counter is at 221

counter is at 222

counter is at 223

counter is at 224

counter is at 225

counter is at 226

counter is at 227

counter is at 228

counter is at 229

counter is at 230

counter is at 231

counter is at 232

counter is at 233

counter is at 234

counter is at 235

counter is at 236

counter is at 237

counter is at 238

counter is at 239

counter is at 240

counter is at 241

counter is at 242

counter is at 243

counter is at 244

counter is at 245

counter is at 246

counter is at 247

counter is at 248

counter is at 249

counter is at 250

counter is at 251

counter is at 252

counter is at 253

counter is at 254

counter is at 255

counter is at 256

counter is at 257

counter is at 258

counter is at 259

counter is at 260

counter is at 261

counter is at 262

counter is at 263

counter is at 264

counter is at 265

counter is at 266

counter is at 267

counter is at 268

counter is at 269

counter is at 270

counter is at 271

counter is at 272

counter is at 273

counter is at 274

counter is at 275

counter is at 276

counter is at 277

counter is at 278

counter is at 279

counter is at 280

counter is at 281

counter is at 282

counter is at 283

counter is at 284

counter is at 285

counter is at 286

counter is at 287

counter is at 288

counter is at 289

counter is at 290

counter is at 291

counter is at 292

counter is at 293

counter is at 294

counter is at 295

counter is at 296

counter is at 297

counter is at 298

counter is at 299

counter is at 300

counter is at 301

counter is at 302

counter is at 303

counter is at 304

counter is at 305

counter is at 306

counter is at 307

counter is at 308

counter is at 309

counter is at 310

counter is at 311

counter is at 312

counter is at 313

counter is at 314

counter is at 315

counter is at 316

counter is at 317

counter is at 318

counter is at 319

counter is at 320

counter is at 321

counter is at 322

counter is at 323

counter is at 324

counter is at 325

counter is at 326

counter is at 327

counter is at 328

counter is at 329

counter is at 330

counter is at 331

counter is at 332

counter is at 333

counter is at 334

counter is at 335

counter is at 336

counter is at 337

counter is at 338

counter is at 339

counter is at 340

counter is at 341

counter is at 342

counter is at 343

counter is at 344

counter is at 345

counter is at 346

counter is at 347

counter is at 348

counter is at 349

counter is at 350

counter is at 351

counter is at 352

counter is at 353

counter is at 354

counter is at 355

counter is at 356

counter is at 357

counter is at 358

counter is at 359

counter is at 360

counter is at 361

counter is at 362

counter is at 363

counter is at 364

counter is at 365

counter is at 366

counter is at 367

counter is at 368

counter is at 369

counter is at 370

counter is at 371

counter is at 372

counter is at 373

counter is at 374

counter is at 375

counter is at 376

counter is at 377

counter is at 378

counter is at 379

counter is at 380

counter is at 381

counter is at 382

counter is at 383

counter is at 384

counter is at 385

counter is at 386

counter is at 387

counter is at 388

counter is at 389

counter is at 390

counter is at 391

counter is at 392

counter is at 393

counter is at 394

counter is at 395

counter is at 396

counter is at 397

counter is at 398

counter is at 399

counter is at 400

counter is at 401

counter is at 402

counter is at 403

counter is at 404

counter is at 405

counter is at 406

counter is at 407

counter is at 408

counter is at 409

counter is at 410

counter is at 411

counter is at 412

counter is at 413

counter is at 414

counter is at 415

counter is at 416

counter is at 417

counter is at 418

counter is at 419

counter is at 420

counter is at 421

counter is at 422

counter is at 423

counter is at 424

counter is at 425

counter is at 426

counter is at 427

counter is at 428

counter is at 429

counter is at 430

counter is at 431

counter is at 432

counter is at 433

counter is at 434

counter is at 435

counter is at 436

counter is at 437

counter is at 438

counter is at 439

counter is at 440

counter is at 441

counter is at 442

counter is at 443

counter is at 444

counter is at 445

counter is at 446

counter is at 447

counter is at 448

counter is at 449

counter is at 450

counter is at 451

counter is at 452

counter is at 453

counter is at 454

counter is at 455

counter is at 456

counter is at 457

counter is at 458

counter is at 459

counter is at 460

counter is at 461

counter is at 462

counter is at 463

counter is at 464

counter is at 465

counter is at 466

counter is at 467

counter is at 468

counter is at 469

counter is at 470

counter is at 471

counter is at 472

counter is at 473

counter is at 474

counter is at 475

counter is at 476

counter is at 477

counter is at 478

counter is at 479

counter is at 480

counter is at 481

counter is at 482

counter is at 483

counter is at 484

counter is at 485

counter is at 486

counter is at 487

counter is at 488

counter is at 489

counter is at 490

counter is at 491

counter is at 492

counter is at 493

counter is at 494

counter is at 495

counter is at 496

counter is at 497

counter is at 498

counter is at 499

counter is at 500

counter is at 501

counter is at 502

counter is at 503

counter is at 504

counter is at 505

counter is at 506

counter is at 507

counter is at 508

counter is at 509

counter is at 510

counter is at 511

counter is at 512

counter is at 513

counter is at 514

counter is at 515

counter is at 516

counter is at 517

counter is at 518

counter is at 519

counter is at 520

counter is at 521

counter is at 522

counter is at 523

counter is at 524

counter is at 525

counter is at 526

counter is at 527

counter is at 528

counter is at 529

counter is at 530

counter is at 531

counter is at 532

counter is at 533

counter is at 534

counter is at 535

counter is at 536

counter is at 537

counter is at 538

counter is at 539

counter is at 540

counter is at 541

counter is at 542

counter is at 543

counter is at 544

counter is at 545

counter is at 546

counter is at 547

counter is at 548

counter is at 549

counter is at 550

counter is at 551

counter is at 552

counter is at 553

counter is at 554

counter is at 555

counter is at 556

counter is at 557

counter is at 558

counter is at 559

counter is at 560

counter is at 561

counter is at 562

counter is at 563

counter is at 564

counter is at 565

counter is at 566

counter is at 567

counter is at 568

counter is at 569

counter is at 570

counter is at 571

counter is at 572

counter is at 573

counter is at 574

counter is at 575

counter is at 576

counter is at 577

counter is at 578

counter is at 579

counter is at 580

counter is at 581

counter is at 582

counter is at 583

counter is at 584

counter is at 585

counter is at 586

counter is at 587

counter is at 588

counter is at 589

counter is at 590

counter is at 591

counter is at 592

counter is at 593

counter is at 594

counter is at 595

counter is at 596

counter is at 597

counter is at 598

counter is at 599

counter is at 600

counter is at 601

counter is at 602

counter is at 603

counter is at 604

counter is at 605

counter is at 606

counter is at 607

counter is at 608

counter is at 609

counter is at 610

counter is at 611

counter is at 612

counter is at 613

counter is at 614

counter is at 615

counter is at 616

counter is at 617

counter is at 618

counter is at 619

counter is at 620

counter is at 621

counter is at 622

counter is at 623

counter is at 624

counter is at 625

counter is at 626

counter is at 627

counter is at 628

counter is at 629

counter is at 630

counter is at 631

counter is at 632

counter is at 633

counter is at 634

counter is at 635

counter is at 636

counter is at 637

counter is at 638

counter is at 639

counter is at 640

counter is at 641

counter is at 642

counter is at 643

counter is at 644

counter is at 645

counter is at 646

counter is at 647

counter is at 648

counter is at 649

counter is at 650

counter is at 651

counter is at 652

counter is at 653

counter is at 654

counter is at 655

counter is at 656

counter is at 657

counter is at 658

counter is at 659

counter is at 660

counter is at 661

counter is at 662

counter is at 663

counter is at 664

counter is at 665

counter is at 666

counter is at 667

counter is at 668

counter is at 669

counter is at 670

counter is at 671

counter is at 672

counter is at 673

counter is at 674

counter is at 675

counter is at 676

counter is at 677

counter is at 678

counter is at 679

counter is at 680

counter is at 681

counter is at 682

counter is at 683

counter is at 684

counter is at 685

counter is at 686

counter is at 687

counter is at 688

counter is at 689

counter is at 690

counter is at 691

counter is at 692

counter is at 693

counter is at 694

counter is at 695

counter is at 696

counter is at 697

counter is at 698

counter is at 699

counter is at 700

counter is at 701

counter is at 702

counter is at 703

counter is at 704

counter is at 705

counter is at 706

counter is at 707

counter is at 708

counter is at 709

counter is at 710

counter is at 711

counter is at 712

counter is at 713

counter is at 714

counter is at 715

counter is at 716

counter is at 717

counter is at 718

counter is at 719

counter is at 720

counter is at 721

counter is at 722

counter is at 723

counter is at 724

counter is at 725

counter is at 726

counter is at 727

counter is at 728

counter is at 729

counter is at 730

counter is at 731

counter is at 732

counter is at 733

counter is at 734

counter is at 735

counter is at 736

counter is at 737

counter is at 738

counter is at 739

counter is at 740

counter is at 741

counter is at 742

counter is at 743

counter is at 744

counter is at 745

counter is at 746

counter is at 747

counter is at 748

counter is at 749

counter is at 750

counter is at 751

counter is at 752

counter is at 753

counter is at 754

counter is at 755

counter is at 756

counter is at 757

counter is at 758

counter is at 759

counter is at 760

counter is at 761

counter is at 762

counter is at 763

counter is at 764

counter is at 765

counter is at 766

counter is at 767

counter is at 768

counter is at 769

counter is at 770

counter is at 771

counter is at 772

counter is at 773

counter is at 774

counter is at 775

counter is at 776

counter is at 777

counter is at 778

counter is at 779

counter is at 780

counter is at 781

counter is at 782

counter is at 783

counter is at 784

counter is at 785

counter is at 786

counter is at 787

counter is at 788

counter is at 789

counter is at 790

counter is at 791

counter is at 792

counter is at 793

counter is at 794

counter is at 795

counter is at 796

counter is at 797

counter is at 798

counter is at 799

counter is at 800

counter is at 801

counter is at 802

counter is at 803

counter is at 804

counter is at 805

counter is at 806

counter is at 807

counter is at 808

counter is at 809

counter is at 810

counter is at 811

counter is at 812

counter is at 813

counter is at 814

counter is at 815

counter is at 816

counter is at 817

counter is at 818

counter is at 819

counter is at 820

counter is at 821

counter is at 822

counter is at 823

counter is at 824

counter is at 825

counter is at 826

counter is at 827

counter is at 828

counter is at 829

counter is at 830

counter is at 831

counter is at 832

counter is at 833

counter is at 834

counter is at 835

counter is at 836

counter is at 837

counter is at 838

counter is at 839

counter is at 840

counter is at 841

counter is at 842

counter is at 843

counter is at 844

counter is at 845

counter is at 846

counter is at 847

counter is at 848

counter is at 849

counter is at 850

counter is at 851

counter is at 852

counter is at 853

counter is at 854

counter is at 855

counter is at 856

counter is at 857

counter is at 858

counter is at 859

counter is at 860

counter is at 861

counter is at 862

counter is at 863

counter is at 864

counter is at 865

counter is at 866

counter is at 867

counter is at 868

counter is at 869

counter is at 870

counter is at 871

counter is at 872

counter is at 873

counter is at 874

counter is at 875

counter is at 876

counter is at 877

counter is at 878

counter is at 879

counter is at 880

counter is at 881

counter is at 882

counter is at 883

counter is at 884

counter is at 885

counter is at 886

counter is at 887

counter is at 888

counter is at 889

counter is at 890

counter is at 891

counter is at 892

counter is at 893

counter is at 894

counter is at 895

counter is at 896

counter is at 897

counter is at 898

counter is at 899

counter is at 900

counter is at 901

counter is at 902

counter is at 903

counter is at 904

counter is at 905

counter is at 906

counter is at 907

counter is at 908

counter is at 909

counter is at 910

counter is at 911

counter is at 912

counter is at 913

counter is at 914

counter is at 915

counter is at 916

counter is at 917

counter is at 918

counter is at 919

counter is at 920

counter is at 921

counter is at 922

counter is at 923

counter is at 924

counter is at 925

counter is at 926

counter is at 927

counter is at 928

counter is at 929

counter is at 930

counter is at 931

counter is at 932

counter is at 933

counter is at 934

counter is at 935

counter is at 936

counter is at 937

counter is at 938

counter is at 939

counter is at 940

counter is at 941

counter is at 942

counter is at 943

counter is at 944

counter is at 945

counter is at 946

counter is at 947

counter is at 948

counter is at 949

counter is at 950

counter is at 951

counter is at 952

counter is at 953

counter is at 954

counter is at 955

counter is at 956

counter is at 957

counter is at 958

counter is at 959

counter is at 960

counter is at 961

counter is at 962

counter is at 963

counter is at 964

counter is at 965

counter is at 966

counter is at 967

counter is at 968

counter is at 969

counter is at 970

counter is at 971

counter is at 972

counter is at 973

counter is at 974

counter is at 975

counter is at 976

counter is at 977

counter is at 978

counter is at 979

counter is at 980

counter is at 981

counter is at 982

counter is at 983

counter is at 984

counter is at 985

counter is at 986

counter is at 987

counter is at 988

counter is at 989

counter is at 990

counter is at 991

counter is at 992

counter is at 993

counter is at 994

counter is at 995

counter is at 996

counter is at 997

counter is at 998

counter is at 999

counter is at 1000

counter is at 1001

counter is at 1002

counter is at 1003

counter is at 1004

counter is at 1005

counter is at 1006

counter is at 1007

counter is at 1008

counter is at 1009

counter is at 1010

counter is at 1011

counter is at 1012

counter is at 1013

counter is at 1014

counter is at 1015

counter is at 1016

counter is at 1017

counter is at 1018

counter is at 1019

counter is at 1020

counter is at 1021

counter is at 1022

counter is at 1023

counter is at 1024

counter is at 1025

counter is at 1026

counter is at 1027

counter is at 1028

counter is at 1029

counter is at 1030

counter is at 1031

counter is at 1032

counter is at 1033

counter is at 1034

counter is at 1035

counter is at 1036

counter is at 1037

counter is at 1038

counter is at 1039

counter is at 1040

counter is at 1041

counter is at 1042

counter is at 1043

counter is at 1044

counter is at 1045

counter is at 1046

counter is at 1047

counter is at 1048

counter is at 1049

counter is at 1050

counter is at 1051

counter is at 1052

counter is at 1053

counter is at 1054

counter is at 1055

counter is at 1056

counter is at 1057

counter is at 1058

counter is at 1059

counter is at 1060

counter is at 1061

counter is at 1062

counter is at 1063

counter is at 1064

counter is at 1065

counter is at 1066

counter is at 1067

counter is at 1068

counter is at 1069

counter is at 1070

counter is at 1071

counter is at 1072

counter is at 1073

counter is at 1074

counter is at 1075

counter is at 1076

counter is at 1077

counter is at 1078

counter is at 1079

counter is at 1080

counter is at 1081

counter is at 1082

counter is at 1083

counter is at 1084

counter is at 1085

counter is at 1086

counter is at 1087

counter is at 1088

counter is at 1089

counter is at 1090

counter is at 1091

counter is at 1092

counter is at 1093

counter is at 1094

counter is at 1095

counter is at 1096

counter is at 1097

counter is at 1098

counter is at 1099

counter is at 1100

counter is at 1101

counter is at 1102

counter is at 1103

counter is at 1104

counter is at 1105

counter is at 1106

counter is at 1107

counter is at 1108

counter is at 1109

counter is at 1110

counter is at 1111

counter is at 1112

counter is at 1113

counter is at 1114

counter is at 1115

counter is at 1116

counter is at 1117

counter is at 1118

counter is at 1119

counter is at 1120

counter is at 1121

counter is at 1122

counter is at 1123

counter is at 1124

counter is at 1125

counter is at 1126

counter is at 1127

counter is at 1128

counter is at 1129

counter is at 1130

counter is at 1131

counter is at 1132

counter is at 1133

counter is at 1134

counter is at 1135

counter is at 1136

counter is at 1137

counter is at 1138

counter is at 1139

counter is at 1140

counter is at 1141

counter is at 1142

counter is at 1143

counter is at 1144

counter is at 1145

counter is at 1146

counter is at 1147

counter is at 1148

counter is at 1149

counter is at 1150

counter is at 1151

counter is at 1152

counter is at 1153

counter is at 1154

counter is at 1155

counter is at 1156

counter is at 1157

counter is at 1158

counter is at 1159

counter is at 1160

counter is at 1161

counter is at 1162

counter is at 1163

counter is at 1164

counter is at 1165

counter is at 1166

counter is at 1167

counter is at 1168

counter is at 1169

counter is at 1170

counter is at 1171

counter is at 1172

counter is at 1173

counter is at 1174

counter is at 1175

counter is at 1176

counter is at 1177

counter is at 1178

counter is at 1179

counter is at 1180

counter is at 1181

counter is at 1182

counter is at 1183

counter is at 1184

counter is at 1185

counter is at 1186

counter is at 1187

counter is at 1188

counter is at 1189

counter is at 1190

counter is at 1191

counter is at 1192

counter is at 1193

counter is at 1194

counter is at 1195

counter is at 1196

counter is at 1197

counter is at 1198

counter is at 1199

counter is at 1200

counter is at 1201

counter is at 1202

counter is at 1203

counter is at 1204

counter is at 1205

counter is at 1206

counter is at 1207

counter is at 1208

counter is at 1209

counter is at 1210

counter is at 1211

counter is at 1212

counter is at 1213

counter is at 1214

counter is at 1215

counter is at 1216

counter is at 1217

counter is at 1218

counter is at 1219

counter is at 1220

counter is at 1221

counter is at 1222

counter is at 1223

counter is at 1224

counter is at 1225

counter is at 1226

counter is at 1227

counter is at 1228

counter is at 1229

counter is at 1230

counter is at 1231

counter is at 1232

counter is at 1233

counter is at 1234

counter is at 1235

counter is at 1236

counter is at 1237

counter is at 1238

counter is at 1239

counter is at 1240

counter is at 1241

counter is at 1242

counter is at 1243

counter is at 1244

counter is at 1245

counter is at 1246

counter is at 1247

counter is at 1248

counter is at 1249

counter is at 1250

counter is at 1251

counter is at 1252

counter is at 1253

counter is at 1254

counter is at 1255

counter is at 1256

counter is at 1257

counter is at 1258

counter is at 1259

counter is at 1260

counter is at 1261

counter is at 1262

counter is at 1263

counter is at 1264

counter is at 1265

counter is at 1266

counter is at 1267

counter is at 1268

counter is at 1269

counter is at 1270

counter is at 1271

counter is at 1272

counter is at 1273

counter is at 1274

counter is at 1275

counter is at 1276

counter is at 1277

counter is at 1278

counter is at 1279

counter is at 1280

counter is at 1281

counter is at 1282

counter is at 1283

counter is at 1284

counter is at 1285

counter is at 1286

counter is at 1287

counter is at 1288

counter is at 1289

counter is at 1290

counter is at 1291

counter is at 1292

counter is at 1293

counter is at 1294

counter is at 1295

counter is at 1296

counter is at 1297

counter is at 1298

counter is at 1299

counter is at 1300

counter is at 1301

counter is at 1302

counter is at 1303

counter is at 1304

counter is at 1305

counter is at 1306

counter is at 1307

counter is at 1308

counter is at 1309

counter is at 1310

counter is at 1311

counter is at 1312

counter is at 1313

counter is at 1314

counter is at 1315

counter is at 1316

counter is at 1317

counter is at 1318

counter is at 1319

counter is at 1320

counter is at 1321

counter is at 1322

counter is at 1323

counter is at 1324

counter is at 1325

counter is at 1326

counter is at 1327

counter is at 1328

counter is at 1329

counter is at 1330

counter is at 1331

counter is at 1332

counter is at 1333

counter is at 1334

counter is at 1335

counter is at 1336

counter is at 1337

counter is at 1338

counter is at 1339

counter is at 1340

counter is at 1341

counter is at 1342

counter is at 1343

counter is at 1344

counter is at 1345

counter is at 1346

counter is at 1347

counter is at 1348

counter is at 1349

counter is at 1350

counter is at 1351

counter is at 1352

counter is at 1353

counter is at 1354

counter is at 1355

counter is at 1356

counter is at 1357

counter is at 1358

counter is at 1359

counter is at 1360

counter is at 1361

counter is at 1362

counter is at 1363

counter is at 1364

counter is at 1365

counter is at 1366

counter is at 1367

counter is at 1368

counter is at 1369

counter is at 1370

counter is at 1371

counter is at 1372

counter is at 1373

counter is at 1374

counter is at 1375

counter is at 1376

counter is at 1377

counter is at 1378

counter is at 1379

counter is at 1380

counter is at 1381

counter is at 1382

counter is at 1383

counter is at 1384

counter is at 1385

counter is at 1386

counter is at 1387

counter is at 1388

counter is at 1389

counter is at 1390

counter is at 1391

counter is at 1392

counter is at 1393

counter is at 1394

counter is at 1395

counter is at 1396

counter is at 1397

counter is at 1398

counter is at 1399

counter is at 1400

counter is at 1401

counter is at 1402

counter is at 1403

counter is at 1404

counter is at 1405

counter is at 1406

counter is at 1407

counter is at 1408

counter is at 1409

counter is at 1410

counter is at 1411

counter is at 1412

counter is at 1413

counter is at 1414

counter is at 1415

counter is at 1416

counter is at 1417

counter is at 1418

counter is at 1419

counter is at 1420

counter is at 1421

counter is at 1422

counter is at 1423

counter is at 1424

counter is at 1425

counter is at 1426

counter is at 1427

counter is at 1428

counter is at 1429

counter is at 1430

counter is at 1431

counter is at 1432

counter is at 1433

counter is at 1434

counter is at 1435

counter is at 1436

counter is at 1437

counter is at 1438

counter is at 1439

counter is at 1440

counter is at 1441

counter is at 1442

counter is at 1443

counter is at 1444

counter is at 1445

counter is at 1446

counter is at 1447

counter is at 1448

counter is at 1449

counter is at 1450

counter is at 1451

counter is at 1452

counter is at 1453

counter is at 1454

counter is at 1455

counter is at 1456

counter is at 1457

counter is at 1458

counter is at 1459

counter is at 1460

counter is at 1461

counter is at 1462

counter is at 1463

counter is at 1464

counter is at 1465

counter is at 1466

counter is at 1467

counter is at 1468

counter is at 1469

counter is at 1470

counter is at 1471

counter is at 1472

counter is at 1473

counter is at 1474

counter is at 1475

counter is at 1476

counter is at 1477

counter is at 1478

counter is at 1479

counter is at 1480

counter is at 1481

counter is at 1482

counter is at 1483

counter is at 1484

counter is at 1485

counter is at 1486

counter is at 1487

counter is at 1488

counter is at 1489

counter is at 1490

counter is at 1491

counter is at 1492

counter is at 1493

counter is at 1494

counter is at 1495

counter is at 1496

counter is at 1497

counter is at 1498

counter is at 1499

counter is at 1500

counter is at 1501

counter is at 1502

counter is at 1503

counter is at 1504

counter is at 1505

counter is at 1506

counter is at 1507

counter is at 1508

counter is at 1509

counter is at 1510

counter is at 1511

counter is at 1512

counter is at 1513

counter is at 1514

counter is at 1515

counter is at 1516

counter is at 1517

counter is at 1518

counter is at 1519

counter is at 1520

counter is at 1521

counter is at 1522

counter is at 1523

counter is at 1524

counter is at 1525

counter is at 1526

counter is at 1527

counter is at 1528

counter is at 1529

counter is at 1530

counter is at 1531

counter is at 1532

counter is at 1533

counter is at 1534

counter is at 1535

counter is at 1536

counter is at 1537

counter is at 1538

counter is at 1539

counter is at 1540

counter is at 1541

counter is at 1542

counter is at 1543

counter is at 1544

counter is at 1545

counter is at 1546

counter is at 1547

counter is at 1548

counter is at 1549

counter is at 1550

counter is at 1551

counter is at 1552

counter is at 1553

counter is at 1554

counter is at 1555

counter is at 1556

counter is at 1557

counter is at 1558

counter is at 1559

counter is at 1560

counter is at 1561

counter is at 1562

counter is at 1563

counter is at 1564

counter is at 1565

counter is at 1566

counter is at 1567

counter is at 1568

counter is at 1569

counter is at 1570

counter is at 1571

counter is at 1572

counter is at 1573

counter is at 1574

counter is at 1575

counter is at 1576

counter is at 1577

counter is at 1578

counter is at 1579

counter is at 1580

counter is at 1581

counter is at 1582

counter is at 1583

counter is at 1584

counter is at 1585

counter is at 1586

counter is at 1587

counter is at 1588

counter is at 1589

counter is at 1590

counter is at 1591

counter is at 1592

counter is at 1593

counter is at 1594

counter is at 1595

counter is at 1596

counter is at 1597

counter is at 1598

counter is at 1599

counter is at 1600

counter is at 1601

counter is at 1602

counter is at 1603

counter is at 1604

counter is at 1605

counter is at 1606

counter is at 1607

counter is at 1608

counter is at 1609

counter is at 1610

counter is at 1611

counter is at 1612

counter is at 1613

counter is at 1614

counter is at 1615

counter is at 1616

counter is at 1617

counter is at 1618

counter is at 1619

counter is at 1620

counter is at 1621

counter is at 1622

counter is at 1623

counter is at 1624

counter is at 1625

counter is at 1626

counter is at 1627

counter is at 1628

counter is at 1629

counter is at 1630

counter is at 1631

counter is at 1632

counter is at 1633

counter is at 1634

counter is at 1635

counter is at 1636

counter is at 1637

counter is at 1638

counter is at 1639

counter is at 1640

counter is at 1641

counter is at 1642

counter is at 1643

counter is at 1644

counter is at 1645

counter is at 1646

counter is at 1647

counter is at 1648

counter is at 1649

counter is at 1650

counter is at 1651

counter is at 1652

counter is at 1653

counter is at 1654

counter is at 1655

counter is at 1656

counter is at 1657

counter is at 1658

counter is at 1659

counter is at 1660

counter is at 1661

counter is at 1662

counter is at 1663

counter is at 1664

counter is at 1665

counter is at 1666

counter is at 1667

counter is at 1668

counter is at 1669

counter is at 1670

counter is at 1671

counter is at 1672

counter is at 1673

counter is at 1674

counter is at 1675

counter is at 1676

counter is at 1677

counter is at 1678

counter is at 1679

counter is at 1680

counter is at 1681

counter is at 1682

counter is at 1683

counter is at 1684

counter is at 1685

counter is at 1686

counter is at 1687

counter is at 1688

counter is at 1689

counter is at 1690

counter is at 1691

counter is at 1692

counter is at 1693

counter is at 1694

counter is at 1695

counter is at 1696

counter is at 1697

counter is at 1698

counter is at 1699

counter is at 1700

counter is at 1701

counter is at 1702

counter is at 1703

counter is at 1704

counter is at 1705

counter is at 1706

counter is at 1707

counter is at 1708

counter is at 1709

counter is at 1710

counter is at 1711

counter is at 1712

counter is at 1713

counter is at 1714

counter is at 1715

counter is at 1716

counter is at 1717

counter is at 1718

counter is at 1719

counter is at 1720

counter is at 1721

counter is at 1722

counter is at 1723

counter is at 1724

counter is at 1725

counter is at 1726

counter is at 1727

counter is at 1728

counter is at 1729

counter is at 1730

counter is at 1731

counter is at 1732

counter is at 1733

counter is at 1734

counter is at 1735

counter is at 1736

counter is at 1737

counter is at 1738

counter is at 1739

counter is at 1740

counter is at 1741

counter is at 1742

counter is at 1743

counter is at 1744

counter is at 1745

counter is at 1746

counter is at 1747

counter is at 1748

counter is at 1749

counter is at 1750

counter is at 1751

counter is at 1752

counter is at 1753

counter is at 1754

counter is at 1755

counter is at 1756

counter is at 1757

counter is at 1758

counter is at 1759

counter is at 1760

counter is at 1761

counter is at 1762

counter is at 1763

counter is at 1764

counter is at 1765

counter is at 1766

counter is at 1767

counter is at 1768

counter is at 1769

counter is at 1770

counter is at 1771

counter is at 1772

counter is at 1773

counter is at 1774

counter is at 1775

counter is at 1776

counter is at 1777

counter is at 1778

counter is at 1779

counter is at 1780

counter is at 1781

counter is at 1782

counter is at 1783

counter is at 1784

counter is at 1785

counter is at 1786

counter is at 1787

counter is at 1788

counter is at 1789

counter is at 1790

counter is at 1791

counter is at 1792

counter is at 1793

counter is at 1794

counter is at 1795

counter is at 1796

counter is at 1797

counter is at 1798

counter is at 1799

counter is at 1800

counter is at 1801

counter is at 1802

counter is at 1803

counter is at 1804

counter is at 1805

counter is at 1806

counter is at 1807

counter is at 1808

counter is at 1809

counter is at 1810

counter is at 1811

counter is at 1812

counter is at 1813

counter is at 1814

counter is at 1815

counter is at 1816

counter is at 1817

counter is at 1818

counter is at 1819

counter is at 1820

counter is at 1821

counter is at 1822

counter is at 1823

counter is at 1824

counter is at 1825

counter is at 1826

counter is at 1827

counter is at 1828

counter is at 1829

counter is at 1830

counter is at 1831

counter is at 1832

counter is at 1833

counter is at 1834

counter is at 1835

counter is at 1836

counter is at 1837

counter is at 1838

counter is at 1839

counter is at 1840

counter is at 1841

counter is at 1842

counter is at 1843

counter is at 1844

counter is at 1845

counter is at 1846

counter is at 1847

counter is at 1848

counter is at 1849

counter is at 1850

counter is at 1851

counter is at 1852

counter is at 1853

counter is at 1854

counter is at 1855

counter is at 1856

counter is at 1857

counter is at 1858

counter is at 1859

counter is at 1860

counter is at 1861

counter is at 1862

counter is at 1863

counter is at 1864

counter is at 1865

counter is at 1866

counter is at 1867

counter is at 1868

counter is at 1869

counter is at 1870

counter is at 1871

counter is at 1872

counter is at 1873

counter is at 1874

counter is at 1875

counter is at 1876

counter is at 1877

counter is at 1878

counter is at 1879

counter is at 1880

counter is at 1881

counter is at 1882

counter is at 1883

counter is at 1884

counter is at 1885

counter is at 1886

counter is at 1887

counter is at 1888

counter is at 1889

counter is at 1890

counter is at 1891

counter is at 1892

counter is at 1893

counter is at 1894

counter is at 1895

counter is at 1896

counter is at 1897

counter is at 1898

counter is at 1899

counter is at 1900

counter is at 1901

counter is at 1902

counter is at 1903

counter is at 1904

counter is at 1905

counter is at 1906

counter is at 1907

counter is at 1908

counter is at 1909

counter is at 1910

counter is at 1911

counter is at 1912

counter is at 1913

counter is at 1914

counter is at 1915

counter is at 1916

counter is at 1917

counter is at 1918

counter is at 1919

counter is at 1920

counter is at 1921

counter is at 1922

counter is at 1923

counter is at 1924

counter is at 1925

counter is at 1926

counter is at 1927

counter is at 1928

counter is at 1929

counter is at 1930

counter is at 1931

counter is at 1932

counter is at 1933

counter is at 1934

counter is at 1935

counter is at 1936

counter is at 1937

counter is at 1938

counter is at 1939

counter is at 1940

counter is at 1941

counter is at 1942

counter is at 1943

counter is at 1944

counter is at 1945

counter is at 1946

counter is at 1947

counter is at 1948

counter is at 1949

counter is at 1950

counter is at 1951

counter is at 1952

counter is at 1953

counter is at 1954

counter is at 1955

counter is at 1956

counter is at 1957

counter is at 1958

counter is at 1959

counter is at 1960

counter is at 1961

counter is at 1962

counter is at 1963

counter is at 1964

counter is at 1965

counter is at 1966

counter is at 1967

counter is at 1968

counter is at 1969

counter is at 1970

counter is at 1971

counter is at 1972

counter is at 1973

counter is at 1974

counter is at 1975

counter is at 1976

counter is at 1977

counter is at 1978

counter is at 1979

counter is at 1980

counter is at 1981

counter is at 1982

counter is at 1983

counter is at 1984

counter is at 1985

counter is at 1986

counter is at 1987

counter is at 1988

counter is at 1989

counter is at 1990

counter is at 1991

counter is at 1992

counter is at 1993

counter is at 1994

counter is at 1995

counter is at 1996

counter is at 1997

counter is at 1998

counter is at 1999

counter is at 2000

counter is at 2001

counter is at 2002

counter is at 2003

counter is at 2004

counter is at 2005

counter is at 2006

counter is at 2007

counter is at 2008

counter is at 2009

counter is at 2010

counter is at 2011

counter is at 2012

counter is at 2013

counter is at 2014

counter is at 2015

counter is at 2016

counter is at 2017

counter is at 2018

counter is at 2019

counter is at 2020

counter is at 2021

counter is at 2022

counter is at 2023

counter is at 2024

counter is at 2025

counter is at 2026

counter is at 2027

counter is at 2028

counter is at 2029

counter is at 2030

counter is at 2031

counter is at 2032

counter is at 2033

counter is at 2034

counter is at 2035

counter is at 2036

counter is at 2037

counter is at 2038

counter is at 2039

counter is at 2040

counter is at 2041

counter is at 2042

counter is at 2043

counter is at 2044

counter is at 2045

counter is at 2046

counter is at 2047

counter is at 2048

counter is at 2049

counter is at 2050

counter is at 2051

counter is at 2052

counter is at 2053

counter is at 2054

counter is at 2055

counter is at 2056

counter is at 2057

counter is at 2058

counter is at 2059

counter is at 2060

counter is at 2061

counter is at 2062

counter is at 2063

counter is at 2064

counter is at 2065

counter is at 2066

counter is at 2067

counter is at 2068

counter is at 2069

counter is at 2070

counter is at 2071

counter is at 2072

counter is at 2073

counter is at 2074

counter is at 2075

counter is at 2076

counter is at 2077

counter is at 2078

counter is at 2079

counter is at 2080

counter is at 2081

counter is at 2082

counter is at 2083

counter is at 2084

counter is at 2085

counter is at 2086

counter is at 2087

counter is at 2088

counter is at 2089

counter is at 2090

counter is at 2091

counter is at 2092

counter is at 2093

counter is at 2094

counter is at 2095

counter is at 2096

counter is at 2097

counter is at 2098

counter is at 2099

counter is at 2100

counter is at 2101

counter is at 2102

counter is at 2103

counter is at 2104

counter is at 2105

counter is at 2106

counter is at 2107

counter is at 2108

counter is at 2109

counter is at 2110

counter is at 2111

counter is at 2112

counter is at 2113

counter is at 2114

counter is at 2115

counter is at 2116

counter is at 2117

counter is at 2118

counter is at 2119

counter is at 2120

counter is at 2121

counter is at 2122

counter is at 2123

counter is at 2124

counter is at 2125

counter is at 2126

counter is at 2127

counter is at 2128

counter is at 2129

counter is at 2130

counter is at 2131

counter is at 2132

counter is at 2133

counter is at 2134

counter is at 2135

counter is at 2136

counter is at 2137

counter is at 2138

counter is at 2139

counter is at 2140

counter is at 2141

counter is at 2142

counter is at 2143

counter is at 2144

counter is at 2145

counter is at 2146

counter is at 2147

counter is at 2148

counter is at 2149

counter is at 2150

counter is at 2151

counter is at 2152

counter is at 2153

counter is at 2154

counter is at 2155

counter is at 2156

counter is at 2157

counter is at 2158

counter is at 2159

counter is at 2160

counter is at 2161

counter is at 2162

counter is at 2163

counter is at 2164

counter is at 2165

counter is at 2166

counter is at 2167

counter is at 2168

counter is at 2169

counter is at 2170

counter is at 2171

counter is at 2172

counter is at 2173

counter is at 2174

counter is at 2175

counter is at 2176

counter is at 2177

counter is at 2178

counter is at 2179

counter is at 2180

counter is at 2181

counter is at 2182

counter is at 2183

counter is at 2184

counter is at 2185

counter is at 2186

counter is at 2187

counter is at 2188

counter is at 2189

counter is at 2190

counter is at 2191

counter is at 2192

counter is at 2193

counter is at 2194

counter is at 2195

counter is at 2196

counter is at 2197

counter is at 2198

counter is at 2199

counter is at 2200

counter is at 2201

counter is at 2202

counter is at 2203

counter is at 2204

counter is at 2205

counter is at 2206

counter is at 2207

counter is at 2208

counter is at 2209

counter is at 2210

counter is at 2211

counter is at 2212

counter is at 2213

counter is at 2214

counter is at 2215

counter is at 2216

counter is at 2217

counter is at 2218

counter is at 2219

counter is at 2220

counter is at 2221

counter is at 2222

counter is at 2223

counter is at 2224

counter is at 2225

counter is at 2226

counter is at 2227

counter is at 2228

counter is at 2229

counter is at 2230

counter is at 2231

counter is at 2232

counter is at 2233

counter is at 2234

counter is at 2235

counter is at 2236

counter is at 2237

counter is at 2238

counter is at 2239

counter is at 2240

counter is at 2241

counter is at 2242

counter is at 2243

counter is at 2244

counter is at 2245

counter is at 2246

counter is at 2247

counter is at 2248

counter is at 2249

counter is at 2250

counter is at 2251

counter is at 2252

counter is at 2253

counter is at 2254

counter is at 2255

counter is at 2256

counter is at 2257

counter is at 2258

counter is at 2259

counter is at 2260

counter is at 2261

counter is at 2262

counter is at 2263

counter is at 2264

counter is at 2265

counter is at 2266

counter is at 2267

counter is at 2268

counter is at 2269

counter is at 2270

counter is at 2271

counter is at 2272

counter is at 2273

counter is at 2274

counter is at 2275

counter is at 2276

counter is at 2277

counter is at 2278

counter is at 2279

counter is at 2280

counter is at 2281

counter is at 2282

counter is at 2283

counter is at 2284

counter is at 2285

counter is at 2286

counter is at 2287

counter is at 2288

counter is at 2289

counter is at 2290

counter is at 2291

counter is at 2292

counter is at 2293

counter is at 2294

counter is at 2295

counter is at 2296

counter is at 2297

counter is at 2298

counter is at 2299

counter is at 2300

counter is at 2301

counter is at 2302

counter is at 2303

counter is at 2304

counter is at 2305

counter is at 2306

counter is at 2307

counter is at 2308

counter is at 2309

counter is at 2310

counter is at 2311

counter is at 2312

counter is at 2313

counter is at 2314

counter is at 2315

counter is at 2316

counter is at 2317

counter is at 2318

counter is at 2319

counter is at 2320

counter is at 2321

counter is at 2322

counter is at 2323

counter is at 2324

counter is at 2325

counter is at 2326

counter is at 2327

counter is at 2328

counter is at 2329

counter is at 2330

counter is at 2331

counter is at 2332

counter is at 2333

counter is at 2334

counter is at 2335

counter is at 2336

counter is at 2337

counter is at 2338

counter is at 2339

counter is at 2340

counter is at 2341

counter is at 2342

counter is at 2343

counter is at 2344

counter is at 2345

counter is at 2346

counter is at 2347

counter is at 2348

counter is at 2349

counter is at 2350

counter is at 2351

counter is at 2352

counter is at 2353

counter is at 2354

counter is at 2355

counter is at 2356

counter is at 2357

counter is at 2358

counter is at 2359

counter is at 2360

counter is at 2361

counter is at 2362

counter is at 2363

counter is at 2364

counter is at 2365

counter is at 2366

counter is at 2367

counter is at 2368

counter is at 2369

counter is at 2370

counter is at 2371

counter is at 2372

counter is at 2373

counter is at 2374

counter is at 2375

counter is at 2376

counter is at 2377

counter is at 2378

counter is at 2379

counter is at 2380

counter is at 2381

counter is at 2382

counter is at 2383

counter is at 2384

counter is at 2385

counter is at 2386

counter is at 2387

counter is at 2388

counter is at 2389

counter is at 2390

counter is at 2391

counter is at 2392

counter is at 2393

counter is at 2394

counter is at 2395

counter is at 2396

counter is at 2397

counter is at 2398

counter is at 2399

counter is at 2400

counter is at 2401

counter is at 2402

counter is at 2403

counter is at 2404

counter is at 2405

counter is at 2406

counter is at 2407

counter is at 2408

counter is at 2409

counter is at 2410

counter is at 2411

counter is at 2412

counter is at 2413

counter is at 2414

counter is at 2415

counter is at 2416

counter is at 2417

counter is at 2418

counter is at 2419

counter is at 2420

counter is at 2421

counter is at 2422

counter is at 2423

counter is at 2424

counter is at 2425

counter is at 2426

counter is at 2427

counter is at 2428

counter is at 2429

counter is at 2430

counter is at 2431

counter is at 2432

counter is at 2433

counter is at 2434

counter is at 2435

counter is at 2436

counter is at 2437

counter is at 2438

counter is at 2439

counter is at 2440

counter is at 2441

counter is at 2442

counter is at 2443

counter is at 2444

counter is at 2445

counter is at 2446

counter is at 2447

counter is at 2448

counter is at 2449

counter is at 2450

counter is at 2451

counter is at 2452

counter is at 2453

counter is at 2454

counter is at 2455

counter is at 2456

counter is at 2457

counter is at 2458

counter is at 2459

counter is at 2460

counter is at 2461

counter is at 2462

counter is at 2463

counter is at 2464

counter is at 2465

counter is at 2466

counter is at 2467

counter is at 2468

counter is at 2469

counter is at 2470

counter is at 2471

counter is at 2472

counter is at 2473

counter is at 2474

counter is at 2475

counter is at 2476

counter is at 2477

counter is at 2478

counter is at 2479

counter is at 2480

counter is at 2481

counter is at 2482

counter is at 2483

counter is at 2484

counter is at 2485

counter is at 2486

counter is at 2487

counter is at 2488

counter is at 2489

counter is at 2490

counter is at 2491

counter is at 2492

counter is at 2493

counter is at 2494

counter is at 2495

counter is at 2496

counter is at 2497

counter is at 2498

counter is at 2499

counter is at 2500

counter is at 2501

counter is at 2502

counter is at 2503

counter is at 2504

counter is at 2505

counter is at 2506

counter is at 2507

counter is at 2508

counter is at 2509

counter is at 2510

counter is at 2511

counter is at 2512

counter is at 2513

counter is at 2514

counter is at 2515

counter is at 2516

counter is at 2517

counter is at 2518

counter is at 2519

counter is at 2520

counter is at 2521

counter is at 2522

counter is at 2523

counter is at 2524

counter is at 2525

counter is at 2526

counter is at 2527

counter is at 2528

counter is at 2529

counter is at 2530

counter is at 2531

counter is at 2532

counter is at 2533

counter is at 2534

counter is at 2535

counter is at 2536

counter is at 2537

counter is at 2538

counter is at 2539

counter is at 2540

counter is at 2541

counter is at 2542

counter is at 2543

counter is at 2544

counter is at 2545

counter is at 2546

counter is at 2547

counter is at 2548

counter is at 2549

counter is at 2550

counter is at 2551

counter is at 2552

counter is at 2553

counter is at 2554

counter is at 2555

counter is at 2556

counter is at 2557

counter is at 2558

counter is at 2559

counter is at 2560

counter is at 2561

counter is at 2562

counter is at 2563

counter is at 2564

counter is at 2565

counter is at 2566

counter is at 2567

counter is at 2568

counter is at 2569

counter is at 2570

counter is at 2571

counter is at 2572

counter is at 2573

counter is at 2574

counter is at 2575

counter is at 2576

counter is at 2577

counter is at 2578

counter is at 2579

counter is at 2580

counter is at 2581

counter is at 2582

counter is at 2583

counter is at 2584

counter is at 2585

counter is at 2586

counter is at 2587

counter is at 2588

counter is at 2589

counter is at 2590

counter is at 2591

counter is at 2592

counter is at 2593

counter is at 2594

counter is at 2595

counter is at 2596

counter is at 2597

counter is at 2598

counter is at 2599

counter is at 2600

counter is at 2601

counter is at 2602

counter is at 2603

counter is at 2604

counter is at 2605

counter is at 2606

counter is at 2607

counter is at 2608

counter is at 2609

counter is at 2610

counter is at 2611

counter is at 2612

counter is at 2613

counter is at 2614

counter is at 2615

counter is at 2616

counter is at 2617

counter is at 2618

counter is at 2619

counter is at 2620

counter is at 2621

counter is at 2622

counter is at 2623

counter is at 2624

counter is at 2625

counter is at 2626

counter is at 2627

counter is at 2628

counter is at 2629

counter is at 2630

counter is at 2631

counter is at 2632

counter is at 2633

counter is at 2634

counter is at 2635

counter is at 2636

counter is at 2637

counter is at 2638

counter is at 2639

counter is at 2640

counter is at 2641

counter is at 2642

counter is at 2643

counter is at 2644

counter is at 2645

counter is at 2646

counter is at 2647

counter is at 2648

counter is at 2649

counter is at 2650

counter is at 2651

counter is at 2652

counter is at 2653

counter is at 2654

counter is at 2655

counter is at 2656

counter is at 2657

counter is at 2658

counter is at 2659

counter is at 2660

counter is at 2661

counter is at 2662

counter is at 2663

counter is at 2664

counter is at 2665

counter is at 2666

counter is at 2667

counter is at 2668

counter is at 2669

counter is at 2670

counter is at 2671

counter is at 2672

counter is at 2673

counter is at 2674

counter is at 2675

counter is at 2676

counter is at 2677

counter is at 2678

counter is at 2679

counter is at 2680

counter is at 2681

counter is at 2682

counter is at 2683

counter is at 2684

counter is at 2685

counter is at 2686

counter is at 2687

counter is at 2688

counter is at 2689

counter is at 2690

counter is at 2691

counter is at 2692

counter is at 2693

counter is at 2694

counter is at 2695

counter is at 2696

counter is at 2697

counter is at 2698

counter is at 2699

counter is at 2700

counter is at 2701

counter is at 2702

counter is at 2703

counter is at 2704

counter is at 2705

counter is at 2706

counter is at 2707

counter is at 2708

counter is at 2709

counter is at 2710

counter is at 2711

counter is at 2712

counter is at 2713

counter is at 2714

counter is at 2715

counter is at 2716

counter is at 2717

counter is at 2718

counter is at 2719

counter is at 2720

counter is at 2721

counter is at 2722

counter is at 2723

counter is at 2724

counter is at 2725

counter is at 2726

counter is at 2727

counter is at 2728

counter is at 2729

counter is at 2730

counter is at 2731

counter is at 2732

counter is at 2733

counter is at 2734

counter is at 2735

counter is at 2736

counter is at 2737

counter is at 2738

counter is at 2739

counter is at 2740

counter is at 2741

counter is at 2742

counter is at 2743

counter is at 2744

counter is at 2745

counter is at 2746

counter is at 2747

counter is at 2748

counter is at 2749

counter is at 2750

counter is at 2751

counter is at 2752

counter is at 2753

counter is at 2754

counter is at 2755

counter is at 2756

counter is at 2757

counter is at 2758

counter is at 2759

counter is at 2760

counter is at 2761

counter is at 2762

counter is at 2763

counter is at 2764

counter is at 2765

counter is at 2766

counter is at 2767

counter is at 2768

counter is at 2769

counter is at 2770

counter is at 2771

counter is at 2772

counter is at 2773

counter is at 2774

counter is at 2775

counter is at 2776

counter is at 2777

counter is at 2778

counter is at 2779

counter is at 2780

counter is at 2781

counter is at 2782

counter is at 2783

counter is at 2784

counter is at 2785

counter is at 2786

counter is at 2787

counter is at 2788

counter is at 2789

counter is at 2790

counter is at 2791

counter is at 2792

counter is at 2793

counter is at 2794

counter is at 2795

counter is at 2796

counter is at 2797

counter is at 2798

counter is at 2799

counter is at 2800

counter is at 2801

counter is at 2802

counter is at 2803

counter is at 2804

counter is at 2805

counter is at 2806

counter is at 2807

counter is at 2808

counter is at 2809

counter is at 2810

counter is at 2811

counter is at 2812

counter is at 2813

counter is at 2814

counter is at 2815

counter is at 2816

counter is at 2817

counter is at 2818

counter is at 2819

counter is at 2820

counter is at 2821

counter is at 2822

counter is at 2823

counter is at 2824

counter is at 2825

counter is at 2826

counter is at 2827

counter is at 2828

counter is at 2829

counter is at 2830

counter is at 2831

counter is at 2832

counter is at 2833

counter is at 2834

counter is at 2835

counter is at 2836

counter is at 2837

counter is at 2838

counter is at 2839

counter is at 2840

counter is at 2841

counter is at 2842

counter is at 2843

counter is at 2844

counter is at 2845

counter is at 2846

counter is at 2847

counter is at 2848

counter is at 2849

counter is at 2850

counter is at 2851

counter is at 2852

counter is at 2853

counter is at 2854

counter is at 2855

counter is at 2856

counter is at 2857

counter is at 2858

counter is at 2859

counter is at 2860

counter is at 2861

counter is at 2862

counter is at 2863

counter is at 2864

counter is at 2865

counter is at 2866

counter is at 2867

counter is at 2868

counter is at 2869

counter is at 2870

counter is at 2871

counter is at 2872

counter is at 2873

counter is at 2874

counter is at 2875

counter is at 2876

counter is at 2877

counter is at 2878

counter is at 2879

counter is at 2880

counter is at 2881

counter is at 2882

counter is at 2883

counter is at 2884

counter is at 2885

counter is at 2886

counter is at 2887

counter is at 2888

counter is at 2889

counter is at 2890

counter is at 2891

counter is at 2892

counter is at 2893

counter is at 2894

counter is at 2895

counter is at 2896

counter is at 2897

counter is at 2898

counter is at 2899

counter is at 2900

counter is at 2901

counter is at 2902

counter is at 2903

counter is at 2904

counter is at 2905

counter is at 2906

counter is at 2907

counter is at 2908

counter is at 2909

counter is at 2910

counter is at 2911

counter is at 2912

counter is at 2913

counter is at 2914

counter is at 2915

counter is at 2916

counter is at 2917

counter is at 2918

counter is at 2919

counter is at 2920

counter is at 2921

counter is at 2922

counter is at 2923

counter is at 2924

counter is at 2925

counter is at 2926

counter is at 2927

counter is at 2928

counter is at 2929

counter is at 2930

counter is at 2931

counter is at 2932

counter is at 2933

counter is at 2934

counter is at 2935

counter is at 2936

counter is at 2937

counter is at 2938

counter is at 2939

counter is at 2940

counter is at 2941

counter is at 2942

counter is at 2943

counter is at 2944

counter is at 2945

counter is at 2946

counter is at 2947

counter is at 2948

counter is at 2949

counter is at 2950

counter is at 2951

counter is at 2952

counter is at 2953

counter is at 2954

counter is at 2955

counter is at 2956

counter is at 2957

counter is at 2958

counter is at 2959

counter is at 2960

counter is at 2961

counter is at 2962

counter is at 2963

counter is at 2964

counter is at 2965

counter is at 2966

counter is at 2967

counter is at 2968

counter is at 2969

counter is at 2970

counter is at 2971

counter is at 2972

counter is at 2973

counter is at 2974

counter is at 2975

counter is at 2976

counter is at 2977

counter is at 2978

counter is at 2979

counter is at 2980

counter is at 2981

counter is at 2982

counter is at 2983

counter is at 2984

counter is at 2985

counter is at 2986

counter is at 2987

counter is at 2988

counter is at 2989

counter is at 2990

counter is at 2991

counter is at 2992

counter is at 2993

counter is at 2994

counter is at 2995

counter is at 2996

counter is at 2997

counter is at 2998

counter is at 2999

counter is at 3000

counter is at 3001

counter is at 3002

counter is at 3003

counter is at 3004

counter is at 3005

counter is at 3006

counter is at 3007

counter is at 3008

counter is at 3009

counter is at 3010

counter is at 3011

counter is at 3012

counter is at 3013

counter is at 3014

counter is at 3015

counter is at 3016

counter is at 3017

counter is at 3018

counter is at 3019

counter is at 3020

counter is at 3021

counter is at 3022

counter is at 3023

counter is at 3024

counter is at 3025

counter is at 3026

counter is at 3027

counter is at 3028

counter is at 3029

counter is at 3030

counter is at 3031

counter is at 3032

counter is at 3033

counter is at 3034

counter is at 3035

counter is at 3036

counter is at 3037

counter is at 3038

counter is at 3039

counter is at 3040

counter is at 3041

counter is at 3042

counter is at 3043

counter is at 3044

counter is at 3045

counter is at 3046

counter is at 3047

counter is at 3048

counter is at 3049

counter is at 3050

counter is at 3051

counter is at 3052

counter is at 3053

counter is at 3054

counter is at 3055

counter is at 3056

counter is at 3057

counter is at 3058

counter is at 3059

counter is at 3060

counter is at 3061

counter is at 3062

counter is at 3063

counter is at 3064

counter is at 3065

counter is at 3066

counter is at 3067

counter is at 3068

counter is at 3069

counter is at 3070

counter is at 3071

counter is at 3072

counter is at 3073

counter is at 3074

counter is at 3075

counter is at 3076

counter is at 3077

counter is at 3078

counter is at 3079

counter is at 3080

counter is at 3081

counter is at 3082

counter is at 3083

counter is at 3084

counter is at 3085

counter is at 3086

counter is at 3087

counter is at 3088

counter is at 3089

counter is at 3090

counter is at 3091

counter is at 3092

counter is at 3093

counter is at 3094

counter is at 3095

counter is at 3096

counter is at 3097

counter is at 3098

counter is at 3099

counter is at 3100

counter is at 3101

counter is at 3102

counter is at 3103

counter is at 3104

counter is at 3105

counter is at 3106

counter is at 3107

counter is at 3108

counter is at 3109

counter is at 3110

counter is at 3111

counter is at 3112

counter is at 3113

counter is at 3114

counter is at 3115

counter is at 3116

counter is at 3117

counter is at 3118

counter is at 3119

counter is at 3120

counter is at 3121

counter is at 3122

counter is at 3123

counter is at 3124

counter is at 3125

counter is at 3126

counter is at 3127

counter is at 3128

counter is at 3129

counter is at 3130

counter is at 3131

counter is at 3132

counter is at 3133

counter is at 3134

counter is at 3135

counter is at 3136

counter is at 3137

counter is at 3138

counter is at 3139

counter is at 3140

counter is at 3141

counter is at 3142

counter is at 3143

counter is at 3144

counter is at 3145

counter is at 3146

counter is at 3147

counter is at 3148

counter is at 3149

counter is at 3150

counter is at 3151

counter is at 3152

counter is at 3153

counter is at 3154

counter is at 3155

counter is at 3156

counter is at 3157

counter is at 3158

counter is at 3159

counter is at 3160

counter is at 3161

counter is at 3162

counter is at 3163

counter is at 3164

counter is at 3165

counter is at 3166

counter is at 3167

counter is at 3168

counter is at 3169

counter is at 3170

counter is at 3171

counter is at 3172

counter is at 3173

counter is at 3174

counter is at 3175

counter is at 3176

counter is at 3177

counter is at 3178

counter is at 3179

counter is at 3180

counter is at 3181

counter is at 3182

counter is at 3183

counter is at 3184

counter is at 3185

counter is at 3186

counter is at 3187

counter is at 3188

counter is at 3189

counter is at 3190

counter is at 3191

counter is at 3192

counter is at 3193

counter is at 3194

counter is at 3195

counter is at 3196

counter is at 3197

counter is at 3198

counter is at 3199

counter is at 3200

counter is at 3201

counter is at 3202

counter is at 3203

counter is at 3204

counter is at 3205

counter is at 3206

counter is at 3207

counter is at 3208

counter is at 3209

counter is at 3210

counter is at 3211

counter is at 3212

counter is at 3213

counter is at 3214

counter is at 3215

counter is at 3216

counter is at 3217

counter is at 3218

counter is at 3219

counter is at 3220

counter is at 3221

counter is at 3222

counter is at 3223

counter is at 3224

counter is at 3225

counter is at 3226

counter is at 3227

counter is at 3228

counter is at 3229

counter is at 3230

counter is at 3231

counter is at 3232

counter is at 3233

counter is at 3234

counter is at 3235

counter is at 3236

counter is at 3237

counter is at 3238

counter is at 3239

counter is at 3240

counter is at 3241

counter is at 3242

counter is at 3243

counter is at 3244

counter is at 3245

counter is at 3246

counter is at 3247

counter is at 3248

counter is at 3249

counter is at 3250

counter is at 3251

counter is at 3252

counter is at 3253

counter is at 3254

counter is at 3255

counter is at 3256

counter is at 3257

counter is at 3258

counter is at 3259

counter is at 3260

counter is at 3261

counter is at 3262

counter is at 3263

counter is at 3264

counter is at 3265

counter is at 3266

counter is at 3267

counter is at 3268

counter is at 3269

counter is at 3270

counter is at 3271

counter is at 3272

counter is at 3273

counter is at 3274

counter is at 3275

counter is at 3276

counter is at 3277

counter is at 3278

counter is at 3279

counter is at 3280

counter is at 3281

counter is at 3282

counter is at 3283

counter is at 3284

counter is at 3285

counter is at 3286

counter is at 3287

counter is at 3288

counter is at 3289

counter is at 3290

counter is at 3291

counter is at 3292

counter is at 3293

counter is at 3294

counter is at 3295

counter is at 3296

counter is at 3297

counter is at 3298

counter is at 3299

counter is at 3300

counter is at 3301

counter is at 3302

counter is at 3303

counter is at 3304

counter is at 3305

counter is at 3306

counter is at 3307

counter is at 3308

counter is at 3309

counter is at 3310

counter is at 3311

counter is at 3312

counter is at 3313

counter is at 3314

counter is at 3315

counter is at 3316

counter is at 3317

counter is at 3318

counter is at 3319

counter is at 3320

counter is at 3321

counter is at 3322

counter is at 3323

counter is at 3324

counter is at 3325

counter is at 3326

counter is at 3327

counter is at 3328

counter is at 3329

counter is at 3330

counter is at 3331

counter is at 3332

counter is at 3333

counter is at 3334

counter is at 3335

counter is at 3336

counter is at 3337

counter is at 3338

counter is at 3339

counter is at 3340

counter is at 3341

counter is at 3342

counter is at 3343

counter is at 3344

counter is at 3345

counter is at 3346

counter is at 3347

counter is at 3348

counter is at 3349

counter is at 3350

counter is at 3351

counter is at 3352

counter is at 3353

counter is at 3354

counter is at 3355

counter is at 3356

counter is at 3357

counter is at 3358

counter is at 3359

counter is at 3360

counter is at 3361

counter is at 3362

counter is at 3363

counter is at 3364

counter is at 3365

counter is at 3366

counter is at 3367

counter is at 3368

counter is at 3369

counter is at 3370

counter is at 3371

counter is at 3372

counter is at 3373

counter is at 3374

counter is at 3375

counter is at 3376

counter is at 3377

counter is at 3378

counter is at 3379

counter is at 3380

counter is at 3381

counter is at 3382

counter is at 3383

counter is at 3384

counter is at 3385

counter is at 3386

counter is at 3387

counter is at 3388

counter is at 3389

counter is at 3390

counter is at 3391

counter is at 3392

counter is at 3393

counter is at 3394

counter is at 3395

counter is at 3396

counter is at 3397

counter is at 3398

counter is at 3399

counter is at 3400

counter is at 3401

counter is at 3402

counter is at 3403

counter is at 3404

counter is at 3405

counter is at 3406

counter is at 3407

counter is at 3408

counter is at 3409

counter is at 3410

counter is at 3411

counter is at 3412

counter is at 3413

counter is at 3414

counter is at 3415

counter is at 3416

counter is at 3417

counter is at 3418

counter is at 3419

counter is at 3420

counter is at 3421

counter is at 3422

counter is at 3423

counter is at 3424

counter is at 3425

counter is at 3426

counter is at 3427

counter is at 3428

counter is at 3429

counter is at 3430

counter is at 3431

counter is at 3432

counter is at 3433

counter is at 3434

counter is at 3435

counter is at 3436

counter is at 3437

counter is at 3438

counter is at 3439

counter is at 3440

counter is at 3441

counter is at 3442

counter is at 3443

counter is at 3444

counter is at 3445

counter is at 3446

counter is at 3447

counter is at 3448

counter is at 3449

counter is at 3450

counter is at 3451

counter is at 3452

counter is at 3453

counter is at 3454

counter is at 3455

counter is at 3456

counter is at 3457

counter is at 3458

counter is at 3459

counter is at 3460

counter is at 3461

counter is at 3462

counter is at 3463

counter is at 3464

counter is at 3465

counter is at 3466

counter is at 3467

counter is at 3468

counter is at 3469

counter is at 3470

counter is at 3471

counter is at 3472

counter is at 3473

counter is at 3474

counter is at 3475

counter is at 3476

counter is at 3477

counter is at 3478

counter is at 3479

counter is at 3480

counter is at 3481

counter is at 3482

counter is at 3483

counter is at 3484

counter is at 3485

counter is at 3486

counter is at 3487

counter is at 3488

counter is at 3489

counter is at 3490

counter is at 3491

counter is at 3492

counter is at 3493

counter is at 3494

counter is at 3495

counter is at 3496

counter is at 3497

counter is at 3498

counter is at 3499

counter is at 3500

counter is at 3501

counter is at 3502

counter is at 3503

counter is at 3504

counter is at 3505

counter is at 3506

counter is at 3507

counter is at 3508

counter is at 3509

counter is at 3510

counter is at 3511

counter is at 3512

counter is at 3513

counter is at 3514

counter is at 3515

counter is at 3516

counter is at 3517

counter is at 3518

counter is at 3519

counter is at 3520

counter is at 3521

counter is at 3522

counter is at 3523

counter is at 3524

counter is at 3525

counter is at 3526

counter is at 3527

counter is at 3528

counter is at 3529

counter is at 3530

counter is at 3531

counter is at 3532

counter is at 3533

counter is at 3534

counter is at 3535

counter is at 3536

counter is at 3537

counter is at 3538

counter is at 3539

counter is at 3540

counter is at 3541

counter is at 3542

counter is at 3543

counter is at 3544

counter is at 3545

counter is at 3546

counter is at 3547

counter is at 3548

counter is at 3549

counter is at 3550

counter is at 3551

counter is at 3552

counter is at 3553

counter is at 3554

counter is at 3555

counter is at 3556

counter is at 3557

counter is at 3558

counter is at 3559

counter is at 3560

counter is at 3561

counter is at 3562

counter is at 3563

counter is at 3564

counter is at 3565

counter is at 3566

counter is at 3567

counter is at 3568

counter is at 3569

counter is at 3570

counter is at 3571

counter is at 3572

counter is at 3573

counter is at 3574

counter is at 3575

counter is at 3576

counter is at 3577

counter is at 3578

counter is at 3579

counter is at 3580

counter is at 3581

counter is at 3582

counter is at 3583

counter is at 3584

counter is at 3585

counter is at 3586

counter is at 3587

counter is at 3588

counter is at 3589

counter is at 3590

counter is at 3591

counter is at 3592

counter is at 3593

counter is at 3594

counter is at 3595

counter is at 3596

counter is at 3597

counter is at 3598

counter is at 3599

counter is at 3600

counter is at 3601

counter is at 3602

counter is at 3603

counter is at 3604

counter is at 3605

counter is at 3606

counter is at 3607

counter is at 3608

counter is at 3609

counter is at 3610

counter is at 3611

counter is at 3612

counter is at 3613

counter is at 3614

counter is at 3615

counter is at 3616

counter is at 3617

counter is at 3618

counter is at 3619

counter is at 3620

counter is at 3621

counter is at 3622

counter is at 3623

counter is at 3624

counter is at 3625

counter is at 3626

counter is at 3627

counter is at 3628

counter is at 3629

counter is at 3630

counter is at 3631

counter is at 3632

counter is at 3633

counter is at 3634

counter is at 3635

counter is at 3636

counter is at 3637

counter is at 3638

counter is at 3639

counter is at 3640

counter is at 3641

counter is at 3642

counter is at 3643

counter is at 3644

counter is at 3645

counter is at 3646

counter is at 3647

counter is at 3648

counter is at 3649

counter is at 3650

counter is at 3651

counter is at 3652

counter is at 3653

counter is at 3654

counter is at 3655

counter is at 3656

counter is at 3657

counter is at 3658

counter is at 3659

counter is at 3660

counter is at 3661

counter is at 3662

counter is at 3663

counter is at 3664

counter is at 3665

counter is at 3666

counter is at 3667

counter is at 3668

counter is at 3669

counter is at 3670

counter is at 3671

counter is at 3672

counter is at 3673

counter is at 3674

counter is at 3675

counter is at 3676

counter is at 3677

counter is at 3678

counter is at 3679

counter is at 3680

counter is at 3681

counter is at 3682

counter is at 3683

counter is at 3684

counter is at 3685

counter is at 3686

counter is at 3687

counter is at 3688

counter is at 3689

counter is at 3690

counter is at 3691

counter is at 3692

counter is at 3693

counter is at 3694

counter is at 3695

counter is at 3696

counter is at 3697

counter is at 3698

counter is at 3699

counter is at 3700

counter is at 3701

counter is at 3702

counter is at 3703

counter is at 3704

counter is at 3705

counter is at 3706

counter is at 3707

counter is at 3708

counter is at 3709

counter is at 3710

counter is at 3711

counter is at 3712

counter is at 3713

counter is at 3714

counter is at 3715

counter is at 3716

counter is at 3717

counter is at 3718

counter is at 3719

counter is at 3720

counter is at 3721

counter is at 3722

counter is at 3723

counter is at 3724

counter is at 3725

counter is at 3726

counter is at 3727

counter is at 3728

counter is at 3729

counter is at 3730

counter is at 3731

counter is at 3732

counter is at 3733

counter is at 3734

counter is at 3735

counter is at 3736

counter is at 3737

counter is at 3738

counter is at 3739

counter is at 3740

counter is at 3741

counter is at 3742

counter is at 3743

counter is at 3744

counter is at 3745

counter is at 3746

counter is at 3747

counter is at 3748

counter is at 3749

counter is at 3750

counter is at 3751

counter is at 3752

counter is at 3753

counter is at 3754

counter is at 3755

counter is at 3756

counter is at 3757

counter is at 3758

counter is at 3759

counter is at 3760

counter is at 3761

counter is at 3762

counter is at 3763

counter is at 3764

counter is at 3765

counter is at 3766

counter is at 3767

counter is at 3768

counter is at 3769

counter is at 3770

counter is at 3771

counter is at 3772

counter is at 3773

counter is at 3774

counter is at 3775

counter is at 3776

counter is at 3777

counter is at 3778

counter is at 3779

counter is at 3780

counter is at 3781

counter is at 3782

counter is at 3783

counter is at 3784

counter is at 3785

counter is at 3786

counter is at 3787

counter is at 3788

counter is at 3789

counter is at 3790

counter is at 3791

counter is at 3792

counter is at 3793

counter is at 3794

counter is at 3795

counter is at 3796

counter is at 3797

counter is at 3798

counter is at 3799

counter is at 3800

counter is at 3801

counter is at 3802

counter is at 3803

counter is at 3804

counter is at 3805

counter is at 3806

counter is at 3807

counter is at 3808

counter is at 3809

counter is at 3810

counter is at 3811

counter is at 3812

counter is at 3813

counter is at 3814

counter is at 3815

counter is at 3816

counter is at 3817

counter is at 3818

counter is at 3819

counter is at 3820

counter is at 3821

counter is at 3822

counter is at 3823

counter is at 3824

counter is at 3825

counter is at 3826

counter is at 3827

counter is at 3828

counter is at 3829

counter is at 3830

counter is at 3831

counter is at 3832

counter is at 3833

counter is at 3834

counter is at 3835

counter is at 3836

counter is at 3837

counter is at 3838

counter is at 3839

counter is at 3840

counter is at 3841

counter is at 3842

counter is at 3843

counter is at 3844

counter is at 3845

counter is at 3846

counter is at 3847

counter is at 3848

counter is at 3849

counter is at 3850

counter is at 3851

counter is at 3852

counter is at 3853

counter is at 3854

counter is at 3855

counter is at 3856

counter is at 3857

counter is at 3858

counter is at 3859

counter is at 3860

counter is at 3861

counter is at 3862

counter is at 3863

counter is at 3864

counter is at 3865

counter is at 3866

counter is at 3867

counter is at 3868

counter is at 3869

counter is at 3870

counter is at 3871

counter is at 3872

counter is at 3873

counter is at 3874

counter is at 3875

counter is at 3876

counter is at 3877

counter is at 3878

counter is at 3879

counter is at 3880

counter is at 3881

counter is at 3882

counter is at 3883

counter is at 3884

counter is at 3885

counter is at 3886

counter is at 3887

counter is at 3888

counter is at 3889

counter is at 3890

counter is at 3891
```
```bash
[root@rocky14 c_practice]# touch scriptfile.sh

[root@rocky14 c_practice]# chmod 755 scriptfile.sh

[root@rocky14 c_practice]# vi scriptfile.sh

[root@rocky14 c_practice]# ./scriptfile.sh

checking system requirements

We can install someprogram

[root@rocky14 c_practice]# strace ./scriptfile.sh

execve("./scriptfile.sh", ["./scriptfile.sh"], 0x7fff47885010 /* 32 vars */) = 0

brk(NULL)                                                              = 0x55bc83bcd000

arch_prctl(0x3001 /* ARCH_??? */, 0x7ffc149515a0) = -1 EINVAL (Invalid argument)

access("/etc/ld.so.preload", R_OK)            = -1 ENOENT (No such file or directory)

openat(AT_FDCWD, "/etc/ld.so.cache", O_RDONLY|O_CLOEXEC) = 3

fstat(3, {st_mode=S_IFREG|0644, st_size=16027, ...}) = 0

mmap(NULL, 16027, PROT_READ, MAP_PRIVATE, 3, 0) = 0x7fa05b602000

close(3)                                                                = 0

openat(AT_FDCWD, "/lib64/libtinfo.so.6", O_RDONLY|O_CLOEXEC) = 3

read(3, "\177ELF\2\1\1\0\0\0\0\0\0\0\0\0\3\0>\0\1\0\0\0p\365\0\0\0\0\0\0"..., 832) = 832

fstat(3, {st_mode=S_IFREG|0755, st_size=195080, ...}) = 0

mmap(NULL, 8192, PROT_READ|PROT_WRITE, MAP_PRIVATE|MAP_ANONYMOUS, -1, 0) = 0x7fa05b600000

mmap(NULL, 194928, PROT_READ, MAP_PRIVATE|MAP_DENYWRITE, 3, 0) = 0x7fa05b5d0000

mmap(0x7fa05b5de000, 61440, PROT_READ|PROT_EXEC, MAP_PRIVATE|MAP_FIXED|MAP_DENYWRITE, 3, 0xe000) = 0x7fa05b5de000

mmap(0x7fa05b5ed000, 57344, PROT_READ, MAP_PRIVATE|MAP_FIXED|MAP_DENYWRITE, 3, 0x1d000) = 0x7fa05b5ed000

mmap(0x7fa05b5fb000, 20480, PROT_READ|PROT_WRITE, MAP_PRIVATE|MAP_FIXED|MAP_DENYWRITE, 3, 0x2a000) = 0x7fa05b5fb000

close(3)                                                                = 0

openat(AT_FDCWD, "/lib64/libc.so.6", O_RDONLY|O_CLOEXEC) = 3

read(3, "\177ELF\2\1\1\3\0\0\0\0\0\0\0\0\3\0>\0\1\0\0\0\220\227\2\0\0\0\0\0"..., 832) = 832

pread64(3, "\6\0\0\0\4\0\0\0@\0\0\0\0\0\0\0@\0\0\0\0\0\0\0@\0\0\0\0\0\0\0"..., 784, 64) = 784

pread64(3, "\4\0\0\0 \0\0\0\5\0\0\0GNU\0\2\0\0\300\4\0\0\0\3\0\0\0\0\0\0\0"..., 48, 848) = 48

pread64(3, "\4\0\0\0\24\0\0\0\3\0\0\0GNU\0\374F\274A\223g\0=\16N9\234\276\"\252\336"..., 68, 896) = 68

fstat(3, {st_mode=S_IFREG|0755, st_size=2539928, ...}) = 0

pread64(3, "\6\0\0\0\4\0\0\0@\0\0\0\0\0\0\0@\0\0\0\0\0\0\0@\0\0\0\0\0\0\0"..., 784, 64) = 784

mmap(NULL, 2125744, PROT_READ, MAP_PRIVATE|MAP_DENYWRITE, 3, 0) = 0x7fa05b3c9000

mmap(0x7fa05b3f1000, 1523712, PROT_READ|PROT_EXEC, MAP_PRIVATE|MAP_FIXED|MAP_DENYWRITE, 3, 0x28000) = 0x7fa05b3f1000

mmap(0x7fa05b565000, 360448, PROT_READ, MAP_PRIVATE|MAP_FIXED|MAP_DENYWRITE, 3, 0x19c000) = 0x7fa05b565000

mmap(0x7fa05b5bd000, 24576, PROT_READ|PROT_WRITE, MAP_PRIVATE|MAP_FIXED|MAP_DENYWRITE, 3, 0x1f4000) = 0x7fa05b5bd000

mmap(0x7fa05b5c3000, 53168, PROT_READ|PROT_WRITE, MAP_PRIVATE|MAP_FIXED|MAP_ANONYMOUS, -1, 0) = 0x7fa05b5c3000

close(3)                                                                = 0

mmap(NULL, 12288, PROT_READ|PROT_WRITE, MAP_PRIVATE|MAP_ANONYMOUS, -1, 0) = 0x7fa05b3c6000

arch_prctl(ARCH_SET_FS, 0x7fa05b3c6740) = 0

set_tid_address(0x7fa05b3c6a10)                  = 12990

set_robust_list(0x7fa05b3c6a20, 24)          = 0

rseq(0x7fa05b3c70e0, 0x20, 0, 0x53053053) = 0

mprotect(0x7fa05b5bd000, 16384, PROT_READ) = 0

mprotect(0x7fa05b5fb000, 16384, PROT_READ) = 0

mprotect(0x55bc82c5a000, 16384, PROT_READ) = 0

mprotect(0x7fa05b63a000, 8192, PROT_READ) = 0

prlimit64(0, RLIMIT_STACK, NULL, {rlim_cur=8192*1024, rlim_max=RLIM64_INFINITY}) = 0

munmap(0x7fa05b602000, 16027)                      = 0

openat(AT_FDCWD, "/dev/tty", O_RDWR|O_NONBLOCK) = 3

close(3)                                                                = 0

getrandom("\xc3\x24\xa8\xf1\x66\xb0\x17\x54", 8, GRND_NONBLOCK) = 8

brk(NULL)                                                              = 0x55bc83bcd000

brk(0x55bc83bee000)                                          = 0x55bc83bee000

openat(AT_FDCWD, "/usr/lib/locale/locale-archive", O_RDONLY|O_CLOEXEC) = -1 ENOENT (No such file or directory)

openat(AT_FDCWD, "/usr/share/locale/locale.alias", O_RDONLY|O_CLOEXEC) = 3

fstat(3, {st_mode=S_IFREG|0644, st_size=2998, ...}) = 0

read(3, "# Locale name alias data base.\n#"..., 4096) = 2998

read(3, "", 4096)                                              = 0

close(3)                                                                = 0

openat(AT_FDCWD, "/usr/lib/locale/C.UTF-8/LC_IDENTIFICATION", O_RDONLY|O_CLOEXEC) = -1 ENOENT (No such file or directory)

openat(AT_FDCWD, "/usr/lib/locale/C.utf8/LC_IDENTIFICATION", O_RDONLY|O_CLOEXEC) = 3

fstat(3, {st_mode=S_IFREG|0644, st_size=258, ...}) = 0

mmap(NULL, 258, PROT_READ, MAP_PRIVATE, 3, 0) = 0x7fa05b605000

close(3)                                                                = 0

openat(AT_FDCWD, "/usr/lib64/gconv/gconv-modules.cache", O_RDONLY) = 3

fstat(3, {st_mode=S_IFREG|0644, st_size=2218, ...}) = 0

mmap(NULL, 2218, PROT_READ, MAP_SHARED, 3, 0) = 0x7fa05b604000

close(3)                                                                = 0

futex(0x7fa05b5c2a6c, FUTEX_WAKE_PRIVATE, 2147483647) = 0

openat(AT_FDCWD, "/usr/lib/locale/C.UTF-8/LC_MEASUREMENT", O_RDONLY|O_CLOEXEC) = -1 ENOENT (No such file or directory)

openat(AT_FDCWD, "/usr/lib/locale/C.utf8/LC_MEASUREMENT", O_RDONLY|O_CLOEXEC) = 3

fstat(3, {st_mode=S_IFREG|0644, st_size=23, ...}) = 0

mmap(NULL, 23, PROT_READ, MAP_PRIVATE, 3, 0) = 0x7fa05b603000

close(3)                                                                = 0

openat(AT_FDCWD, "/usr/lib/locale/C.UTF-8/LC_TELEPHONE", O_RDONLY|O_CLOEXEC) = -1 ENOENT (No such file or directory)

openat(AT_FDCWD, "/usr/lib/locale/C.utf8/LC_TELEPHONE", O_RDONLY|O_CLOEXEC) = 3

fstat(3, {st_mode=S_IFREG|0644, st_size=47, ...}) = 0

mmap(NULL, 47, PROT_READ, MAP_PRIVATE, 3, 0) = 0x7fa05b602000

close(3)                                                                = 0

openat(AT_FDCWD, "/usr/lib/locale/C.UTF-8/LC_ADDRESS", O_RDONLY|O_CLOEXEC) = -1 ENOENT (No such file or directory)

openat(AT_FDCWD, "/usr/lib/locale/C.utf8/LC_ADDRESS", O_RDONLY|O_CLOEXEC) = 3

fstat(3, {st_mode=S_IFREG|0644, st_size=127, ...}) = 0

mmap(NULL, 127, PROT_READ, MAP_PRIVATE, 3, 0) = 0x7fa05b3c5000

close(3)                                                                = 0

openat(AT_FDCWD, "/usr/lib/locale/C.UTF-8/LC_NAME", O_RDONLY|O_CLOEXEC) = -1 ENOENT (No such file or directory)

openat(AT_FDCWD, "/usr/lib/locale/C.utf8/LC_NAME", O_RDONLY|O_CLOEXEC) = 3

fstat(3, {st_mode=S_IFREG|0644, st_size=62, ...}) = 0

mmap(NULL, 62, PROT_READ, MAP_PRIVATE, 3, 0) = 0x7fa05b3c4000

close(3)                                                                = 0

openat(AT_FDCWD, "/usr/lib/locale/C.UTF-8/LC_PAPER", O_RDONLY|O_CLOEXEC) = -1 ENOENT (No such file or directory)

openat(AT_FDCWD, "/usr/lib/locale/C.utf8/LC_PAPER", O_RDONLY|O_CLOEXEC) = 3

fstat(3, {st_mode=S_IFREG|0644, st_size=34, ...}) = 0

mmap(NULL, 34, PROT_READ, MAP_PRIVATE, 3, 0) = 0x7fa05b3c3000

close(3)                                                                = 0

openat(AT_FDCWD, "/usr/lib/locale/C.UTF-8/LC_MESSAGES", O_RDONLY|O_CLOEXEC) = -1 ENOENT (No such file or directory)

openat(AT_FDCWD, "/usr/lib/locale/C.utf8/LC_MESSAGES", O_RDONLY|O_CLOEXEC) = 3

fstat(3, {st_mode=S_IFDIR|0755, st_size=60, ...}) = 0

close(3)                                                                = 0

openat(AT_FDCWD, "/usr/lib/locale/C.utf8/LC_MESSAGES/SYS_LC_MESSAGES", O_RDONLY|O_CLOEXEC) = 3

fstat(3, {st_mode=S_IFREG|0644, st_size=48, ...}) = 0

mmap(NULL, 48, PROT_READ, MAP_PRIVATE, 3, 0) = 0x7fa05b3c2000

close(3)                                                                = 0

openat(AT_FDCWD, "/usr/lib/locale/C.UTF-8/LC_MONETARY", O_RDONLY|O_CLOEXEC) = -1 ENOENT (No such file or directory)

openat(AT_FDCWD, "/usr/lib/locale/C.utf8/LC_MONETARY", O_RDONLY|O_CLOEXEC) = 3

fstat(3, {st_mode=S_IFREG|0644, st_size=270, ...}) = 0

mmap(NULL, 270, PROT_READ, MAP_PRIVATE, 3, 0) = 0x7fa05b3c1000

close(3)                                                                = 0

openat(AT_FDCWD, "/usr/lib/locale/C.UTF-8/LC_COLLATE", O_RDONLY|O_CLOEXEC) = -1 ENOENT (No such file or directory)

openat(AT_FDCWD, "/usr/lib/locale/C.utf8/LC_COLLATE", O_RDONLY|O_CLOEXEC) = 3

fstat(3, {st_mode=S_IFREG|0644, st_size=1406, ...}) = 0

mmap(NULL, 1406, PROT_READ, MAP_PRIVATE, 3, 0) = 0x7fa05b3c0000

close(3)                                                                = 0

openat(AT_FDCWD, "/usr/lib/locale/C.UTF-8/LC_TIME", O_RDONLY|O_CLOEXEC) = -1 ENOENT (No such file or directory)

openat(AT_FDCWD, "/usr/lib/locale/C.utf8/LC_TIME", O_RDONLY|O_CLOEXEC) = 3

fstat(3, {st_mode=S_IFREG|0644, st_size=3360, ...}) = 0

mmap(NULL, 3360, PROT_READ, MAP_PRIVATE, 3, 0) = 0x7fa05b3bf000

close(3)                                                                = 0

openat(AT_FDCWD, "/usr/lib/locale/C.UTF-8/LC_NUMERIC", O_RDONLY|O_CLOEXEC) = -1 ENOENT (No such file or directory)

openat(AT_FDCWD, "/usr/lib/locale/C.utf8/LC_NUMERIC", O_RDONLY|O_CLOEXEC) = 3

fstat(3, {st_mode=S_IFREG|0644, st_size=50, ...}) = 0

mmap(NULL, 50, PROT_READ, MAP_PRIVATE, 3, 0) = 0x7fa05b3be000

close(3)                                                                = 0

openat(AT_FDCWD, "/usr/lib/locale/C.UTF-8/LC_CTYPE", O_RDONLY|O_CLOEXEC) = -1 ENOENT (No such file or directory)

openat(AT_FDCWD, "/usr/lib/locale/C.utf8/LC_CTYPE", O_RDONLY|O_CLOEXEC) = 3

fstat(3, {st_mode=S_IFREG|0644, st_size=346132, ...}) = 0

mmap(NULL, 346132, PROT_READ, MAP_PRIVATE, 3, 0) = 0x7fa05b369000

close(3)                                                                = 0

getuid()                                                                = 0

getgid()                                                                = 0

geteuid()                                                              = 0

getegid()                                                              = 0

rt_sigprocmask(SIG_BLOCK, NULL, [], 8)    = 0

gettimeofday({tv_sec=1747942641, tv_usec=830240}, NULL) = 0

ioctl(-1, TIOCGPGRP, 0x7ffc149513f4)        = -1 EBADF (Bad file descriptor)

sysinfo({uptime=52885, loads=[4384, 1024, 288], totalram=4081106944, freeram=1406275584, sharedram=2268094464, bufferram=0, totalswap=0, freeswap=0, procs=128, totalhigh=0, freehigh=0, mem_unit=1}) = 0

rt_sigaction(SIGCHLD, {sa_handler=SIG_DFL, sa_mask=[], sa_flags=SA_RESTORER|SA_RESTART, sa_restorer=0x7fa05b407730}, {sa_handler=SIG_DFL, sa_mask=[], sa_flags=0}, 8) = 0

rt_sigaction(SIGCHLD, {sa_handler=SIG_DFL, sa_mask=[], sa_flags=SA_RESTORER|SA_RESTART, sa_restorer=0x7fa05b407730}, {sa_handler=SIG_DFL, sa_mask=[], sa_flags=SA_RESTORER|SA_RESTART, sa_restorer=0x7fa05b407730}, 8) = 0

rt_sigaction(SIGINT, {sa_handler=SIG_DFL, sa_mask=[], sa_flags=SA_RESTORER, sa_restorer=0x7fa05b407730}, {sa_handler=SIG_DFL, sa_mask=[], sa_flags=0}, 8) = 0

rt_sigaction(SIGINT, {sa_handler=SIG_DFL, sa_mask=[], sa_flags=SA_RESTORER, sa_restorer=0x7fa05b407730}, {sa_handler=SIG_DFL, sa_mask=[], sa_flags=SA_RESTORER, sa_restorer=0x7fa05b407730}, 8) = 0

rt_sigaction(SIGQUIT, {sa_handler=SIG_DFL, sa_mask=[], sa_flags=SA_RESTORER, sa_restorer=0x7fa05b407730}, {sa_handler=SIG_DFL, sa_mask=[], sa_flags=0}, 8) = 0

rt_sigaction(SIGQUIT, {sa_handler=SIG_DFL, sa_mask=[], sa_flags=SA_RESTORER, sa_restorer=0x7fa05b407730}, {sa_handler=SIG_DFL, sa_mask=[], sa_flags=SA_RESTORER, sa_restorer=0x7fa05b407730}, 8) = 0

rt_sigaction(SIGTSTP, {sa_handler=SIG_DFL, sa_mask=[], sa_flags=SA_RESTORER, sa_restorer=0x7fa05b407730}, {sa_handler=SIG_DFL, sa_mask=[], sa_flags=0}, 8) = 0

rt_sigaction(SIGTSTP, {sa_handler=SIG_DFL, sa_mask=[], sa_flags=SA_RESTORER, sa_restorer=0x7fa05b407730}, {sa_handler=SIG_DFL, sa_mask=[], sa_flags=SA_RESTORER, sa_restorer=0x7fa05b407730}, 8) = 0

rt_sigaction(SIGTTIN, {sa_handler=SIG_DFL, sa_mask=[], sa_flags=SA_RESTORER, sa_restorer=0x7fa05b407730}, {sa_handler=SIG_DFL, sa_mask=[], sa_flags=0}, 8) = 0

rt_sigaction(SIGTTIN, {sa_handler=SIG_DFL, sa_mask=[], sa_flags=SA_RESTORER, sa_restorer=0x7fa05b407730}, {sa_handler=SIG_DFL, sa_mask=[], sa_flags=SA_RESTORER, sa_restorer=0x7fa05b407730}, 8) = 0

rt_sigaction(SIGTTOU, {sa_handler=SIG_DFL, sa_mask=[], sa_flags=SA_RESTORER, sa_restorer=0x7fa05b407730}, {sa_handler=SIG_DFL, sa_mask=[], sa_flags=0}, 8) = 0

rt_sigaction(SIGTTOU, {sa_handler=SIG_DFL, sa_mask=[], sa_flags=SA_RESTORER, sa_restorer=0x7fa05b407730}, {sa_handler=SIG_DFL, sa_mask=[], sa_flags=SA_RESTORER, sa_restorer=0x7fa05b407730}, 8) = 0

rt_sigprocmask(SIG_BLOCK, NULL, [], 8)    = 0

rt_sigaction(SIGQUIT, {sa_handler=SIG_IGN, sa_mask=[], sa_flags=SA_RESTORER, sa_restorer=0x7fa05b407730}, {sa_handler=SIG_DFL, sa_mask=[], sa_flags=SA_RESTORER, sa_restorer=0x7fa05b407730}, 8) = 0

uname({sysname="Linux", nodename="rocky14", ...}) = 0

rt_sigprocmask(SIG_BLOCK, NULL, [], 8)    = 0

newfstatat(AT_FDCWD, "/root/c_practice", {st_mode=S_IFDIR|0755, st_size=120, ...}, 0) = 0

newfstatat(AT_FDCWD, ".", {st_mode=S_IFDIR|0755, st_size=120, ...}, 0) = 0

newfstatat(AT_FDCWD, "/root", {st_mode=S_IFDIR|0755, st_size=380, ...}, 0) = 0

newfstatat(AT_FDCWD, "/root/c_practice", {st_mode=S_IFDIR|0755, st_size=120, ...}, 0) = 0

newfstatat(AT_FDCWD, "/root", {st_mode=S_IFDIR|0755, st_size=380, ...}, 0) = 0

getpid()                                                                = 12990

getppid()                                                              = 12987

gettimeofday({tv_sec=1747942641, tv_usec=839665}, NULL) = 0

getpid()                                                                = 12990

getppid()                                                              = 12987

gettimeofday({tv_sec=1747942641, tv_usec=840545}, NULL) = 0

getpid()                                                                = 12990

getppid()                                                              = 12987

getpgrp()                                                              = 12987

ioctl(2, TIOCGPGRP, [12987])                        = 0

rt_sigaction(SIGCHLD, {sa_handler=0x55bc82b74b80, sa_mask=[], sa_flags=SA_RESTORER|SA_RESTART, sa_restorer=0x7fa05b407730}, {sa_handler=SIG_DFL, sa_mask=[], sa_flags=SA_RESTORER|SA_RESTART, sa_restorer=0x7fa05b407730}, 8) = 0

prlimit64(0, RLIMIT_NPROC, NULL, {rlim_cur=15291, rlim_max=15291}) = 0

rt_sigprocmask(SIG_BLOCK, NULL, [], 8)    = 0

openat(AT_FDCWD, "./scriptfile.sh", O_RDONLY) = 3

newfstatat(AT_FDCWD, "./scriptfile.sh", {st_mode=S_IFREG|0755, st_size=291, ...}, 0) = 0

ioctl(3, TCGETS, 0x7ffc14951380)                = -1 ENOTTY (Inappropriate ioctl for device)

lseek(3, 0, SEEK_CUR)                                      = 0

read(3, "#!/bin/bash\n\necho \"checking syst"..., 80) = 80

lseek(3, 0, SEEK_SET)                                      = 0

prlimit64(0, RLIMIT_NOFILE, NULL, {rlim_cur=1024, rlim_max=512*1024}) = 0

fcntl(255, F_GETFD)                                          = -1 EBADF (Bad file descriptor)

dup2(3, 255)                                                        = 255

close(3)                                                                = 0

fcntl(255, F_SETFD, FD_CLOEXEC)                  = 0

fcntl(255, F_GETFL)                                          = 0x8000 (flags O_RDONLY|O_LARGEFILE)

fstat(255, {st_mode=S_IFREG|0755, st_size=291, ...}) = 0

lseek(255, 0, SEEK_CUR)                                  = 0

read(255, "#!/bin/bash\n\necho \"checking syst"..., 291) = 291

fstat(1, {st_mode=S_IFCHR|0620, st_rdev=makedev(0x88, 0), ...}) = 0

write(1, "checking system requirements\n", 29checking system requirements

) = 29

rt_sigprocmask(SIG_BLOCK, [CHLD], [], 8) = 0

pipe([3, 4])                                                        = 0

rt_sigprocmask(SIG_BLOCK, NULL, [CHLD], 8) = 0

rt_sigprocmask(SIG_BLOCK, [INT TERM CHLD], [CHLD], 8) = 0

lseek(255, -207, SEEK_CUR)                            = 84

clone(child_stack=NULL, flags=CLONE_CHILD_CLEARTID|CLONE_CHILD_SETTID|SIGCHLD, child_tidptr=0x7fa05b3c6a10) = 12991

rt_sigprocmask(SIG_SETMASK, [CHLD], NULL, 8) = 0

close(4)                                                                = 0

close(4)                                                                = -1 EBADF (Bad file descriptor)

rt_sigprocmask(SIG_BLOCK, NULL, [CHLD], 8) = 0

rt_sigprocmask(SIG_BLOCK, [INT TERM CHLD], [CHLD], 8) = 0

clone(child_stack=NULL, flags=CLONE_CHILD_CLEARTID|CLONE_CHILD_SETTID|SIGCHLD, child_tidptr=0x7fa05b3c6a10) = 12992

rt_sigprocmask(SIG_SETMASK, [CHLD], NULL, 8) = 0

close(3)                                                                = 0

rt_sigprocmask(SIG_BLOCK, [CHLD], [CHLD], 8) = 0

rt_sigprocmask(SIG_SETMASK, [CHLD], NULL, 8) = 0

rt_sigprocmask(SIG_BLOCK, [CHLD], [CHLD], 8) = 0

rt_sigaction(SIGINT, {sa_handler=0x55bc82b76fe0, sa_mask=[], sa_flags=SA_RESTORER, sa_restorer=0x7fa05b407730}, {sa_handler=SIG_DFL, sa_mask=[], sa_flags=SA_RESTORER, sa_restorer=0x7fa05b407730}, 8) = 0

wait4(-1, [{WIFEXITED(s) && WEXITSTATUS(s) == 0}], 0, NULL) = 12991

wait4(-1, [{WIFEXITED(s) && WEXITSTATUS(s) == 0}], 0, NULL) = 12992

rt_sigaction(SIGINT, {sa_handler=SIG_DFL, sa_mask=[], sa_flags=SA_RESTORER, sa_restorer=0x7fa05b407730}, {sa_handler=0x55bc82b76fe0, sa_mask=[], sa_flags=SA_RESTORER, sa_restorer=0x7fa05b407730}, 8) = 0

ioctl(2, TIOCGWINSZ, {ws_row=60, ws_col=206, ws_xpixel=0, ws_ypixel=0}) = 0

ioctl(1, TCGETS, {B38400 opost isig icanon echo ...}) = 0

newfstatat(AT_FDCWD, "/root/.terminfo", 0x55bc83be42c0, 0) = -1 ENOENT (No such file or directory)

newfstatat(AT_FDCWD, "/etc/terminfo", {st_mode=S_IFDIR|0755, st_size=40, ...}, 0) = 0

newfstatat(AT_FDCWD, "/usr/share/terminfo", {st_mode=S_IFDIR|0755, st_size=460, ...}, 0) = 0

access("/etc/terminfo/x/xterm", R_OK)      = -1 ENOENT (No such file or directory)

access("/usr/share/terminfo/x/xterm", R_OK) = 0

openat(AT_FDCWD, "/usr/share/terminfo/x/xterm", O_RDONLY) = 3

fstat(3, {st_mode=S_IFREG|0644, st_size=3720, ...}) = 0

read(3, "\32\0010\0&\0\17\0\235\1\351\5xterm|xterm terminal"..., 32768) = 3720

read(3, "", 28672)                                            = 0

close(3)                                                                = 0

ioctl(1, TCGETS, {B38400 opost isig icanon echo ...}) = 0

ioctl(1, TCGETS, {B38400 opost isig icanon echo ...}) = 0

ioctl(1, TCGETS, {B38400 opost isig icanon echo ...}) = 0

ioctl(1, TCGETS, {B38400 opost isig icanon echo ...}) = 0

ioctl(1, TIOCGWINSZ, {ws_row=60, ws_col=206, ws_xpixel=0, ws_ypixel=0}) = 0

ioctl(0, TIOCGWINSZ, {ws_row=60, ws_col=206, ws_xpixel=0, ws_ypixel=0}) = 0

brk(0x55bc83c0f000)                                          = 0x55bc83c0f000

rt_sigprocmask(SIG_SETMASK, [CHLD], NULL, 8) = 0

close(3)                                                                = -1 EBADF (Bad file descriptor)

rt_sigprocmask(SIG_SETMASK, [], NULL, 8) = 0

--- SIGCHLD {si_signo=SIGCHLD, si_code=CLD_EXITED, si_pid=12992, si_uid=0, si_status=0, si_utime=0, si_stime=0} ---

wait4(-1, 0x7ffc14950a50, WNOHANG, NULL) = -1 ECHILD (No child processes)

rt_sigreturn({mask=[]})                                  = 0

read(255, "gccCheck=$?\n\nrpm -qa | grep -i s"..., 291) = 207

rt_sigprocmask(SIG_BLOCK, [CHLD], [], 8) = 0

pipe([3, 4])                                                        = 0

rt_sigprocmask(SIG_BLOCK, NULL, [CHLD], 8) = 0

rt_sigprocmask(SIG_BLOCK, [INT TERM CHLD], [CHLD], 8) = 0

lseek(255, -151, SEEK_CUR)                            = 140

clone(child_stack=NULL, flags=CLONE_CHILD_CLEARTID|CLONE_CHILD_SETTID|SIGCHLD, child_tidptr=0x7fa05b3c6a10) = 12994

rt_sigprocmask(SIG_SETMASK, [CHLD], NULL, 8) = 0

close(4)                                                                = 0

close(4)                                                                = -1 EBADF (Bad file descriptor)

rt_sigprocmask(SIG_BLOCK, NULL, [CHLD], 8) = 0

rt_sigprocmask(SIG_BLOCK, [INT TERM CHLD], [CHLD], 8) = 0

clone(child_stack=NULL, flags=CLONE_CHILD_CLEARTID|CLONE_CHILD_SETTID|SIGCHLD, child_tidptr=0x7fa05b3c6a10) = 12995

rt_sigprocmask(SIG_SETMASK, [CHLD], NULL, 8) = 0

close(3)                                                                = 0

rt_sigprocmask(SIG_BLOCK, [CHLD], [CHLD], 8) = 0

rt_sigprocmask(SIG_SETMASK, [CHLD], NULL, 8) = 0

rt_sigprocmask(SIG_BLOCK, [CHLD], [CHLD], 8) = 0

rt_sigaction(SIGINT, {sa_handler=0x55bc82b76fe0, sa_mask=[], sa_flags=SA_RESTORER, sa_restorer=0x7fa05b407730}, {sa_handler=SIG_DFL, sa_mask=[], sa_flags=SA_RESTORER, sa_restorer=0x7fa05b407730}, 8) = 0

wait4(-1, [{WIFEXITED(s) && WEXITSTATUS(s) == 0}], 0, NULL) = 12994

wait4(-1, [{WIFEXITED(s) && WEXITSTATUS(s) == 1}], 0, NULL) = 12995

rt_sigaction(SIGINT, {sa_handler=SIG_DFL, sa_mask=[], sa_flags=SA_RESTORER, sa_restorer=0x7fa05b407730}, {sa_handler=0x55bc82b76fe0, sa_mask=[], sa_flags=SA_RESTORER, sa_restorer=0x7fa05b407730}, 8) = 0

ioctl(2, TIOCGWINSZ, {ws_row=60, ws_col=206, ws_xpixel=0, ws_ypixel=0}) = 0

rt_sigprocmask(SIG_SETMASK, [CHLD], NULL, 8) = 0

close(3)                                                                = -1 EBADF (Bad file descriptor)

rt_sigprocmask(SIG_SETMASK, [], NULL, 8) = 0

--- SIGCHLD {si_signo=SIGCHLD, si_code=CLD_EXITED, si_pid=12994, si_uid=0, si_status=0, si_utime=105, si_stime=5} ---

wait4(-1, 0x7ffc14950a50, WNOHANG, NULL) = -1 ECHILD (No child processes)

rt_sigreturn({mask=[]})                                  = 0

read(255, "superCheck=$?\n\nif [ $gccCheck -e"..., 291) = 151

write(1, "We can install someprogram\n", 27We can install someprogram

) = 27

read(255, "", 291)                                            = 0

rt_sigprocmask(SIG_BLOCK, [CHLD], [], 8) = 0

rt_sigprocmask(SIG_SETMASK, [], NULL, 8) = 0

exit_group(0)                                                      = ?

+++ exited with 0 +++
```

