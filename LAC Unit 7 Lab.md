```bash
[root@rocky14 ~]# rpm -qi systemd

Name                : systemd

Version          : 252

Release          : 46.el9_5.2.0.1

Architecture: x86_64

Install Date: Mon Feb 10 18:36:58 2025

Group              : Unspecified

Size                : 12864308

License          : LGPLv2+ and MIT and GPLv2+

Signature      : RSA/SHA256, Fri Nov 15 18:27:06 2024, Key ID 702d426d350d275d

Source RPM    : systemd-252-46.el9_5.2.0.1.src.rpm

Build Date    : Fri Nov 15 18:18:17 2024

Build Host    : pb-7cdab3d7-2cf4-4e0b-b1ed-bf89e9226511-b-x86-64

Packager        : Rocky Linux Build System (Peridot) <releng@rockylinux.org>

Vendor            : Rocky Enterprise Software Foundation

URL                  : https://systemd.io

Summary          : System and Service Manager

Description :

systemd is a system and service manager that runs as PID 1 and starts

the rest of the system. It provides aggressive parallelization

capabilities, uses socket and D-Bus activation for starting services,

offers on-demand starting of daemons, keeps track of processes using

Linux control groups, maintains mount and automount points, and

implements an elaborate transactional dependency-based service control

logic. systemd supports SysV and LSB init scripts and works as a

replacement for sysvinit. Other parts of this package are a logging daemon,

utilities to control basic system configuration like the hostname,

date, locale, maintain a list of logged-in users, system accounts,

runtime directories and settings, and daemons to manage simple network

configuration, network time synchronization, log forwarding, and name

resolution.

[root@rocky14 ~]# rpm -q systemd

systemd-252-46.el9_5.2.0.1.x86_64

[root@rocky14 ~]# rpm -qa

libreport-filesystem-2.15.2-6.el9.rocky.0.2.noarch

ncurses-base-6.2-10.20210508.el9.noarch

ncurses-libs-6.2-10.20210508.el9.x86_64

zlib-1.2.11-40.el9.x86_64

xz-libs-5.2.5-8.el9_0.x86_64

libzstd-1.5.1-2.el9.x86_64

libxcrypt-4.4.18-3.el9.x86_64

popt-1.18-8.el9.x86_64

libcap-2.48-9.el9_2.x86_64

libgpg-error-1.42-5.el9.x86_64

readline-8.1-4.el9.x86_64

lua-libs-5.4.4-4.el9.x86_64

libattr-2.5.1-3.el9.x86_64

libffi-3.4.2-8.el9.x86_64

libassuan-2.5.5-3.el9.x86_64

lz4-libs-1.9.3-5.el9.x86_64

libcap-ng-0.8.2-7.el9.x86_64

libsigsegv-2.13-4.el9.x86_64

libunistring-0.9.10-15.el9.x86_64

gmp-6.2.0-13.el9.x86_64

libtasn1-4.16.0-8.el9_1.x86_64

grep-3.6-5.el9.x86_64

json-c-0.14-11.el9.x86_64

keyutils-libs-1.6.3-1.el9.x86_64

mpfr-4.1.0-7.el9.x86_64

gawk-5.1.0-6.el9.x86_64

libidn2-2.3.0-7.el9.x86_64

libcomps-0.1.18-1.el9.x86_64

libverto-0.3.2-3.el9.x86_64

npth-1.6-8.el9.x86_64

libyaml-0.2.5-7.el9.x86_64

sed-4.8-9.el9.x86_64

cyrus-sasl-lib-2.1.27-21.el9.x86_64

libmodulemd-2.13.0-2.el9.x86_64

gnupg2-2.3.3-4.el9.x86_64

gpgme-1.15.1-6.el9.x86_64

python3-libcomps-0.1.18-1.el9.x86_64

python3-gpg-1.15.1-6.el9.x86_64

gzip-1.12-1.el9.x86_64

cracklib-2.9.6-27.el9.x86_64

cracklib-dicts-2.9.6-27.el9.x86_64

libpwquality-1.4.4-8.el9.x86_64

passwd-0.80-12.el9.x86_64

libutempter-1.2.1-6.el9.x86_64

libusbx-1.0.26-1.el9.x86_64

hostname-3.23-6.el9.x86_64

rootfiles-8.1-31.el9.noarch

gpg-pubkey-350d275d-6279464b

setup-2.13.7-10.el9.noarch

basesystem-11-13.el9.0.1.noarch

bash-5.1.8-9.el9.x86_64

libacl-2.3.1-4.el9.x86_64

sqlite-libs-3.34.1-7.el9_3.x86_64

libxml2-2.9.13-6.el9_4.x86_64

libsepol-3.6-1.el9.x86_64

libarchive-3.5.3-4.el9.0.1.x86_64

libxcrypt-compat-4.4.18-3.el9.x86_64

file-libs-5.39-16.el9.x86_64

libcom_err-1.46.5-5.el9.x86_64

nettle-3.9.1-1.el9.x86_64

gnutls-3.8.3-4.el9_4.x86_64

libselinux-3.6-1.el9.x86_64

librepo-1.14.5-2.el9.x86_64

openldap-2.6.6-3.el9.x86_64

libref_array-0.1.5-53.el9.x86_64

e2fsprogs-libs-1.46.5-5.el9.x86_64

procps-ng-3.3.17-14.el9.x86_64

libfastjson-0.99.9-5.el9.x86_64

libestr-0.1.11-4.el9.x86_64

geolite2-city-20191217-6.el9.noarch

geolite2-country-20191217-6.el9.noarch

ipcalc-1.0.0-5.el9.x86_64

keyutils-1.6.3-1.el9.x86_64

dhcp-common-4.4.2-19.b1.el9.noarch

libbasicobjects-0.1.1-53.el9.x86_64

libcollection-0.7.0-53.el9.x86_64

libpath_utils-0.2.1-53.el9.x86_64

libini_config-1.3.1-53.el9.x86_64

libcbor-0.7.0-5.el9.x86_64

pciutils-libs-3.7.0-5.el9.x86_64

libselinux-utils-3.6-1.el9.x86_64

libss-1.46.5-5.el9.x86_64

libseccomp-2.5.2-2.el9.x86_64

libedit-3.1-38.20210216cvs.el9.x86_64

diffutils-3.7-12.el9.x86_64

policycoreutils-3.6-2.1.el9.x86_64

xz-5.2.5-8.el9_0.x86_64

psmisc-23.4-3.el9.x86_64

libverto-libev-0.3.2-3.el9.x86_64

cpio-2.13-16.el9.x86_64

pigz-2.5-4.el9.x86_64

iproute-6.2.0-6.el9_4.x86_64

python3-pyyaml-5.4.1-6.el9.x86_64

publicsuffix-list-dafsa-20210518-3.el9.noarch

libpsl-0.21.1-5.el9.x86_64

acl-2.3.1-4.el9.x86_64

dbus-1.12.20-8.el9.x86_64

dbus-common-1.12.20-8.el9.noarch

dbus-broker-28-7.el9.x86_64

rpcbind-1.2.6-7.el9.x86_64

logrotate-3.18.0-8.el9.x86_64

rsyslog-logrotate-8.2310.0-4.el9.x86_64

rsyslog-8.2310.0-4.el9.x86_64

libkcapi-1.4.0-2.el9.x86_64

libkcapi-hmaccalc-1.4.0-2.el9.x86_64

libfido2-1.13.0-2.el9.x86_64

kernel-modules-core-5.14.0-427.18.1.el9_4.x86_64

kernel-core-5.14.0-427.18.1.el9_4.x86_64

pciutils-3.7.0-5.el9.x86_64

kernel-modules-5.14.0-427.18.1.el9_4.x86_64

dhcp-client-4.4.2-19.b1.el9.x86_64

ipmitool-1.8.18-27.el9.x86_64

e2fsprogs-1.46.5-5.el9.x86_64

ethtool-6.2-1.el9.x86_64

strace-5.18-2.el9.x86_64

which-2.21-29.el9.x86_64

words-3.0-39.el9.noarch

parted-3.5-2.el9.x86_64

libblockdev-utils-2.28-10.el9.x86_64

gdisk-1.0.7-5.el9.x86_64

shared-mime-info-2.1-5.el9.x86_64

libgudev-237-1.el9.x86_64

json-glib-1.6.6-1.el9.x86_64

file-5.39-16.el9.x86_64

libjcat-0.1.6-3.el9.x86_64

libxmlb-0.3.10-1.el9.x86_64

libblockdev-part-2.28-10.el9.x86_64

libblockdev-swap-2.28-10.el9.x86_64

libblockdev-loop-2.28-10.el9.x86_64

libblockdev-fs-2.28-10.el9.x86_64

libblockdev-2.28-10.el9.x86_64

polkit-pkla-compat-0.1-21.el9.x86_64

volume_key-libs-0.3.12-15.el9.x86_64

libblockdev-crypto-2.28-10.el9.x86_64

libatasmart-0.19-22.el9.x86_64

userspace-rcu-0.12.1-6.el9.x86_64

gettext-libs-0.21-8.el9.x86_64

gettext-0.21-8.el9.x86_64

inih-49-6.el9.x86_64

libgusb-0.3.8-2.el9.x86_64

libblockdev-mdraid-2.28-10.el9.x86_64

dosfstools-4.2-3.el9.x86_64

flashrom-1.2-10.el9.x86_64

fwupd-plugin-flashrom-1.9.13-2.el9.x86_64

fwupd-1.9.13-2.el9.x86_64

efi-filesystem-6-2.el9_0.noarch

efivar-libs-38-3.el9.x86_64

mokutil-0.6.0-4.el9.x86_64

shim-x64-15.8-2.el9.x86_64

warewulf-dracut-4.5.5-1.el9.noarch

protobuf-c-1.3.3-13.el9.x86_64

lmdb-libs-0.9.29-3.el9.x86_64

fstrm-0.6.1-3.el9.x86_64

dbus-libs-1.12.20-8.el9.x86_64

python3-dbus-1.2.18-2.el9.0.1.x86_64

python3-six-1.15.0-9.el9.noarch

python3-dateutil-2.8.1-7.el9.noarch

gpg-pubkey-3228467c-613798eb

sshpass-1.09-4.el9.x86_64

python3-resolvelib-0.5.4-5.el9.noarch

python3-ply-3.11-14.el9.0.1.noarch

python3-pycparser-2.20-6.el9.noarch

python3-cffi-1.14.5-5.el9.x86_64

python3-cryptography-36.0.1-4.el9.x86_64

python3-pyparsing-2.4.7-9.el9.noarch

python3-packaging-20.9-5.el9.noarch

ansible-7.7.0-1.el9.noarch

libaio-0.3.111-13.el9.x86_64

device-mapper-persistent-data-1.0.9-3.el9_4.x86_64

ncurses-6.2-10.20210508.el9.x86_64

groff-base-1.22.4-10.el9.x86_64

perl-Digest-1.19-4.el9.noarch

perl-Digest-MD5-2.58-4.el9.x86_64

perl-B-1.80-481.el9.x86_64

perl-FileHandle-2.03-481.el9.noarch

perl-Data-Dumper-2.174-462.el9.x86_64

perl-libnet-3.13-4.el9.noarch

perl-base-2.27-481.el9.noarch

perl-AutoLoader-5.74-481.el9.noarch

perl-URI-5.09-3.el9.noarch

perl-Mozilla-CA-20200520-6.el9.noarch

perl-Text-Tabs+Wrap-2013.0523-460.el9.noarch

perl-Pod-Escapes-1.07-460.el9.noarch

perl-if-0.60.800-481.el9.noarch

perl-File-Path-2.18-4.el9.noarch

perl-IO-Socket-IP-0.41-5.el9.noarch

perl-Time-Local-1.300-7.el9.noarch

perl-Term-ANSIColor-5.01-461.el9.noarch

perl-POSIX-1.94-481.el9.x86_64

perl-Term-Cap-1.17-460.el9.noarch

perl-subs-1.03-481.el9.noarch

perl-Pod-Simple-3.42-4.el9.noarch

perl-IPC-Open3-1.21-481.el9.noarch

perl-Class-Struct-0.66-481.el9.noarch

perl-HTTP-Tiny-0.076-462.el9.noarch

perl-File-Temp-0.231.100-4.el9.noarch

perl-Socket-2.031-4.el9.x86_64

perl-Symbol-1.08-481.el9.noarch

perl-SelectSaver-1.02-481.el9.noarch

perl-File-stat-1.09-481.el9.noarch

perl-podlators-4.14-460.el9.noarch

perl-Pod-Perldoc-3.28.01-461.el9.noarch

perl-Text-ParseWords-3.30-460.el9.noarch

perl-mro-1.23-481.el9.x86_64

perl-Fcntl-1.13-481.el9.x86_64

perl-overloading-0.02-481.el9.noarch

perl-IO-1.43-481.el9.x86_64

perl-Pod-Usage-2.01-4.el9.noarch

perl-constant-1.33-461.el9.noarch

perl-MIME-Base64-3.16-4.el9.x86_64

perl-Errno-1.30-481.el9.x86_64

perl-vars-1.05-481.el9.noarch

perl-overload-1.31-481.el9.noarch

perl-Getopt-Std-1.12-481.el9.noarch

perl-File-Basename-2.85-481.el9.noarch

perl-Storable-3.21-460.el9.x86_64

perl-parent-0.238-460.el9.noarch

perl-Getopt-Long-2.52-4.el9.noarch

perl-Exporter-5.74-461.el9.noarch

perl-Carp-1.50-460.el9.noarch

perl-NDBM_File-1.15-481.el9.x86_64

perl-PathTools-3.78-461.el9.x86_64

perl-Encode-3.08-462.el9.x86_64

perl-libs-5.32.1-481.el9.x86_64

perl-interpreter-5.32.1-481.el9.x86_64

perl-File-Find-1.37-481.el9.noarch

cowsay-3.7.0-10.el9.noarch

libpng-1.6.37-12.el9.x86_64

graphite2-1.3.14-9.el9.x86_64

harfbuzz-2.7.4-10.el9.x86_64

freetype-2.10.4-9.el9.x86_64

gpm-libs-1.20.7-29.el9.x86_64

libpipeline-1.5.3-4.el9.x86_64

man-db-2.9.3-7.el9.x86_64

python3-setools-4.4.4-1.el9.x86_64

setools-console-4.4.4-1.el9.x86_64

python3-libselinux-3.6-1.el9.x86_64

checkpolicy-3.6-1.el9.x86_64

python3-distro-1.5.0-7.el9.noarch

python3-policycoreutils-3.6-2.1.el9.noarch

policycoreutils-python-utils-3.6-2.1.el9.noarch

make-4.3-8.el9.x86_64

m4-1.4.19-1.el9.x86_64

policycoreutils-devel-3.6-2.1.el9.x86_64

lsof-4.94.0-3.el9.x86_64

lm_sensors-libs-3.6.0-10.el9.x86_64

libnl3-3.9.0-1.el9.x86_64

libpcap-1.10.0-4.el9.x86_64

libnftnl-1.2.6-4.el9_4.x86_64

libcap-ng-python3-0.8.2-7.el9.x86_64

gobject-introspection-1.68.0-11.el9.x86_64

python3-gobject-base-noarch-3.40.1-6.el9.noarch

python3-gobject-base-3.40.1-6.el9.x86_64

jansson-2.14-1.el9.x86_64

libnetfilter_conntrack-1.0.9-1.el9.x86_64

glib2-2.68.4-14.el9_4.1.x86_64

libuv-1.42.0-2.el9_4.x86_64

ca-certificates-2024.2.69_v8.0.303-91.4.el9_4.noarch

libevent-2.1.12-8.el9_4.x86_64

kernel-core-5.14.0-427.42.1.el9_4.x86_64

kernel-modules-core-5.14.0-427.42.1.el9_4.x86_64

kernel-modules-5.14.0-427.42.1.el9_4.x86_64

libmnl-1.0.4-16.el9_4.x86_64

wget-1.21.1-8.el9_4.x86_64

criu-3.19-1.el9.x86_64

criu-libs-3.19-1.el9.x86_64

yajl-2.1.0-22.el9.x86_64

lksctp-tools-1.0.19-3.el9_4.x86_64

libgcc-11.5.0-2.el9.x86_64

crypto-policies-20240828-2.git626aa59.el9_5.noarch

filesystem-3.16-5.el9.x86_64

tzdata-2025a-1.el9.noarch

glibc-minimal-langpack-2.34-125.el9_5.1.x86_64

glibc-2.34-125.el9_5.1.x86_64

glibc-common-2.34-125.el9_5.1.x86_64

openssl-libs-3.2.2-6.el9_5.x86_64

audit-libs-3.1.5-1.el9.x86_64

bzip2-libs-1.0.8-10.el9_5.x86_64

libuuid-2.37.4-20.el9.x86_64

libstdc++-11.5.0-2.el9.x86_64

kmod-28-10.el9.x86_64

alternatives-1.24-1.el9_5.1.x86_64

p11-kit-0.25.3-3.el9_5.x86_64

nspr-4.35.0-17.el9_5.x86_64

nss-util-3.101.0-10.el9_5.x86_64

expat-2.5.0-3.el9_5.1.x86_64

findutils-4.8.0-7.el9.x86_64

elfutils-libelf-0.191-4.el9.x86_64

libsmartcols-2.37.4-20.el9.x86_64

libsemanage-3.6-2.1.el9_5.x86_64

shadow-utils-4.9-10.el9_5.x86_64

kmod-libs-28-10.el9.x86_64

iptables-libs-1.8.10-11.el9_5.x86_64

nftables-1.0.9-3.el9.x86_64

libgcrypt-1.10.0-11.el9.x86_64

fuse3-libs-3.10.2-9.el9.x86_64

shadow-utils-subid-4.9-10.el9_5.x86_64

nss-softokn-freebl-3.101.0-10.el9_5.x86_64

nss-softokn-3.101.0-10.el9_5.x86_64

p11-kit-trust-0.25.3-3.el9_5.x86_64

nmap-ncat-7.92-3.el9.x86_64

perl-Net-SSLeay-1.94-1.el9.x86_64

attr-2.5.1-3.el9.x86_64

avahi-libs-0.8-21.el9.x86_64

chkconfig-1.24-1.el9_5.1.x86_64

libdb-5.3.28-54.el9.x86_64

libndp-1.9-1.el9.x86_64

fuse-libs-2.9.9-16.el9.x86_64

libnghttp2-1.43.0-6.el9.x86_64

less-590-5.el9.x86_64

gdbm-libs-1.23-1.el9.x86_64

ipset-libs-7.11-11.el9_5.x86_64

ipset-7.11-11.el9_5.x86_64

pcre-8.44-4.el9.x86_64

libgomp-11.5.0-2.el9.x86_64

libeconf-0.4.1-4.el9.x86_64

oniguruma-6.9.6-1.el9.6.x86_64

jq-1.6-17.el9.x86_64

libudisks2-2.9.4-11.el9.x86_64

libslirp-4.4.0-8.el9.x86_64

slirp4netns-1.3.1-1.el9.x86_64

libmaxminddb-1.5.2-4.el9.x86_64

aardvark-dns-1.12.2-1.el9_5.x86_64

netavark-1.12.2-1.el9.x86_64

pcp-conf-6.2.2-7.el9_5.x86_64

bind-license-9.16.23-24.el9_5.noarch

rocky-gpg-keys-9.5-1.2.el9.noarch

rocky-release-9.5-1.2.el9.noarch

rocky-repos-9.5-1.2.el9.noarch

kbd-legacy-2.4.0-10.el9.noarch

fuse-common-3.10.2-9.el9.x86_64

fuse3-3.10.2-9.el9.x86_64

fuse-overlayfs-1.14-1.el9.x86_64

vim-filesystem-8.2.2637-21.el9.noarch

vim-common-8.2.2637-21.el9.x86_64

systemd-rpm-macros-252-46.el9_5.2.0.1.noarch

coreutils-common-8.32-36.el9.x86_64

coreutils-8.32-36.el9.x86_64

systemd-libs-252-46.el9_5.2.0.1.x86_64

libblkid-2.37.4-20.el9.x86_64

krb5-libs-1.21.1-4.el9_5.x86_64

libcurl-minimal-7.76.1-31.el9.x86_64

libmount-2.37.4-20.el9.x86_64

util-linux-core-2.37.4-20.el9.x86_64

libfdisk-2.37.4-20.el9.x86_64

tpm2-tss-3.2.3-1.el9.x86_64

libtirpc-1.3.3-9.el9.x86_64

polkit-libs-0.117-13.el9.x86_64

crun-1.16.1-1.el9.x86_64

selinux-policy-38.1.45-3.el9_5.noarch

selinux-policy-targeted-38.1.45-3.el9_5.noarch

container-selinux-2.232.1-1.el9.noarch

iptables-nft-1.8.10-11.el9_5.x86_64

containers-common-1-96.el9_5.x86_64

passt-0^20240806.gee36266-6.el9_5.x86_64

passt-selinux-0^20240806.gee36266-6.el9_5.noarch

ima-evm-utils-1.5-2.el9.0.1.x86_64

curl-minimal-7.76.1-31.el9.x86_64

rpm-libs-4.16.1.3-34.el9.0.1.x86_64

rpm-4.16.1.3-34.el9.0.1.x86_64

libsolv-0.7.24-3.el9.x86_64

libdnf-0.69.0-12.el9.x86_64

rpm-plugin-systemd-inhibit-4.16.1.3-34.el9.0.1.x86_64

rpm-sign-libs-4.16.1.3-34.el9.0.1.x86_64

libnfsidmap-2.5.4-27.el9.x86_64

bind-libs-9.16.23-24.el9_5.x86_64

NetworkManager-libnm-1.48.10-5.el9_5.x86_64

conmon-2.1.12-1.el9.x86_64

pcp-libs-6.2.2-7.el9_5.x86_64

openssl-3.2.2-6.el9_5.x86_64

pam-1.5.1-22.el9_5.x86_64

util-linux-2.37.4-20.el9.x86_64

grub2-common-2.06-93.el9_5.noarch

openssh-8.7p1-43.el9.x86_64

openssh-clients-8.7p1-43.el9.x86_64

grub2-pc-modules-2.06-93.el9_5.noarch

libuser-0.63-15.el9.x86_64

initscripts-rename-device-10.11.7-1.el9.x86_64

linux-firmware-whence-20250114-146.3.el9_5.noarch

linux-firmware-20250114-146.3.el9_5.noarch

python3-setuptools-wheel-53.0.0-13.el9.noarch

pcre2-syntax-10.40-6.el9.noarch

pcre2-10.40-6.el9.x86_64

systemd-pam-252-46.el9_5.2.0.1.x86_64

systemd-252-46.el9_5.2.0.1.x86_64

initscripts-service-10.11.7-1.el9.noarch

device-mapper-libs-1.02.198-2.el9.x86_64

device-mapper-1.02.198-2.el9.x86_64

grub2-tools-minimal-2.06-93.el9_5.x86_64

device-mapper-event-libs-1.02.198-2.el9.x86_64

device-mapper-event-1.02.198-2.el9.x86_64

lvm2-libs-2.03.24-2.el9.x86_64

cryptsetup-libs-2.7.2-3.el9_5.x86_64

kpartx-0.8.7-32.el9.x86_64

xfsprogs-6.4.0-4.el9.x86_64

iputils-20210202-10.el9_5.x86_64

polkit-0.117-13.el9.x86_64

elfutils-default-yama-scope-0.191-4.el9.noarch

elfutils-libs-0.191-4.el9.x86_64

elfutils-debuginfod-client-0.191-4.el9.x86_64

binutils-gold-2.35.2-54.el9.x86_64

binutils-2.35.2-54.el9.x86_64

rpm-build-libs-4.16.1.3-34.el9.0.1.x86_64

gssproxy-0.8.4-7.el9.x86_64

git-core-2.43.5-2.el9_5.x86_64

quota-nls-4.09-2.el9.noarch

quota-4.09-2.el9.x86_64

python3-pip-wheel-21.3.1-1.el9.noarch

python3-3.9.21-1.el9_5.x86_64

python3-libs-3.9.21-1.el9_5.x86_64

python3-libdnf-0.69.0-12.el9.x86_64

python3-hawkey-0.69.0-12.el9.x86_64

python3-rpm-4.16.1.3-34.el9.0.1.x86_64

python3-setuptools-53.0.0-13.el9.noarch

python3-systemd-234-19.el9.x86_64

python3-nftables-1.0.9-3.el9.x86_64

python3-firewall-1.3.4-9.el9_5.noarch

kbd-misc-2.4.0-10.el9.noarch

kbd-2.4.0-10.el9.x86_64

systemd-udev-252-46.el9_5.2.0.1.x86_64

dracut-057-70.git20240819.el9.x86_64

os-prober-1.77-12.el9_5.x86_64

grub2-tools-2.06-93.el9_5.x86_64

kernel-core-5.14.0-503.23.1.el9_5.x86_64

kernel-modules-core-5.14.0-503.23.1.el9_5.x86_64

grubby-8.40-64.el9.x86_64

crypto-policies-scripts-20240828-2.git626aa59.el9_5.noarch

nss-sysinit-3.101.0-10.el9_5.x86_64

nss-3.101.0-10.el9_5.x86_64

NetworkManager-1.48.10-5.el9_5.x86_64

firewalld-filesystem-1.3.4-9.el9_5.noarch

dnf-data-4.14.0-17.el9.noarch

python3-dnf-4.14.0-17.el9.noarch

dnf-4.14.0-17.el9.noarch

python3-dnf-plugins-core-4.3.0-16.el9.noarch

dnf-plugins-core-4.3.0-16.el9.noarch

epel-release-9-9.el9.noarch

yum-4.14.0-17.el9.noarch

firewalld-1.3.4-9.el9_5.noarch

dracut-network-057-70.git20240819.el9.x86_64

kernel-modules-5.14.0-503.23.1.el9_5.x86_64

grub2-pc-2.06-93.el9_5.x86_64

grub2-tools-extra-2.06-93.el9_5.x86_64

grub2-tools-efi-2.06-93.el9_5.x86_64

udisks2-2.9.4-11.el9.x86_64

ansible-core-2.14.17-1.el9.x86_64

vim-enhanced-8.2.2637-21.el9.x86_64

nfs-utils-2.5.4-27.el9.x86_64

python3-audit-3.1.5-1.el9.x86_64

python3-libsemanage-3.6-2.1.el9_5.x86_64

lvm2-2.03.24-2.el9.x86_64

audit-3.1.5-1.el9.x86_64

initscripts-10.11.7-1.el9.x86_64

mdadm-4.3-3.el9.x86_64

net-tools-2.0-0.64.20160912git.el9.x86_64

openssh-server-8.7p1-43.el9.x86_64

sysstat-12.5.4-9.el9.x86_64

libbytesize-2.5-3.el9.0.1.x86_64

usermode-1.114-5.el9.x86_64

podman-5.2.2-13.el9_5.x86_64

bind-utils-9.16.23-24.el9_5.x86_64

rpm-plugin-selinux-4.16.1.3-34.el9.0.1.x86_64

selinux-policy-devel-38.1.45-3.el9_5.noarch

nmap-7.92-3.el9.x86_64

perl-IO-Socket-SSL-2.073-2.el9.noarch

libbpf-1.4.0-1.el9.x86_64

unzip-6.0-57.el9.x86_64

rsync-3.2.3-20.el9_5.1.x86_64

iperf3-3.9-13.el9_5.1.x86_64

libbrotli-1.0.9-7.el9_5.x86_64

libibverbs-51.0-1.el9.x86_64

dmidecode-3.6-1.el9.x86_64

libnfnetlink-1.0.1-23.el9_5.x86_64

libev-4.33-5.el9.0.1.x86_64

libksba-1.5.1-7.el9.x86_64

tar-1.34-7.el9.x86_64

vim-minimal-8.2.2637-21.el9.x86_64

perl-Scalar-List-Utils-1.56-462.el9.x86_64

libnet-1.2-7.el9.x86_64

hwdata-0.348-9.15.el9.noarch

cronie-1.5.7-12.el9_5.x86_64

crontabs-1.11-27.20190603git.el9.noarch

cronie-anacron-1.5.7-12.el9_5.x86_64

[root@rocky14 ~]# rpm -qa | grep -i kernel

kernel-modules-core-5.14.0-427.18.1.el9_4.x86_64

kernel-core-5.14.0-427.18.1.el9_4.x86_64

kernel-modules-5.14.0-427.18.1.el9_4.x86_64

kernel-core-5.14.0-427.42.1.el9_4.x86_64

kernel-modules-core-5.14.0-427.42.1.el9_4.x86_64

kernel-modules-5.14.0-427.42.1.el9_4.x86_64

kernel-core-5.14.0-503.23.1.el9_5.x86_64

kernel-modules-core-5.14.0-503.23.1.el9_5.x86_64

kernel-modules-5.14.0-503.23.1.el9_5.x86_64

[root@rocky14 ~]# rpm -qc systemd

/etc/X11/xinit/xinitrc.d/50-systemd-user.sh

/etc/X11/xorg.conf.d/00-keyboard.conf

/etc/dnf/protected.d/systemd.conf

/etc/hostname

/etc/locale.conf

/etc/localtime

/etc/machine-id

/etc/machine-info

/etc/pam.d/systemd-user

/etc/rc.d/rc.local

/etc/systemd/journald.conf

/etc/systemd/logind.conf

/etc/systemd/system.conf

/etc/systemd/user.conf

/etc/xdg/systemd/user

[root@rocky14 ~]# rpm -qi systemd

Name                : systemd

Version          : 252

Release          : 46.el9_5.2.0.1

Architecture: x86_64

Install Date: Mon Feb 10 18:36:58 2025

Group              : Unspecified

Size                : 12864308

License          : LGPLv2+ and MIT and GPLv2+

Signature      : RSA/SHA256, Fri Nov 15 18:27:06 2024, Key ID 702d426d350d275d

Source RPM    : systemd-252-46.el9_5.2.0.1.src.rpm

Build Date    : Fri Nov 15 18:18:17 2024

Build Host    : pb-7cdab3d7-2cf4-4e0b-b1ed-bf89e9226511-b-x86-64

Packager        : Rocky Linux Build System (Peridot) <releng@rockylinux.org>

Vendor            : Rocky Enterprise Software Foundation

URL                  : https://systemd.io

Summary          : System and Service Manager

Description :

systemd is a system and service manager that runs as PID 1 and starts

the rest of the system. It provides aggressive parallelization

capabilities, uses socket and D-Bus activation for starting services,

offers on-demand starting of daemons, keeps track of processes using

Linux control groups, maintains mount and automount points, and

implements an elaborate transactional dependency-based service control

logic. systemd supports SysV and LSB init scripts and works as a

replacement for sysvinit. Other parts of this package are a logging daemon,

utilities to control basic system configuration like the hostname,

date, locale, maintain a list of logged-in users, system accounts,

runtime directories and settings, and daemons to manage simple network

configuration, network time synchronization, log forwarding, and name

resolution.

[root@rocky14 ~]# rpm -ql systemd

/etc/X11/xinit/xinitrc.d/50-systemd-user.sh

/etc/X11/xorg.conf.d/00-keyboard.conf

/etc/dnf/protected.d/systemd.conf

/etc/hostname

/etc/inittab

/etc/locale.conf

/etc/localtime

/etc/machine-id

/etc/machine-info

/etc/pam.d/systemd-user

/etc/rc.d

/etc/rc.d/init.d

/etc/rc.d/init.d/README

/etc/rc.d/rc.local

/etc/rc.local

/etc/systemd

/etc/systemd/journald.conf

/etc/systemd/logind.conf

/etc/systemd/system

/etc/systemd/system.conf

/etc/systemd/system/basic.target.wants

/etc/systemd/system/bluetooth.target.wants

/etc/systemd/system/default.target.wants

/etc/systemd/system/getty.target.wants

/etc/systemd/system/graphical.target.wants

/etc/systemd/system/local-fs.target.wants

/etc/systemd/system/machines.target.wants

/etc/systemd/system/multi-user.target.wants

/etc/systemd/system/network-online.target.wants

/etc/systemd/system/printer.target.wants

/etc/systemd/system/remote-fs.target.wants

/etc/systemd/system/sockets.target.wants

/etc/systemd/system/sysinit.target.wants

/etc/systemd/system/system-update.target.wants

/etc/systemd/system/timers.target.wants

/etc/systemd/user

/etc/systemd/user.conf

/etc/tmpfiles.d

/etc/xdg/systemd

/etc/xdg/systemd/user

/run/utmp

/usr/bin/busctl

/usr/bin/hostnamectl

/usr/bin/journalctl

/usr/bin/localectl

/usr/bin/loginctl

/usr/bin/systemctl

/usr/bin/systemd-analyze

/usr/bin/systemd-ask-password

/usr/bin/systemd-cat

/usr/bin/systemd-cgls

/usr/bin/systemd-cgtop

/usr/bin/systemd-creds

/usr/bin/systemd-delta

/usr/bin/systemd-detect-virt

/usr/bin/systemd-dissect

/usr/bin/systemd-escape

/usr/bin/systemd-firstboot

/usr/bin/systemd-id128

/usr/bin/systemd-inhibit

/usr/bin/systemd-machine-id-setup

/usr/bin/systemd-mount

/usr/bin/systemd-notify

/usr/bin/systemd-path

/usr/bin/systemd-run

/usr/bin/systemd-socket-activate

/usr/bin/systemd-stdio-bridge

/usr/bin/systemd-sysext

/usr/bin/systemd-sysusers

/usr/bin/systemd-tmpfiles

/usr/bin/systemd-tty-ask-password-agent

/usr/bin/systemd-umount

/usr/bin/timedatectl

/usr/lib/.build-id

/usr/lib/.build-id/03

/usr/lib/.build-id/03/05f94b8455bf4fcd77a014f6d659beeea0cae8

/usr/lib/.build-id/03/5818efa3cf4be89cd50cecc0336ddc900bb523

/usr/lib/.build-id/07

/usr/lib/.build-id/07/12e011496609af6d3538c8dd9c1c608d6663fa

/usr/lib/.build-id/08

/usr/lib/.build-id/08/030b451772034cf2bdc959e4ba40088702cab0

/usr/lib/.build-id/0a

/usr/lib/.build-id/0a/430a5af5bc343d93252feac51eb3829d7f4507

/usr/lib/.build-id/13

/usr/lib/.build-id/13/8ad766266c2161878b617cb53f20257f4a497d

/usr/lib/.build-id/15

/usr/lib/.build-id/15/cae4b899735e116413b125f8d37b171feda71f

/usr/lib/.build-id/1a

/usr/lib/.build-id/1a/44ac302c1346a3ff8dd1037a7fe0a3508a8055

/usr/lib/.build-id/1b

/usr/lib/.build-id/1b/55175fa8a3e0f3a8fbb9d6de94a025c5c31b05

/usr/lib/.build-id/1b/554aca3011b44885d0e2ef4dea30a24726b65c

/usr/lib/.build-id/22

/usr/lib/.build-id/22/e082d68efabd21f76ad3c363f32ad9d5de9881

/usr/lib/.build-id/24

/usr/lib/.build-id/24/65ea9e8ac762687f6ccafc33d054427e011186

/usr/lib/.build-id/28

/usr/lib/.build-id/28/e662a5d56a9616fc73a9d046ead369d5f6fdd3

/usr/lib/.build-id/2d

/usr/lib/.build-id/2d/17303aa61dd600f9aafe863b75d675c976a729

/usr/lib/.build-id/2f

/usr/lib/.build-id/2f/b4cb201a90bee76366a61659d56b45d97a529d

/usr/lib/.build-id/31

/usr/lib/.build-id/31/d8ebdd515e28d7b59fd9c8564f239eff8424f2

/usr/lib/.build-id/3b

/usr/lib/.build-id/3b/2d60ceaa5c9bc0713c9f5d1c97e5cc67f86a2d

/usr/lib/.build-id/41

/usr/lib/.build-id/41/390abf468e5901171b06c0104a2eebac843198

/usr/lib/.build-id/41/39dd9eda87e6555fbfac906fa25013edee1e4b

/usr/lib/.build-id/43

/usr/lib/.build-id/43/77da3837dd472f05af31f0c414840492420423

/usr/lib/.build-id/45

/usr/lib/.build-id/45/ec717d89e1a83a893857c6969d0aeabc1ee601

/usr/lib/.build-id/4a

/usr/lib/.build-id/4a/840a7e37cf6d438f7cf4a75402683e4c123494

/usr/lib/.build-id/52

/usr/lib/.build-id/52/9b25311405a13a409c885fe59c0e588c0df088

/usr/lib/.build-id/53

/usr/lib/.build-id/53/0c90c5e1497023067c2c211924aa2ee2eab018

/usr/lib/.build-id/54

/usr/lib/.build-id/54/c0725290fd20d6c690ee72534d5b3b2ba22261

/usr/lib/.build-id/55

/usr/lib/.build-id/55/0da599325992b5ecd2dcea73221b9f064413d2

/usr/lib/.build-id/55/a9d4a822eb1074ca61659e8eb3697906df1e0a

/usr/lib/.build-id/56

/usr/lib/.build-id/56/12acf00f72853a136e10c8220f7af7220c0b36

/usr/lib/.build-id/56/9516c711717292ee19052b796cc268191264f1

/usr/lib/.build-id/65

/usr/lib/.build-id/65/ad3b60db4c7546dba3f31d833ccb2d2c6f6917

/usr/lib/.build-id/76

/usr/lib/.build-id/76/59f910cbb4a4629282ed0268286c0f01c5bb6e

/usr/lib/.build-id/76/6c5f6493de9c953c813554b7708c9bd99fc948

/usr/lib/.build-id/78

/usr/lib/.build-id/78/b8f28cf2c6c0dfb8b2b596272a5b8b5b173723

/usr/lib/.build-id/79

/usr/lib/.build-id/79/0c31e0d94b10a000871d987e02a9060c433572

/usr/lib/.build-id/7d

/usr/lib/.build-id/7d/3ac952bed7eccce12de2a2276893882b720c58

/usr/lib/.build-id/7e

/usr/lib/.build-id/7e/dac2ca6f3bc27132d708369695bdc79589687e

/usr/lib/.build-id/82

/usr/lib/.build-id/82/daf02a3390927615bf44f27e7e7e8fa366743f

/usr/lib/.build-id/8a

/usr/lib/.build-id/8a/ad8e6b9000622068eefe883907349f1a0b4e96

/usr/lib/.build-id/91

/usr/lib/.build-id/91/c96edce83227943d8d5a85632a01d4667f48e4

/usr/lib/.build-id/93

/usr/lib/.build-id/93/46805ab1fb117d9bea63e3aa415923a9aed96f

/usr/lib/.build-id/94

/usr/lib/.build-id/94/b2d405ad7331e0035102561dc5c9d56f089fb2

/usr/lib/.build-id/96

/usr/lib/.build-id/96/d9ca02f52df7473e38d7ffef65357b68cf6577

/usr/lib/.build-id/99

/usr/lib/.build-id/99/0d0a3edbcdb26fbd5dcd2d45ccba6bb033d45d

/usr/lib/.build-id/a0

/usr/lib/.build-id/a0/dac91e97a7ff83df4b909d83650ea5e5cc10d4

/usr/lib/.build-id/a0/f1ca85223a58c445c6f84c15b458a40f580204

/usr/lib/.build-id/a6

/usr/lib/.build-id/a6/0cffbff79fdfc18533a64cfc18b5944096d230

/usr/lib/.build-id/aa

/usr/lib/.build-id/aa/4dd7a60918bdaaf8b4e28978731b94e4ee272d

/usr/lib/.build-id/aa/b65226742b80e296fb23a042313fbb6ac0177e

/usr/lib/.build-id/ac

/usr/lib/.build-id/ac/5f0c9d01023e64d5cf5308af9bb5083d724221

/usr/lib/.build-id/ba

/usr/lib/.build-id/ba/e1a47da1853f8f3eb34d88b35dd413d9073817

/usr/lib/.build-id/ba/fc320aa325a3301bbd243f4667b60324f31152

/usr/lib/.build-id/c0

/usr/lib/.build-id/c0/135a2d72845595db653f87eefa68d7279b0cf2

/usr/lib/.build-id/c7

/usr/lib/.build-id/c7/0dc4df069592f33788ecef7a7cc371e0b0b7ec

/usr/lib/.build-id/c7/4f478b294b3584dbc5777187de1d83e24ae134

/usr/lib/.build-id/c9

/usr/lib/.build-id/c9/05c197621e0e539e4f2a5fe9d3f0de7348a8f1

/usr/lib/.build-id/d5

/usr/lib/.build-id/d5/a6d7fc0fcb882cd018feae7201f17d8dc26b1c

/usr/lib/.build-id/e2

/usr/lib/.build-id/e2/509c5cfa69e1f800c6c13da320f03cd3f9a2ef

/usr/lib/.build-id/e3

/usr/lib/.build-id/e3/8dec03df05fd9df73cc99d8c949c27ce978108

/usr/lib/.build-id/e8

/usr/lib/.build-id/e8/03b384a0013a747a4cd2e60392c4a557266ee2

/usr/lib/.build-id/ea

/usr/lib/.build-id/ea/d49965fc15921ad695cb05cc1e53299e7973e3

/usr/lib/.build-id/f2

/usr/lib/.build-id/f2/1fcd26f5e16bf97f0b55747f18287b53f34f13

/usr/lib/.build-id/f5

/usr/lib/.build-id/f5/c1e5e17565d7b1021af4ab5fb87e25a22d946a

/usr/lib/.build-id/fa

/usr/lib/.build-id/fa/206a49d5246b6a69192cb01f897ac2bb7c7eca

/usr/lib/.build-id/ff

/usr/lib/.build-id/ff/7e65d82d0e976420023eca8ccc0a5bdd5f7587

/usr/lib/environment.d

/usr/lib/environment.d/99-environment.conf

/usr/lib/pam.d

/usr/lib/pam.d/systemd-user

/usr/lib/systemd

/usr/lib/systemd/catalog

/usr/lib/systemd/catalog/systemd.be.catalog

/usr/lib/systemd/catalog/systemd.be@latin.catalog

/usr/lib/systemd/catalog/systemd.bg.catalog

/usr/lib/systemd/catalog/systemd.catalog

/usr/lib/systemd/catalog/systemd.de.catalog

/usr/lib/systemd/catalog/systemd.fr.catalog

/usr/lib/systemd/catalog/systemd.it.catalog

/usr/lib/systemd/catalog/systemd.pl.catalog

/usr/lib/systemd/catalog/systemd.pt_BR.catalog

/usr/lib/systemd/catalog/systemd.ru.catalog

/usr/lib/systemd/catalog/systemd.zh_CN.catalog

/usr/lib/systemd/catalog/systemd.zh_TW.catalog

/usr/lib/systemd/libsystemd-shared.abignore

/usr/lib/systemd/network

/usr/lib/systemd/purge-nobody-user

/usr/lib/systemd/resolv.conf

/usr/lib/systemd/system

/usr/lib/systemd/system-generators

/usr/lib/systemd/system-generators/systemd-debug-generator

/usr/lib/systemd/system-generators/systemd-fstab-generator

/usr/lib/systemd/system-generators/systemd-getty-generator

/usr/lib/systemd/system-generators/systemd-rc-local-generator

/usr/lib/systemd/system-generators/systemd-run-generator

/usr/lib/systemd/system-generators/systemd-system-update-generator

/usr/lib/systemd/system-generators/systemd-sysv-generator

/usr/lib/systemd/system-preset

/usr/lib/systemd/system-preset/90-systemd.preset

/usr/lib/systemd/system-shutdown

/usr/lib/systemd/system/-.slice.d

/usr/lib/systemd/system/autovt@.service

/usr/lib/systemd/system/basic.target

/usr/lib/systemd/system/basic.target.wants

/usr/lib/systemd/system/blockdev@.target

/usr/lib/systemd/system/bluetooth.target

/usr/lib/systemd/system/boot-complete.target

/usr/lib/systemd/system/console-getty.service

/usr/lib/systemd/system/container-getty@.service

/usr/lib/systemd/system/ctrl-alt-del.target

/usr/lib/systemd/system/dbus-org.freedesktop.hostname1.service

/usr/lib/systemd/system/dbus-org.freedesktop.locale1.service

/usr/lib/systemd/system/dbus-org.freedesktop.login1.service

/usr/lib/systemd/system/dbus-org.freedesktop.timedate1.service

/usr/lib/systemd/system/dbus.target.wants

/usr/lib/systemd/system/debug-shell.service

/usr/lib/systemd/system/default.target

/usr/lib/systemd/system/default.target.wants

/usr/lib/systemd/system/dev-hugepages.mount

/usr/lib/systemd/system/dev-mqueue.mount

/usr/lib/systemd/system/emergency.service

/usr/lib/systemd/system/emergency.target

/usr/lib/systemd/system/exit.target

/usr/lib/systemd/system/factory-reset.target

/usr/lib/systemd/system/final.target

/usr/lib/systemd/system/first-boot-complete.target

/usr/lib/systemd/system/getty-pre.target

/usr/lib/systemd/system/getty.target

/usr/lib/systemd/system/getty@.service

/usr/lib/systemd/system/graphical.target

/usr/lib/systemd/system/graphical.target.wants

/usr/lib/systemd/system/graphical.target.wants/systemd-update-utmp-runlevel.service

/usr/lib/systemd/system/halt.target

/usr/lib/systemd/system/kexec.target

/usr/lib/systemd/system/ldconfig.service

/usr/lib/systemd/system/local-fs-pre.target

/usr/lib/systemd/system/local-fs.target

/usr/lib/systemd/system/modprobe@.service

/usr/lib/systemd/system/multi-user.target

/usr/lib/systemd/system/multi-user.target.wants

/usr/lib/systemd/system/multi-user.target.wants/getty.target

/usr/lib/systemd/system/multi-user.target.wants/systemd-ask-password-wall.path

/usr/lib/systemd/system/multi-user.target.wants/systemd-logind.service

/usr/lib/systemd/system/multi-user.target.wants/systemd-update-utmp-runlevel.service

/usr/lib/systemd/system/multi-user.target.wants/systemd-user-sessions.service

/usr/lib/systemd/system/network-online.target

/usr/lib/systemd/system/network-pre.target

/usr/lib/systemd/system/network.target

/usr/lib/systemd/system/nss-lookup.target

/usr/lib/systemd/system/nss-user-lookup.target

/usr/lib/systemd/system/paths.target

/usr/lib/systemd/system/poweroff.target

/usr/lib/systemd/system/printer.target

/usr/lib/systemd/system/rc-local.service

/usr/lib/systemd/system/reboot.target

/usr/lib/systemd/system/remote-fs-pre.target

/usr/lib/systemd/system/remote-fs.target

/usr/lib/systemd/system/remote-fs.target.wants

/usr/lib/systemd/system/rescue.service

/usr/lib/systemd/system/rescue.target

/usr/lib/systemd/system/rescue.target.wants

/usr/lib/systemd/system/rescue.target.wants/systemd-update-utmp-runlevel.service

/usr/lib/systemd/system/rpcbind.target

/usr/lib/systemd/system/runlevel0.target

/usr/lib/systemd/system/runlevel1.target

/usr/lib/systemd/system/runlevel1.target.wants

/usr/lib/systemd/system/runlevel2.target

/usr/lib/systemd/system/runlevel2.target.wants

/usr/lib/systemd/system/runlevel3.target

/usr/lib/systemd/system/runlevel3.target.wants

/usr/lib/systemd/system/runlevel4.target

/usr/lib/systemd/system/runlevel4.target.wants

/usr/lib/systemd/system/runlevel5.target

/usr/lib/systemd/system/runlevel5.target.wants

/usr/lib/systemd/system/runlevel6.target

/usr/lib/systemd/system/serial-getty@.service

/usr/lib/systemd/system/shutdown.target

/usr/lib/systemd/system/sigpwr.target

/usr/lib/systemd/system/slices.target

/usr/lib/systemd/system/smartcard.target

/usr/lib/systemd/system/sockets.target

/usr/lib/systemd/system/sockets.target.wants

/usr/lib/systemd/system/sockets.target.wants/systemd-initctl.socket

/usr/lib/systemd/system/sockets.target.wants/systemd-journald-dev-log.socket

/usr/lib/systemd/system/sockets.target.wants/systemd-journald.socket

/usr/lib/systemd/system/sound.target

/usr/lib/systemd/system/swap.target

/usr/lib/systemd/system/sys-fs-fuse-connections.mount

/usr/lib/systemd/system/sys-kernel-config.mount

/usr/lib/systemd/system/sys-kernel-debug.mount

/usr/lib/systemd/system/sys-kernel-tracing.mount

/usr/lib/systemd/system/sysinit.target

/usr/lib/systemd/system/sysinit.target.wants

/usr/lib/systemd/system/sysinit.target.wants/dev-hugepages.mount

/usr/lib/systemd/system/sysinit.target.wants/dev-mqueue.mount

/usr/lib/systemd/system/sysinit.target.wants/ldconfig.service

/usr/lib/systemd/system/sysinit.target.wants/sys-fs-fuse-connections.mount

/usr/lib/systemd/system/sysinit.target.wants/sys-kernel-config.mount

/usr/lib/systemd/system/sysinit.target.wants/sys-kernel-debug.mount

/usr/lib/systemd/system/sysinit.target.wants/sys-kernel-tracing.mount

/usr/lib/systemd/system/sysinit.target.wants/systemd-ask-password-console.path

/usr/lib/systemd/system/sysinit.target.wants/systemd-firstboot.service

/usr/lib/systemd/system/sysinit.target.wants/systemd-journal-catalog-update.service

/usr/lib/systemd/system/sysinit.target.wants/systemd-journal-flush.service

/usr/lib/systemd/system/sysinit.target.wants/systemd-journald.service

/usr/lib/systemd/system/sysinit.target.wants/systemd-machine-id-commit.service

/usr/lib/systemd/system/sysinit.target.wants/systemd-pcrmachine.service

/usr/lib/systemd/system/sysinit.target.wants/systemd-sysusers.service

/usr/lib/systemd/system/sysinit.target.wants/systemd-tmpfiles-setup.service

/usr/lib/systemd/system/sysinit.target.wants/systemd-update-done.service

/usr/lib/systemd/system/sysinit.target.wants/systemd-update-utmp.service

/usr/lib/systemd/system/syslog.socket

/usr/lib/systemd/system/syslog.target.wants

/usr/lib/systemd/system/system-update-cleanup.service

/usr/lib/systemd/system/system-update-pre.target

/usr/lib/systemd/system/system-update.target

/usr/lib/systemd/system/systemd-ask-password-console.path

/usr/lib/systemd/system/systemd-ask-password-console.service

/usr/lib/systemd/system/systemd-ask-password-wall.path

/usr/lib/systemd/system/systemd-ask-password-wall.service

/usr/lib/systemd/system/systemd-boot-check-no-failures.service

/usr/lib/systemd/system/systemd-exit.service

/usr/lib/systemd/system/systemd-firstboot.service

/usr/lib/systemd/system/systemd-halt.service

/usr/lib/systemd/system/systemd-hostnamed.service

/usr/lib/systemd/system/systemd-hostnamed.service.d

/usr/lib/systemd/system/systemd-hostnamed.service.d/disable-privatedevices.conf

/usr/lib/systemd/system/systemd-initctl.service

/usr/lib/systemd/system/systemd-initctl.socket

/usr/lib/systemd/system/systemd-journal-catalog-update.service

/usr/lib/systemd/system/systemd-journal-flush.service

/usr/lib/systemd/system/systemd-journald-audit.socket

/usr/lib/systemd/system/systemd-journald-dev-log.socket

/usr/lib/systemd/system/systemd-journald-varlink@.socket

/usr/lib/systemd/system/systemd-journald.service

/usr/lib/systemd/system/systemd-journald.socket

/usr/lib/systemd/system/systemd-journald@.service

/usr/lib/systemd/system/systemd-journald@.socket

/usr/lib/systemd/system/systemd-kexec.service

/usr/lib/systemd/system/systemd-localed.service

/usr/lib/systemd/system/systemd-logind.service

/usr/lib/systemd/system/systemd-machine-id-commit.service

/usr/lib/systemd/system/systemd-network-generator.service

/usr/lib/systemd/system/systemd-pcrfs-root.service

/usr/lib/systemd/system/systemd-pcrfs@.service

/usr/lib/systemd/system/systemd-pcrmachine.service

/usr/lib/systemd/system/systemd-poweroff.service

/usr/lib/systemd/system/systemd-reboot.service

/usr/lib/systemd/system/systemd-sysext.service

/usr/lib/systemd/system/systemd-sysupdate-reboot.service

/usr/lib/systemd/system/systemd-sysupdate-reboot.timer

/usr/lib/systemd/system/systemd-sysupdate.service

/usr/lib/systemd/system/systemd-sysupdate.timer

/usr/lib/systemd/system/systemd-sysusers.service

/usr/lib/systemd/system/systemd-timedated.service

/usr/lib/systemd/system/systemd-tmpfiles-clean.service

/usr/lib/systemd/system/systemd-tmpfiles-clean.timer

/usr/lib/systemd/system/systemd-tmpfiles-setup.service

/usr/lib/systemd/system/systemd-update-done.service

/usr/lib/systemd/system/systemd-update-utmp-runlevel.service

/usr/lib/systemd/system/systemd-update-utmp.service

/usr/lib/systemd/system/systemd-user-sessions.service

/usr/lib/systemd/system/time-set.target

/usr/lib/systemd/system/time-sync.target

/usr/lib/systemd/system/timers.target

/usr/lib/systemd/system/timers.target.wants

/usr/lib/systemd/system/timers.target.wants/systemd-tmpfiles-clean.timer

/usr/lib/systemd/system/tmp.mount

/usr/lib/systemd/system/umount.target

/usr/lib/systemd/system/usb-gadget.target

/usr/lib/systemd/system/user-.slice.d

/usr/lib/systemd/system/user-.slice.d/10-defaults.conf

/usr/lib/systemd/system/user-runtime-dir@.service

/usr/lib/systemd/system/user.slice

/usr/lib/systemd/system/user@.service

/usr/lib/systemd/system/user@.service.d

/usr/lib/systemd/system/user@.service.d/10-login-barrier.conf

/usr/lib/systemd/system/user@0.service.d

/usr/lib/systemd/system/user@0.service.d/10-login-barrier.conf

/usr/lib/systemd/systemd

/usr/lib/systemd/systemd-ac-power

/usr/lib/systemd/systemd-boot-check-no-failures

/usr/lib/systemd/systemd-cgroups-agent

/usr/lib/systemd/systemd-export

/usr/lib/systemd/systemd-hostnamed

/usr/lib/systemd/systemd-initctl

/usr/lib/systemd/systemd-journald

/usr/lib/systemd/systemd-localed

/usr/lib/systemd/systemd-logind

/usr/lib/systemd/systemd-network-generator

/usr/lib/systemd/systemd-reply-password

/usr/lib/systemd/systemd-shutdown

/usr/lib/systemd/systemd-socket-proxyd

/usr/lib/systemd/systemd-sulogin-shell

/usr/lib/systemd/systemd-sysroot-fstab-check

/usr/lib/systemd/systemd-sysupdate

/usr/lib/systemd/systemd-timedated

/usr/lib/systemd/systemd-update-done

/usr/lib/systemd/systemd-update-helper

/usr/lib/systemd/systemd-update-utmp

/usr/lib/systemd/systemd-user-runtime-dir

/usr/lib/systemd/systemd-user-sessions

/usr/lib/systemd/systemd-xdg-autostart-condition

/usr/lib/systemd/user

/usr/lib/systemd/user-environment-generators

/usr/lib/systemd/user-environment-generators/30-systemd-environment-d-generator

/usr/lib/systemd/user-generators

/usr/lib/systemd/user-generators/systemd-xdg-autostart-generator

/usr/lib/systemd/user-preset

/usr/lib/systemd/user-preset/90-systemd.preset

/usr/lib/systemd/user/app.slice

/usr/lib/systemd/user/background.slice

/usr/lib/systemd/user/basic.target

/usr/lib/systemd/user/bluetooth.target

/usr/lib/systemd/user/default.target

/usr/lib/systemd/user/exit.target

/usr/lib/systemd/user/graphical-session-pre.target

/usr/lib/systemd/user/graphical-session.target

/usr/lib/systemd/user/paths.target

/usr/lib/systemd/user/printer.target

/usr/lib/systemd/user/session.slice

/usr/lib/systemd/user/shutdown.target

/usr/lib/systemd/user/smartcard.target

/usr/lib/systemd/user/sockets.target

/usr/lib/systemd/user/sound.target

/usr/lib/systemd/user/systemd-exit.service

/usr/lib/systemd/user/systemd-tmpfiles-clean.service

/usr/lib/systemd/user/systemd-tmpfiles-clean.timer

/usr/lib/systemd/user/systemd-tmpfiles-setup.service

/usr/lib/systemd/user/timers.target

/usr/lib/systemd/user/xdg-desktop-autostart.target

/usr/lib/sysusers.d

/usr/lib/sysusers.d/README

/usr/lib/sysusers.d/basic.conf

/usr/lib/sysusers.d/systemd-journal.conf

/usr/lib/tmpfiles.d

/usr/lib/tmpfiles.d/README

/usr/lib/tmpfiles.d/etc.conf

/usr/lib/tmpfiles.d/home.conf

/usr/lib/tmpfiles.d/journal-nocow.conf

/usr/lib/tmpfiles.d/legacy.conf

/usr/lib/tmpfiles.d/provision.conf

/usr/lib/tmpfiles.d/static-nodes-permissions.conf

/usr/lib/tmpfiles.d/systemd-nologin.conf

/usr/lib/tmpfiles.d/systemd-tmp.conf

/usr/lib/tmpfiles.d/systemd.conf

/usr/lib/tmpfiles.d/tmp.conf

/usr/lib/tmpfiles.d/var.conf

/usr/lib/tmpfiles.d/x11.conf

/usr/lib64/systemd

/usr/lib64/systemd/libsystemd-core-252.so

/usr/lib64/systemd/libsystemd-shared-252.so

/usr/sbin/halt

/usr/sbin/init

/usr/sbin/poweroff

/usr/sbin/reboot

/usr/sbin/runlevel

/usr/sbin/shutdown

/usr/sbin/telinit

/usr/share/bash-completion/completions/busctl

/usr/share/bash-completion/completions/hostnamectl

/usr/share/bash-completion/completions/journalctl

/usr/share/bash-completion/completions/localectl

/usr/share/bash-completion/completions/loginctl

/usr/share/bash-completion/completions/systemctl

/usr/share/bash-completion/completions/systemd-analyze

/usr/share/bash-completion/completions/systemd-cat

/usr/share/bash-completion/completions/systemd-cgls

/usr/share/bash-completion/completions/systemd-cgtop

/usr/share/bash-completion/completions/systemd-delta

/usr/share/bash-completion/completions/systemd-detect-virt

/usr/share/bash-completion/completions/systemd-id128

/usr/share/bash-completion/completions/systemd-path

/usr/share/bash-completion/completions/systemd-run

/usr/share/bash-completion/completions/timedatectl

/usr/share/dbus-1/interfaces

/usr/share/dbus-1/interfaces/org.freedesktop.LogControl1.xml

/usr/share/dbus-1/interfaces/org.freedesktop.hostname1.xml

/usr/share/dbus-1/interfaces/org.freedesktop.locale1.xml

/usr/share/dbus-1/interfaces/org.freedesktop.login1.Manager.xml

/usr/share/dbus-1/interfaces/org.freedesktop.login1.Seat.xml

/usr/share/dbus-1/interfaces/org.freedesktop.login1.Session.xml

/usr/share/dbus-1/interfaces/org.freedesktop.login1.User.xml

/usr/share/dbus-1/interfaces/org.freedesktop.systemd1.Automount.xml

/usr/share/dbus-1/interfaces/org.freedesktop.systemd1.Device.xml

/usr/share/dbus-1/interfaces/org.freedesktop.systemd1.Job.xml

/usr/share/dbus-1/interfaces/org.freedesktop.systemd1.Manager.xml

/usr/share/dbus-1/interfaces/org.freedesktop.systemd1.Mount.xml

/usr/share/dbus-1/interfaces/org.freedesktop.systemd1.Path.xml

/usr/share/dbus-1/interfaces/org.freedesktop.systemd1.Scope.xml

/usr/share/dbus-1/interfaces/org.freedesktop.systemd1.Service.xml

/usr/share/dbus-1/interfaces/org.freedesktop.systemd1.Slice.xml

/usr/share/dbus-1/interfaces/org.freedesktop.systemd1.Socket.xml

/usr/share/dbus-1/interfaces/org.freedesktop.systemd1.Swap.xml

/usr/share/dbus-1/interfaces/org.freedesktop.systemd1.Target.xml

/usr/share/dbus-1/interfaces/org.freedesktop.systemd1.Timer.xml

/usr/share/dbus-1/interfaces/org.freedesktop.systemd1.Unit.xml

/usr/share/dbus-1/interfaces/org.freedesktop.timedate1.xml

/usr/share/dbus-1/services/org.freedesktop.systemd1.service

/usr/share/dbus-1/system-services/org.freedesktop.hostname1.service

/usr/share/dbus-1/system-services/org.freedesktop.locale1.service

/usr/share/dbus-1/system-services/org.freedesktop.login1.service

/usr/share/dbus-1/system-services/org.freedesktop.systemd1.service

/usr/share/dbus-1/system-services/org.freedesktop.timedate1.service

/usr/share/dbus-1/system.d/org.freedesktop.hostname1.conf

/usr/share/dbus-1/system.d/org.freedesktop.locale1.conf

/usr/share/dbus-1/system.d/org.freedesktop.login1.conf

/usr/share/dbus-1/system.d/org.freedesktop.systemd1.conf

/usr/share/dbus-1/system.d/org.freedesktop.timedate1.conf

/usr/share/doc/systemd

/usr/share/doc/systemd/20-yama-ptrace.conf

/usr/share/doc/systemd/CODING_STYLE.md

/usr/share/doc/systemd/DISTRO_PORTING.md

/usr/share/doc/systemd/ENVIRONMENT.md

/usr/share/doc/systemd/HACKING.md

/usr/share/doc/systemd/LICENSES

/usr/share/doc/systemd/LICENSES/BSD-2-Clause.txt

/usr/share/doc/systemd/LICENSES/BSD-3-Clause.txt

/usr/share/doc/systemd/LICENSES/CC0-1.0.txt

/usr/share/doc/systemd/LICENSES/LGPL-2.0-or-later.txt

/usr/share/doc/systemd/LICENSES/Linux-syscall-note.txt

/usr/share/doc/systemd/LICENSES/MIT-0.txt

/usr/share/doc/systemd/LICENSES/MIT.txt

/usr/share/doc/systemd/LICENSES/OFL-1.1.txt

/usr/share/doc/systemd/LICENSES/README.md

/usr/share/doc/systemd/LICENSES/lookup3-public-domain.txt

/usr/share/doc/systemd/LICENSES/murmurhash2-public-domain.txt

/usr/share/doc/systemd/NEWS

/usr/share/doc/systemd/README

/usr/share/doc/systemd/README.logs

/usr/share/doc/systemd/TRANSIENT-SETTINGS.md

/usr/share/doc/systemd/TRANSLATORS.md

/usr/share/doc/systemd/UIDS-GIDS.md

/usr/share/factory

/usr/share/factory/etc

/usr/share/factory/etc/issue

/usr/share/factory/etc/locale.conf

/usr/share/factory/etc/nsswitch.conf

/usr/share/factory/etc/pam.d

/usr/share/factory/etc/pam.d/other

/usr/share/factory/etc/pam.d/system-auth

/usr/share/licenses/systemd

/usr/share/licenses/systemd/LICENSE.GPL2

/usr/share/licenses/systemd/LICENSE.LGPL2.1

/usr/share/locale/be/LC_MESSAGES/systemd.mo

/usr/share/locale/be@latin/LC_MESSAGES/systemd.mo

/usr/share/locale/bg/LC_MESSAGES/systemd.mo

/usr/share/locale/ca/LC_MESSAGES/systemd.mo

/usr/share/locale/cs/LC_MESSAGES/systemd.mo

/usr/share/locale/da/LC_MESSAGES/systemd.mo

/usr/share/locale/de/LC_MESSAGES/systemd.mo

/usr/share/locale/el/LC_MESSAGES/systemd.mo

/usr/share/locale/es/LC_MESSAGES/systemd.mo

/usr/share/locale/et/LC_MESSAGES/systemd.mo

/usr/share/locale/fi/LC_MESSAGES/systemd.mo

/usr/share/locale/fr/LC_MESSAGES/systemd.mo

/usr/share/locale/gl/LC_MESSAGES/systemd.mo

/usr/share/locale/hr/LC_MESSAGES/systemd.mo

/usr/share/locale/hu/LC_MESSAGES/systemd.mo

/usr/share/locale/id/LC_MESSAGES/systemd.mo

/usr/share/locale/it/LC_MESSAGES/systemd.mo

/usr/share/locale/ja/LC_MESSAGES/systemd.mo

/usr/share/locale/ka/LC_MESSAGES/systemd.mo

/usr/share/locale/kab/LC_MESSAGES/systemd.mo

/usr/share/locale/ko/LC_MESSAGES/systemd.mo

/usr/share/locale/lt/LC_MESSAGES/systemd.mo

/usr/share/locale/nl/LC_MESSAGES/systemd.mo

/usr/share/locale/pa/LC_MESSAGES/systemd.mo

/usr/share/locale/pl/LC_MESSAGES/systemd.mo

/usr/share/locale/pt/LC_MESSAGES/systemd.mo

/usr/share/locale/pt_BR/LC_MESSAGES/systemd.mo

/usr/share/locale/ro/LC_MESSAGES/systemd.mo

/usr/share/locale/ru/LC_MESSAGES/systemd.mo

/usr/share/locale/si/LC_MESSAGES/systemd.mo

/usr/share/locale/sk/LC_MESSAGES/systemd.mo

/usr/share/locale/sr/LC_MESSAGES/systemd.mo

/usr/share/locale/sv/LC_MESSAGES/systemd.mo

/usr/share/locale/tr/LC_MESSAGES/systemd.mo

/usr/share/locale/uk/LC_MESSAGES/systemd.mo

/usr/share/locale/zh_CN/LC_MESSAGES/systemd.mo

/usr/share/locale/zh_TW/LC_MESSAGES/systemd.mo

/usr/share/man/man1/busctl.1.gz

/usr/share/man/man1/hostnamectl.1.gz

/usr/share/man/man1/init.1.gz

/usr/share/man/man1/journalctl.1.gz

/usr/share/man/man1/localectl.1.gz

/usr/share/man/man1/loginctl.1.gz

/usr/share/man/man1/systemctl.1.gz

/usr/share/man/man1/systemd-analyze.1.gz

/usr/share/man/man1/systemd-ask-password.1.gz

/usr/share/man/man1/systemd-cat.1.gz

/usr/share/man/man1/systemd-cgls.1.gz

/usr/share/man/man1/systemd-cgtop.1.gz

/usr/share/man/man1/systemd-creds.1.gz

/usr/share/man/man1/systemd-delta.1.gz

/usr/share/man/man1/systemd-detect-virt.1.gz

/usr/share/man/man1/systemd-dissect.1.gz

/usr/share/man/man1/systemd-escape.1.gz

/usr/share/man/man1/systemd-firstboot.1.gz

/usr/share/man/man1/systemd-firstboot.service.1.gz

/usr/share/man/man1/systemd-id128.1.gz

/usr/share/man/man1/systemd-inhibit.1.gz

/usr/share/man/man1/systemd-machine-id-setup.1.gz

/usr/share/man/man1/systemd-mount.1.gz

/usr/share/man/man1/systemd-notify.1.gz

/usr/share/man/man1/systemd-path.1.gz

/usr/share/man/man1/systemd-run.1.gz

/usr/share/man/man1/systemd-socket-activate.1.gz

/usr/share/man/man1/systemd-stdio-bridge.1.gz

/usr/share/man/man1/systemd-tty-ask-password-agent.1.gz

/usr/share/man/man1/systemd-umount.1.gz

/usr/share/man/man1/systemd.1.gz

/usr/share/man/man1/timedatectl.1.gz

/usr/share/man/man5/dnssec-trust-anchors.d.5.gz

/usr/share/man/man5/environment.d.5.gz

/usr/share/man/man5/extension-release.5.gz

/usr/share/man/man5/hostname.5.gz

/usr/share/man/man5/journald.conf.5.gz

/usr/share/man/man5/journald.conf.d.5.gz

/usr/share/man/man5/journald@.conf.5.gz

/usr/share/man/man5/locale.conf.5.gz

/usr/share/man/man5/localtime.5.gz

/usr/share/man/man5/logind.conf.5.gz

/usr/share/man/man5/logind.conf.d.5.gz

/usr/share/man/man5/machine-id.5.gz

/usr/share/man/man5/machine-info.5.gz

/usr/share/man/man5/org.freedesktop.LogControl1.5.gz

/usr/share/man/man5/org.freedesktop.hostname1.5.gz

/usr/share/man/man5/org.freedesktop.locale1.5.gz

/usr/share/man/man5/org.freedesktop.login1.5.gz

/usr/share/man/man5/org.freedesktop.systemd1.5.gz

/usr/share/man/man5/org.freedesktop.timedate1.5.gz

/usr/share/man/man5/os-release.5.gz

/usr/share/man/man5/system.conf.d.5.gz

/usr/share/man/man5/systemd-system.conf.5.gz

/usr/share/man/man5/systemd-user-runtime-dir.5.gz

/usr/share/man/man5/systemd-user.conf.5.gz

/usr/share/man/man5/systemd.automount.5.gz

/usr/share/man/man5/systemd.device.5.gz

/usr/share/man/man5/systemd.dnssd.5.gz

/usr/share/man/man5/systemd.exec.5.gz

/usr/share/man/man5/systemd.kill.5.gz

/usr/share/man/man5/systemd.link.5.gz

/usr/share/man/man5/systemd.mount.5.gz

/usr/share/man/man5/systemd.nspawn.5.gz

/usr/share/man/man5/systemd.path.5.gz

/usr/share/man/man5/systemd.preset.5.gz

/usr/share/man/man5/systemd.resource-control.5.gz

/usr/share/man/man5/systemd.scope.5.gz

/usr/share/man/man5/systemd.service.5.gz

/usr/share/man/man5/systemd.slice.5.gz

/usr/share/man/man5/systemd.socket.5.gz

/usr/share/man/man5/systemd.swap.5.gz

/usr/share/man/man5/systemd.target.5.gz

/usr/share/man/man5/systemd.timer.5.gz

/usr/share/man/man5/systemd.unit.5.gz

/usr/share/man/man5/sysupdate.d.5.gz

/usr/share/man/man5/sysusers.d.5.gz

/usr/share/man/man5/tmpfiles.d.5.gz

/usr/share/man/man5/user-runtime-dir@.service.5.gz

/usr/share/man/man5/user.conf.d.5.gz

/usr/share/man/man5/user@.service.5.gz

/usr/share/man/man5/veritytab.5.gz

/usr/share/man/man7/bootup.7.gz

/usr/share/man/man7/daemon.7.gz

/usr/share/man/man7/file-hierarchy.7.gz

/usr/share/man/man7/kernel-command-line.7.gz

/usr/share/man/man7/linuxaa64.efi.stub.7.gz

/usr/share/man/man7/linuxia32.efi.stub.7.gz

/usr/share/man/man7/linuxx64.efi.stub.7.gz

/usr/share/man/man7/sd-stub.7.gz

/usr/share/man/man7/systemd-stub.7.gz

/usr/share/man/man7/systemd.directives.7.gz

/usr/share/man/man7/systemd.environment-generator.7.gz

/usr/share/man/man7/systemd.generator.7.gz

/usr/share/man/man7/systemd.index.7.gz

/usr/share/man/man7/systemd.journal-fields.7.gz

/usr/share/man/man7/systemd.net-naming-scheme.7.gz

/usr/share/man/man7/systemd.offline-updates.7.gz

/usr/share/man/man7/systemd.special.7.gz

/usr/share/man/man7/systemd.syntax.7.gz

/usr/share/man/man7/systemd.system-credentials.7.gz

/usr/share/man/man7/systemd.time.7.gz

/usr/share/man/man8/30-systemd-environment-d-generator.8.gz

/usr/share/man/man8/halt.8.gz

/usr/share/man/man8/nss-myhostname.8.gz

/usr/share/man/man8/nss-systemd.8.gz

/usr/share/man/man8/poweroff.8.gz

/usr/share/man/man8/rc-local.service.8.gz

/usr/share/man/man8/reboot.8.gz

/usr/share/man/man8/runlevel.8.gz

/usr/share/man/man8/shutdown.8.gz

/usr/share/man/man8/systemd-ask-password-console.path.8.gz

/usr/share/man/man8/systemd-ask-password-console.service.8.gz

/usr/share/man/man8/systemd-ask-password-wall.path.8.gz

/usr/share/man/man8/systemd-ask-password-wall.service.8.gz

/usr/share/man/man8/systemd-boot-check-no-failures.8.gz

/usr/share/man/man8/systemd-boot-check-no-failures.service.8.gz

/usr/share/man/man8/systemd-debug-generator.8.gz

/usr/share/man/man8/systemd-environment-d-generator.8.gz

/usr/share/man/man8/systemd-fstab-generator.8.gz

/usr/share/man/man8/systemd-getty-generator.8.gz

/usr/share/man/man8/systemd-halt.service.8.gz

/usr/share/man/man8/systemd-hostnamed.8.gz

/usr/share/man/man8/systemd-hostnamed.service.8.gz

/usr/share/man/man8/systemd-initctl.8.gz

/usr/share/man/man8/systemd-initctl.service.8.gz

/usr/share/man/man8/systemd-initctl.socket.8.gz

/usr/share/man/man8/systemd-journald-audit.socket.8.gz

/usr/share/man/man8/systemd-journald-dev-log.socket.8.gz

/usr/share/man/man8/systemd-journald-varlink@.socket.8.gz

/usr/share/man/man8/systemd-journald.8.gz

/usr/share/man/man8/systemd-journald.service.8.gz

/usr/share/man/man8/systemd-journald.socket.8.gz

/usr/share/man/man8/systemd-journald@.service.8.gz

/usr/share/man/man8/systemd-journald@.socket.8.gz

/usr/share/man/man8/systemd-kexec.service.8.gz

/usr/share/man/man8/systemd-localed.8.gz

/usr/share/man/man8/systemd-localed.service.8.gz

/usr/share/man/man8/systemd-logind.8.gz

/usr/share/man/man8/systemd-logind.service.8.gz

/usr/share/man/man8/systemd-machine-id-commit.service.8.gz

/usr/share/man/man8/systemd-network-generator.8.gz

/usr/share/man/man8/systemd-network-generator.service.8.gz

/usr/share/man/man8/systemd-pcrfs-root.service.8.gz

/usr/share/man/man8/systemd-pcrfs@.service.8.gz

/usr/share/man/man8/systemd-pcrmachine.service.8.gz

/usr/share/man/man8/systemd-poweroff.service.8.gz

/usr/share/man/man8/systemd-rc-local-generator.8.gz

/usr/share/man/man8/systemd-reboot.service.8.gz

/usr/share/man/man8/systemd-run-generator.8.gz

/usr/share/man/man8/systemd-shutdown.8.gz

/usr/share/man/man8/systemd-socket-proxyd.8.gz

/usr/share/man/man8/systemd-sysext.8.gz

/usr/share/man/man8/systemd-sysext.service.8.gz

/usr/share/man/man8/systemd-system-update-generator.8.gz

/usr/share/man/man8/systemd-sysupdate-reboot.service.8.gz

/usr/share/man/man8/systemd-sysupdate-reboot.timer.8.gz

/usr/share/man/man8/systemd-sysupdate.8.gz

/usr/share/man/man8/systemd-sysupdate.service.8.gz

/usr/share/man/man8/systemd-sysupdate.timer.8.gz

/usr/share/man/man8/systemd-sysusers.8.gz

/usr/share/man/man8/systemd-sysusers.service.8.gz

/usr/share/man/man8/systemd-sysv-generator.8.gz

/usr/share/man/man8/systemd-timedated.8.gz

/usr/share/man/man8/systemd-timedated.service.8.gz

/usr/share/man/man8/systemd-tmpfiles-clean.service.8.gz

/usr/share/man/man8/systemd-tmpfiles-clean.timer.8.gz

/usr/share/man/man8/systemd-tmpfiles-setup.service.8.gz

/usr/share/man/man8/systemd-tmpfiles.8.gz

/usr/share/man/man8/systemd-update-done.8.gz

/usr/share/man/man8/systemd-update-done.service.8.gz

/usr/share/man/man8/systemd-update-utmp-runlevel.service.8.gz

/usr/share/man/man8/systemd-update-utmp.8.gz

/usr/share/man/man8/systemd-update-utmp.service.8.gz

/usr/share/man/man8/systemd-user-sessions.8.gz

/usr/share/man/man8/systemd-user-sessions.service.8.gz

/usr/share/man/man8/systemd-xdg-autostart-generator.8.gz

/usr/share/man/man8/telinit.8.gz

/usr/share/pkgconfig/systemd.pc

/usr/share/pkgconfig/udev.pc

/usr/share/polkit-1/actions/org.freedesktop.hostname1.policy

/usr/share/polkit-1/actions/org.freedesktop.locale1.policy

/usr/share/polkit-1/actions/org.freedesktop.login1.policy

/usr/share/polkit-1/actions/org.freedesktop.systemd1.policy

/usr/share/polkit-1/actions/org.freedesktop.timedate1.policy

/usr/share/selinux

/usr/share/selinux/packages

/usr/share/selinux/packages/targeted

/usr/share/selinux/packages/targeted/systemd-container-coredump.pp.bz2

/usr/share/systemd

/usr/share/systemd/kbd-model-map

/usr/share/systemd/language-fallback-map

/usr/share/zsh/site-functions/_busctl

/usr/share/zsh/site-functions/_hostnamectl

/usr/share/zsh/site-functions/_journalctl

/usr/share/zsh/site-functions/_localectl

/usr/share/zsh/site-functions/_loginctl

/usr/share/zsh/site-functions/_sd_hosts_or_user_at_host

/usr/share/zsh/site-functions/_sd_machines

/usr/share/zsh/site-functions/_sd_outputmodes

/usr/share/zsh/site-functions/_sd_unit_files

/usr/share/zsh/site-functions/_systemctl

/usr/share/zsh/site-functions/_systemd

/usr/share/zsh/site-functions/_systemd-analyze

/usr/share/zsh/site-functions/_systemd-delta

/usr/share/zsh/site-functions/_systemd-inhibit

/usr/share/zsh/site-functions/_systemd-path

/usr/share/zsh/site-functions/_systemd-run

/usr/share/zsh/site-functions/_systemd-tmpfiles

/usr/share/zsh/site-functions/_timedatectl

/var/cache/private

/var/lib/private

/var/lib/private/systemd

/var/lib/rpm-state/systemd

/var/lib/selinux/targeted/active/modules/200/systemd-container-coredump

/var/lib/systemd

/var/lib/systemd/catalog

/var/lib/systemd/catalog/database

/var/lib/systemd/linger

/var/log/btmp

/var/log/journal

/var/log/lastlog

/var/log/private

/var/log/wtmp

[root@rocky14 ~]# rpm -qR systemd

/bin/sh

/bin/sh

/bin/sh

/bin/sh

/bin/sh

/usr/bin/bash

/usr/bin/getent

/usr/bin/sh

/usr/sbin/groupadd

acl

config(systemd) = 252-46.el9_5.2.0.1

coreutils

coreutils

dbus >= 1.9.18

grep

ld-linux-x86-64.so.2()(64bit)

ld-linux-x86-64.so.2(GLIBC_2.3)(64bit)

libacl.so.1()(64bit)

libacl.so.1(ACL_1.0)(64bit)

libaudit.so.1()(64bit)

libblkid.so.1()(64bit)

libblkid.so.1(BLKID_2.15)(64bit)

libblkid.so.1(BLKID_2.17)(64bit)

libblkid.so.1(BLKID_2.18)(64bit)

libblkid.so.1(BLKID_2.30)(64bit)

libbz2.so.1()(64bit)

libc.so.6()(64bit)

libc.so.6(GLIBC_2.10)(64bit)

libc.so.6(GLIBC_2.11)(64bit)

libc.so.6(GLIBC_2.14)(64bit)

libc.so.6(GLIBC_2.16)(64bit)

libc.so.6(GLIBC_2.17)(64bit)

libc.so.6(GLIBC_2.2.5)(64bit)

libc.so.6(GLIBC_2.22)(64bit)

libc.so.6(GLIBC_2.25)(64bit)

libc.so.6(GLIBC_2.26)(64bit)

libc.so.6(GLIBC_2.27)(64bit)

libc.so.6(GLIBC_2.28)(64bit)

libc.so.6(GLIBC_2.3)(64bit)

libc.so.6(GLIBC_2.3.2)(64bit)

libc.so.6(GLIBC_2.3.4)(64bit)

libc.so.6(GLIBC_2.30)(64bit)

libc.so.6(GLIBC_2.32)(64bit)

libc.so.6(GLIBC_2.33)(64bit)

libc.so.6(GLIBC_2.34)(64bit)

libc.so.6(GLIBC_2.4)(64bit)

libc.so.6(GLIBC_2.5)(64bit)

libc.so.6(GLIBC_2.6)(64bit)

libc.so.6(GLIBC_2.7)(64bit)

libc.so.6(GLIBC_2.8)(64bit)

libc.so.6(GLIBC_2.9)(64bit)

libcap.so.2()(64bit)

libcrypt.so.2()(64bit)

libcrypt.so.2(XCRYPT_2.0)(64bit)

libcrypt.so.2(XCRYPT_4.4)(64bit)

libcrypto.so.3()(64bit)

libcrypto.so.3(OPENSSL_3.0.0)(64bit)

libfdisk.so.1()(64bit)

libfdisk.so.1(FDISK_2.26)(64bit)

libgcc_s.so.1()(64bit)

libgcc_s.so.1(GCC_3.0)(64bit)

libgcc_s.so.1(GCC_3.3.1)(64bit)

libgcrypt.so.20()(64bit)

libgcrypt.so.20(GCRYPT_1.6)(64bit)

libkmod.so.2()(64bit)

libkmod.so.2(LIBKMOD_5)(64bit)

liblz4.so.1()(64bit)

liblzma.so.5()(64bit)

liblzma.so.5(XZ_5.0)(64bit)

libm.so.6()(64bit)

libm.so.6(GLIBC_2.2.5)(64bit)

libm.so.6(GLIBC_2.29)(64bit)

libmount.so.1()(64bit)

libmount.so.1(MOUNT_2.19)(64bit)

libmount.so.1(MOUNT_2.20)(64bit)

libmount.so.1(MOUNT_2.22)(64bit)

libmount.so.1(MOUNT_2.23)(64bit)

libmount.so.1(MOUNT_2.26)(64bit)

libp11-kit.so.0()(64bit)

libp11-kit.so.0(LIBP11_KIT_1.0)(64bit)

libpam.so.0()(64bit)

libpam.so.0(LIBPAM_1.0)(64bit)

libpam.so.0(LIBPAM_EXTENSION_1.0)(64bit)

libseccomp.so.2()(64bit)

libselinux-utils

libselinux.so.1()(64bit)

libselinux.so.1(LIBSELINUX_1.0)(64bit)

libsystemd-core-252.so()(64bit)

libsystemd-core-252.so(SD_SHARED)(64bit)

libsystemd-shared-252.so()(64bit)

libsystemd-shared-252.so(SD_SHARED)(64bit)

libz.so.1()(64bit)

libzstd.so.1()(64bit)

openssl-libs

pcre2(x86-64)

policycoreutils

rpmlib(CaretInVersions) <= 4.15.0-1

rpmlib(CompressedFileNames) <= 3.0.4-1

rpmlib(FileDigests) <= 4.6.0-1

rpmlib(PayloadFilesHavePrefix) <= 4.0-1

rpmlib(PayloadIsZstd) <= 5.4.18-1

rtld(GNU_HASH)

sed

selinux-policy

systemd-libs = 252-46.el9_5.2.0.1

systemd-pam = 252-46.el9_5.2.0.1

systemd-rpm-macros = 252-46.el9_5.2.0.1

util-linux

[root@rocky14 ~]# rpm -q -changelog systemd

* Sat Nov 16 2024 Release Engineering <releng@rockylinux.org> - 252-46.0.1

- Set support URL to the wiki

- Set sbat mail to security@rockylinux.org

  

* Tue Sep 10 2024 systemd maintenance team <systemd-maint@redhat.com> - 252-46.2

- add %posttrans scriptlet to make sure our SELinux policy module is actually installed (RHEL-46339)

  

* Tue Sep 03 2024 systemd maintenance team <systemd-maint@redhat.com> - 252-46.1

- version bump (RHEL-56019)

  

* Fri Aug 30 2024 systemd maintenance team <systemd-maint@redhat.com> - 252-46

- ukify: Skip test on architectures without UEFI (RHEL-56019)

  

* Sat Aug 24 2024 systemd team <systemd-maint@redhat.com> - 252-45

- build ukify without noarch

  

* Thu Aug 22 2024 systemd maintenance team <systemd-maint@redhat.com> - 252-44

- Revert "udev-builtin-net_id: use firmware_node/sun for ID_NET_NAME_SLOT" (RHEL-50103)

- fundamental: share constants for confidential virt detection (RHEL-50651)

- efi: add helper API for detecting confidential virtualization (RHEL-50651)

- efi: don't pull kernel cmdline from SMBIOS in a confidential VM (RHEL-50651)

- Fix detection of TDX confidential VM on Azure platform (RHEL-50651)

  

* Thu Aug 22 2024 systemd maintenance team <systemd-maint@redhat.com> - 252-43

- udev-builtin-net_id: skip non-directory entry earlier (RHEL-50103)

- udev-builtin-net_id: return earlier when hotplug slot is not found (RHEL-50103)

- udev-builtin-net_id: split-out pci_get_hotplug_slot() and pci_get_hotplug_slot_from_address() (RHEL-50103)

- udev-builtin-net_id: use firmware_node/sun for ID_NET_NAME_SLOT (RHEL-50103)

- Include <threads.h> if possible to get thread_local definition (RHEL-50651)

- add APIs for detecting confidential virtualization (RHEL-50651)

- detect-virt: add --cvm option (RHEL-50651)

- detect-virt: add --list-cvm option (RHEL-50651)

- unit: add "cvm" option for ConditionSecurity (RHEL-50651)

- dbus: add 'ConfidentialVirtualization' property to manager object (RHEL-50651)

- core: log detected confidential virtualization type (RHEL-50651)

- core: set SYSTEMD_CONFIDENTIAL_VIRTUALIZATION env for generators (RHEL-50651)

- udev: add 'conf-virt' constant for confidential virtualization tech (RHEL-50651)

- confidential-virt: split caching of CVM detection into separate method (RHEL-50651)

- confidential-virt: add detection for s390x target (RHEL-50651)

- man/systemd-detect-virt: list known CVM technologies (RHEL-50651)

  

* Mon Aug 19 2024 systemd team <systemd-maint@redhat.com>

- fix applying patches

  

* Thu Aug 15 2024 systemd maintenance team <systemd-maint@redhat.com> - 252-41

- timedatectl: setting set_local_rtc to 1 will throw Warning as well, use log_warning() (#33489) (RHEL-45020)

- cryptsetup-tokens: fix pin asserts (RHEL-36276)

- cryptenroll: Use CTAP2.1 credProtect extension (RHEL-36276)

- kernel-install: check machine ID (RHEL-50672)

- kernel-install: ignore errors when reading /etc/machine-id (RHEL-50672)

- hwdb: Add Lenovo G580 (RHEL-5950)

- Fix key toggle and programmable button for Positivo N14ZP (RHEL-5950)

- hwdb: Add accel orientation quirk for the Acer Switch V 10 SW5-017 2-in-1 (RHEL-5950)

- hwdb: fix Compaq N14KP6 key toggle touchpad (#25404) (RHEL-5950)

- hwdb: remove fuzz and deadzone for Simucube wheel bases. (RHEL-5950)

- hwdb: Add support for Elgato Stream Pedal (#25550) (RHEL-5950)

- hwdb: add Clevo touchpad toggle key quirks (RHEL-5950)

- hwdb: add Dell Inspiron N4010 touchpad corrections (RHEL-5950)

- hwdb: add Positivo-vaio Pro PW key toggle touchpad (#25669) (RHEL-5950)

- Add mount matrix for VisionBook 12Wr Tab (RHEL-5950)

- Update 60-evdev.hwdb (#25704) (RHEL-5950)

- hwdb: Add additional Dell models that require ACCEL_LOCATION=base (#25724) (RHEL-5950)

- hwdb: drop trailing space (RHEL-5950)

- hwdb: add comments about matching entries (RHEL-5950)

- hwdb: also add a generic entry for DualPoint Stick (RHEL-5950)

- hwdb: Add mount matrix for CSL Panther Tab HD (RHEL-5950)

- hwdb: Fix mount matrix for CSL Panther Tab HD (#25752) (RHEL-5950)

- hwdb: Fn+F5 fix for MSI Bravo 15-B5DX (#25788) (RHEL-5950)

- hwdb: change definition of PROXIMITY_NEAR_LEVEL for sensors (RHEL-5950)

- hwdb: Add mic-mute, control-center and screen-rotation mappings for MSI laptops (RHEL-5950)

- Prevents airplane mode toggle for HP Spectre 16 (RHEL-5950)

- Update 60-sensor.hwdb (RHEL-5950)

- Added Tablet Teclast X98 Air 3G (C5J6) (RHEL-5950)

- hwdb: remove spurious whitespace (RHEL-5950)

- hwdb: Add Dell models that require ACCEL_LOCATION=base (RHEL-5950)

- Fix Positivo MASTER-N1110 key toggle touchpad (RHEL-5950)

- hwdb: Mark Dell platform accel sensor location to base (RHEL-5950)

- hwdb: Add mount matrix for Linx 1020 (RHEL-5950)

- hwdb: Add mic mute key mappings for Dell G16 Series (RHEL-5950)

- hwdb: Add Chuwi Hi10X (N4120 version) iio matrix (RHEL-5950)

- hwdb: Add touchpad toggle mapping for System76 Pangolin 12 (RHEL-5950)

- hwdb: Prevent activation of airplane mode on HP ENVY x360 (RHEL-5950)

- Update hwdb (RHEL-5950)

- hwdb: update (RHEL-5950)

- hwdb: update autosuspend db (RHEL-5950)

- hwdb: ieee1394-unit-function: add MOTU 896 mk3 Hybrid (RHEL-5950)

- Add hwdb sensor entry for Lenovo IdeaPad Duet 3 10IGL5 (82AT). (RHEL-5950)

- Fix Positivo-vaio VJPW12F11X key toggle touchpad (RHEL-5950)

- hwdb: Add HP Envy x360 Convertible 15-cn0xxx to existing entry (RHEL-5950)

- hwdb: add override for IdeaPad5 insert key (RHEL-5950)

- hwdb: update database (RHEL-5950)

- hwdb: Add HP ENVY x360 2-in-1 (RHEL-5950)

- hwdb: update (RHEL-5950)

- hwdb: fix swapped buttons for Logitech Lift left (RHEL-5950)

- Revert "hwdb: fix swapped buttons for Logitech Lift left" (RHEL-5950)

- hwdb: update 70-mouse.hwdb (#26782) (RHEL-5950)

- hwdb: 60-keyboard.hwdb: Fix modalias for Thinkpad X200 Tablet (#26795) (RHEL-5950)

- Add rebrands of Medion Akoya notebooks/tablets (RHEL-5950)

- hwdb: fix Wifi toggling for Haier 7G-Series/JWU (#25293) (#26878) (RHEL-5950)

- hwdb: drop boilerplate about match patterns in two more cases (RHEL-5950)

- hwdb: Fix incorrect touchpad dimensions on Thinkpad L14 Gen1 (#26937) (RHEL-5950)

- hwdb: drop redundant entry (RHEL-5950)

- hwdb: Fixed thumb buttons reversed on CHERRY MW 2310 (#26992) (RHEL-5950)

- hwdb: Move MSI touchpad-toggle mapping to generic MSI section (RHEL-5950)

- update 60-sensor.hwdb with toshiba tablet (#27103) (RHEL-5950)

- hwdb: Add support for "Passion Model P612F" (RHEL-5950)

- hwdb: fix ambiguous glob pattern for Lenovo machines (RHEL-5950)

- hwdb: add matrix for Asus BR1100F (#27197) (RHEL-5950)

- hwdb: add accelerometer mount matrix for Lenovo Yoga Tablet 2 851F/L (RHEL-5950)

- hwdb: Fix rotation for BMAX Y13 (RHEL-5950)

- hwdb: disable entry for Logitech USB receiver used by G502 X (RHEL-5950)

- hwdb: add hardware rfkill key for Dell Latitude E6* models (#27462) (RHEL-5950)

- hwdb: do not include '#' in modalias (RHEL-5950)

- hwdb: add landscape IdeaPad Miix 310 sensor orientation (#27555) (RHEL-5950)

- Fix Positivo CF40CM-V2 key toggle touchpad (RHEL-5950)

- hwdb: fix keyboard entry for IdeapadFlex5 (#27643) (RHEL-5950)

- hwdb: fix Positivo CG15D key toggle touchpad and programmable keys (#27689) (RHEL-5950)

- hwdb: add support for Elgato Stream Deck mini (gen 2) (RHEL-5950)

- hwdb: fix arrow keys on HP Elite Dragonfly G3 (RHEL-5950)

- hwdb: add support for Jun Tab2/Dere T11 to 60-sensor.hwdb (#28092) (RHEL-5950)

- hwdb: fix volume control keys on Lenovo IdeaPad Flex 5 (14ARE05) (RHEL-5950)

- hwdb: Add override for headset form-factors (RHEL-5950)

- hwdb : add support for Archos 101 Cesium Educ to 60-sensor.hwdb (RHEL-5950)

- hwdb: drop trailing white space (RHEL-5950)

- hwdb: merge multiple keyboard entries with same setting (RHEL-5950)

- hwdb: make matching modalias for Archos 101 Cesium Educ more strict (RHEL-5950)

- hwdb update for v246-rc1 (RHEL-5950)

- update hwdb autosuspend data for v254 (RHEL-5950)

- hwdb: add support for Archos 101 Cesium to 60-sensor.hwdb (#28270) (RHEL-5950)

- Hwdb: Add Sanwa Direct 400-MA128 external trackpad (#28272) (RHEL-5950)

- hwdb: drop POINTINGSTICK_CONST_ACCEL (RHEL-5950)

- Add alternate name for MX Ergo as found on some devices (RHEL-5950)

- Update hwdb (RHEL-5950)

- hwdb: run update-hwdb (RHEL-5950)

- hwdb: run update-hwdb (RHEL-5950)

- hwdb: Mute SW rfkill keys on MSI Wind U100 (RHEL-5950)

- Update 60-sensor.hwdb (#28804) (RHEL-5950)

- hwdb: Added config for RCA W101SA23T1 (#29041) (RHEL-5950)

- Update 60-input-id.hwdb: add TEX Shinobi (#29068) (RHEL-5950)

- hwdb: keyboard: D330 FnLk toggle (RHEL-5950)

- hwdb: Add Logitech G502 X (RHEL-5950)

- hwdb: ieee1394-unit-function: remove superfluous Weiss Engineering DAC1 entry (RHEL-5950)

- hwdb: ieee1394-unit-function: add Weiss Engineering DAC202 (Maya edition) (RHEL-5950)

- hwdb: ieee1394-unit-function: add Weiss Engineering INT203 entry with older firmware (RHEL-5950)

- hwdb: ieee1394-unit-function: add Weiss Engieering MAN301 (RHEL-5950)

- hwdb: Add quirk for teclast x3 plus (G4K3) rotation (#29202) (RHEL-5950)

- hwdb: add mic mute key mappings for Acer Predator Triton 300 SE (RHEL-5950)

- hwdb: Bush tablet rotation support (#29268) (RHEL-5950)

- hwdb: ieee1394-unit-function: add Miglia Technology Harmony Audio (HA02) (RHEL-5950)

- add support for hp pavilion gaming 15 lid switch (#29304) (RHEL-5950)

- Fix Positivo N14EP6 key toggle touchpad and programmable keys (#29448) (RHEL-5950)

- add udev rule for micmute (f20) (RHEL-5950)

- hwdb,rules: mark host-to-host network devices as only requiring link local addressing (RHEL-5950)

- Update hwdb (RHEL-5950)

- Update hwdb autosuspend rules (RHEL-5950)

- Update hwdb (RHEL-5950)

- hwdb: Add accelerometer data for Librem11 (#29974) (RHEL-5950)

- hwdb: PNP/ACPI lists on uefi.org are now in CSV format (RHEL-5950)

- Update hwdb (RHEL-5950)

- hwdb: rename .html=>.csv (RHEL-5950)

- hwdb/acpi-update.py: streamline python code (RHEL-5950)

- hwdb: Mark Dell platform accel sensor location to base (RHEL-5950)

- hwdb: add Predator PHN16-71 (RHEL-5950)

- Update 60-autosuspend.hwdb (#30131) (RHEL-5950)

- hwdb: update (RHEL-5950)

- hwdb: ieee1394-unit-function: add Sony DVMC-DA1 (RHEL-5950)

- hwdb: ieee1394-unit-function: arrangement for Sony DVMC-DA1 (RHEL-5950)

- hwdb: update (RHEL-5950)

- hwdb: update (RHEL-5950)

- Adding Trekstor Primebook C13 rotation to 60-sensor.hwdb (#30415) (RHEL-5950)

- Add three Dell platforms to sensor accel location base (RHEL-5950)

- Add Bosto BT-12HD series to hwdb (RHEL-5950)

- hwdb: Add override for headset form-factor for the Corsair Void Elite (RHEL-5950)

- hwdb: add Teclast X98 Pro sensor info (#30859) (RHEL-5950)

- hwdb: Correct display rotation on Chuwi Ubook X N4100 (#24248) (RHEL-5950)

- hwdb: ieee1394-unit-function: adjustment of entries with device attributes available in Linux v6.8 (RHEL-5950)

- 60-evdev.hwdb: Add support for Huion Inspiroy 2 L (#31241) (RHEL-5950)

- hwdb: add resolution setting for GAOMON S620 (RHEL-5950)

- hwdb: Remove version check in CH Pro Pedals rule (RHEL-5950)

- hwdb: Add support for MetawillBook01 to 60-sensor.hwdb Add accel orientation quirk for the METAPHYUNI MetawillBook01 2-in-1 laptop (RHEL-5950)

- hwdb: Add headset form-factor override for Xbox Wireless Dongle (RHEL-5950)

- hwdb: Add support for Elgato Stream Deck Plus (RHEL-5950)

- Fix: Chuwi UBook X (CWI535) screen rotation matrix (RHEL-5950)

- hwdb: Add touchpad toggle mapping for Kvadra LE14U/LE15U (RHEL-5950)

- hwdb: Add touchpad configuration for ThinkPad E495 (RHEL-5950)

- Fix Positivo N14NPE-N and N15NPE-N key toggle touchpad and search key (RHEL-5950)

- Update USB ids of hwdb (RHEL-5950)

- Added resolution for Huion Kamvas Pro 19 (RHEL-5950)

- hwdb: Add mapping for ACPI quickstart keys on Toshiba Z830 (RHEL-5950)

- hwdb: fix Asus T300FA rotation matrix (#31973) (RHEL-5950)

- Fixed resolution for pen and touchpad (RHEL-5950)

- hwdb: fix missing colon (#32108) (RHEL-5950)

- hwdb: update for v256 (RHEL-5950)

- autosuspend: update for v256 (RHEL-5950)

- Update hwdb (RHEL-5950)

- Update autosuspend hwdb (RHEL-5950)

- Update hwdb (RHEL-5950)

- hwdb: Add a common Logitech M185/M225 mouse variant (RHEL-5950)

- hwdb: Add mapping for Samsung GalaxyBook - 550X (#32616) (RHEL-5950)

- hwdb: Add mapping for Xiaomi Mipad 2 bottom bezel capacitive buttons (RHEL-5950)

- hwdb: ieee1394-unit-function: add Tascam IF-FW/DM mkII (RHEL-5950)

- hwdb: Add a Logitech MX Master 3S (connected via Bolt Receiver) (RHEL-5950)

- Fix Positivo N14EPE and N15EPE key toggle touchpad and search key (RHEL-5950)

- hwdb: update Dere N12 / Juno Tablet 3 accelerometer (#32765) (RHEL-5950)

- hwdb: updated Librem 11 accelerometer (#32772) (RHEL-5950)

- hwdb: ID_INPUT_XYZ allows an empty string (RHEL-5950)

- hwdb: ASRock LED Controller classified incorrectly as joystick due to buttons and axis (#32775) (RHEL-5950)

- Update hwdb (RHEL-5950)

- hwdb.d/60-keyboard.hwdb: enable Clevo quirk for model V5x0TU (RHEL-5950)

- hwdb: Enable JP-IK LEAP W502's touchpad toggle key (RHEL-5950)

- Update hwdb (RHEL-5950)

- Update autosuspend hwdb (RHEL-5950)

- hwdb: Lenovo IdeaPad Z500 Touchpad Toggle (#33039) (RHEL-5950)

- hwdb: add a vmbus id for HyperV Video device (RHEL-5950)

- hwdb: Add Logitech MX Master 3S Bluetooth ID (RHEL-5950)

- hwdb: Lenovo 16G6IRL volume keys and friends (#33107) (RHEL-5950)

- hwdb: added hwdb rules for micmute and power button on Acer Nitro AN 515-58 (#32867) (RHEL-5950)

- Fix key toggle touchpad and programmable buttom for Positivo N14AP7 (RHEL-5950)

- Update hwdb (RHEL-5950)

- hwdb: add keyboard mappings for the Ayaneo Kun face buttons (RHEL-5950)

- Update hwdb (RHEL-5950)

- hwdb: add support for AIPTEK Media Tablet Ultimate (#33371) (RHEL-5950)

- hwdb: add scancodes for AYANEO devices (#33378) (RHEL-5950)

- Add OrangePi NEO Scancodes (RHEL-5950)

- hwdb: Fix Logitech G915 TKL (Bluetooth) appearing as a mouse (RHEL-5950)

- hwdb: fix keyboard of RedmiBook Pro 15 2022 (#33465) (RHEL-5950)

- Added mised EVDEV_ABS_35 & EVDEV_ABS_36 for GAOMON s620 (RHEL-5950)

- hwdb: Add some HP IR cameras (RHEL-5950)

- hwdb: add more AV controllers (RHEL-5950)

- Fix key toggle touchpad button for multilaser ul154 (#33630) (RHEL-5950)

- hwdb: Added StarLabs StarLite position sensor mapping (RHEL-5950)

- 70-mouse.hwdb: Added Glorious Model O DPI (RHEL-5950)

- Update 60-sensor.hwdb (RHEL-5950)

- Add MSI Claw AT Keyboard Scancodes. (RHEL-5950)

- Add or fix mount matrix for multiple handhelds. (#33586) (RHEL-5950)

- Revert "hwdb: Added StarLabs StarLite position sensor mapping" (RHEL-5950)

- hwdb: fix accelerometer mount matrix for Aquarius Cmp NS483 (RHEL-5950)

- hwdb: add backslash and touchpad toggle mapping for Aquarius Cmp NS483 (RHEL-5950)

- hwdb: Add mic mute key mapping for Dell Pro Rugged series (RHEL-5950)

- hwdb: fix MXC6655 accelerometer mount matrix for Aquarius Cmp NS483 (RHEL-5950)

- add udev rules for trezor hw wallet devices (RHEL-5950)

- hwdb: add axis range corrections for the Lenovo Thinkpad E16 (RHEL-5950)

- hwdb: fix auto rotate on Asus Q551LB (#33921) (RHEL-5950)

- udev: add hwdb execution for hidraw subsystem devices (RHEL-5950)

  

* Wed Aug 07 2024 systemd maintenance team <systemd-maint@redhat.com> - 252-40

- add Requires(post) on selinux-policy (RHEL-46339)

  

* Wed Jul 17 2024 systemd maintenance team <systemd-maint@redhat.com> - 252-39

- enable FIDO2 support (RHEL-36276)

- netif-naming-scheme: disable NAMING_BRIDGE_MULTIFUNCTION_SLOT (RHEL-44630)

- netif-naming-scheme: make actually possible to use rhel-9.5 scheme (RHEL-44630)

- generator: "uninline" generator_open_unit_file and generator_add_symlink (RHEL-33436)

- ci: add support for rhel-only parameters (RHEL-30372)

  

* Wed Jun 19 2024 systemd maintenance team <systemd-maint@redhat.com> - 252-38

- tools: fix the file name that "meson setup" generates (RHEL-30372)

- tools: explicitly specify "setup" subcommand (RHEL-30372)

- fuzz: pass -Dc_args=/-Dcpp_args= to fuzzer targets (RHEL-30372)

- fuzz: don't panic without a C++ compiler (RHEL-30372)

- meson: use ternary op for brevity (RHEL-30372)

  

* Thu Jun 13 2024 systemd maintenance team <systemd-maint@redhat.com> - 252-37

- ci(src-git): add RHEL-9.1 and RHEL-9.1.z to allowed versions (RHEL-30372)

- libsystemd: link with '-z nodelete' (RHEL-6589)

- basic/utf8: make utf8_encoded_to_unichar() return length of the codepoint (RHEL-31219)

- test-gunicode: add new test to show that unichar_iswide() is borked (RHEL-31219)

- string-util: pass ANSI sequences through unchanged (RHEL-31219)

- cryptsetup: do not assert when unsealing token without salt (RHEL-38864)

- cryptsetup: check the existence of salt by salt_size > 0 (RHEL-38864)

- core/mount: if umount(8) fails but mount disappeared, assume success (RHEL-13159)

- Drop log level of header limits log message (RHEL-33890)

- journal: do not rotate unrelated journal files when full or corrupted (RHEL-33890)

- man: suffix --unit with an equal sign, since it expects an argument (RHEL-31070)

- shared: move uid-alloc-range.[ch] from src/shared/ → src/basic/ (RHEL-31070)

- journald: move uid_for_system_journal() to uid-alloc-range.h (RHEL-31070)

- sd-journal: when SD_JOURNAL_CURRENT_USER is set, and called from system UID, imply SD_JOURNAL_SYSTEM (RHEL-31070)

- man: document that journalctl --user requires Storage=persistent (RHEL-31070)

- fix: prefix of dmesg pstore files (RHEL-20322)

- backport new mkosi (RHEL-27512)

- test: Skip various tests when /sys is not mounted (RHEL-27512)

- string-util: introduce ascii_ishex() (RHEL-27512)

- sd-id128: several cleanups (RHEL-27512)

- sd-id128: make id128_read() or friends return -ENOPKG when the file contents is "uninitialized" (RHEL-27512)

- test: add tests for "uninitialized" string handling by id128_read_fd() (RHEL-27512)

- man: mention sd_id128_get_machine() or friend may return -ENOPKG (RHEL-27512)

- sd-id128: make sd_id128_get_boot() and friend return -ENOMEDIUM (RHEL-27512)

- sd-id128: make sd_id128_get_boot() and friend return -ENOSYS when /proc/ is not mounted (RHEL-27512)

- man: mention that sd_id128_get_boot() and friend may return -ENOSYS (RHEL-27512)

- sd-id128: fold do_sync flag into Id128FormatFlag (RHEL-27512)

- sd-id128: make sd_id128_get_machine() or friends return -EUCLEAN when an ID is in an invalid format (RHEL-27512)

- sd-id128: allow sd_id128_get_machine() and friend to be called with NULL (RHEL-27512)

- sd-id128: also refuse an empty invocation ID (RHEL-27512)

- man: update documents for sd_id128_get_invocation() (RHEL-27512)

- test-id128: simplify machine-id check (RHEL-27512)

- test-fs-util: skip part of test_chase_symlinks if machine-id is not initialized (RHEL-27512)

- test-unit-name: simplify machine-id check (RHEL-27512)

- test-load-fragment: simplify machine-id check (RHEL-27512)

- journal: skip part of test-journal-interleaving if no machine-id exists (RHEL-27512)

- test: skip journal tests without valid /etc/machine-id (RHEL-27512)

- test-recurse-dir: work around nftw() ignoring symlinks() (RHEL-27512)

- test: Skip test-recurse-dir on overlayfs (RHEL-27512)

- test-specifier: Ignore -ENOPKG from specifier_printf() (RHEL-27512)

- test-execute: Skip when /sys is read-only (RHEL-27512)

- kernel-install: Make sure KERNEL_INSTALL_BYPASS is disabled in tests (RHEL-27512)

- tools: make sure $KERNEL_INSTALL_BYPASS is disabled when checking help (RHEL-27512)

- test-execute: drop capabilities when testing with user manager (RHEL-27512)

- tmpfiles: Add merge support for copy files action (RHEL-27512)

- generator: add generator_open_unit_file_full to allow creating temporary units (RHEL-27512)

- network-generator: rewrite unit if it already exists and its content changed (RHEL-27512)

- ci: drop super-linter's shellcheck (RHEL-27512)

- mkosi: make sure we build & use RHEL 9 stuff (RHEL-27512)

- ci: backport mkosi CI configuration from upstream (RHEL-27512)

- mkosi: explicitly enroll SecureBoot keys (RHEL-27512)

- test-execute: also mount tmpfs on /dev/shm (RHEL-27512)

- mkosi: fix UKI addons test (RHEL-27512)

- Revert "mkosi: Disable cmdline addon test for now" (RHEL-27512)

- Revert "mkosi: Don't fail on systemd-vconsole-setup.service failure for now" (RHEL-27512)

- mkosi: make shellcheck happy (RHEL-27512)

- mkosi: use pesign for signing UKI addons (RHEL-27512)

- test: copy out the necessary test data before we start overmounting stuff (RHEL-27512)

- ci: make the build dir accessible when running w/o privileges (RHEL-27512)

- ci: explicitly change oom-{score}-adj before running tests (RHEL-27512)

- ratelimit: add ratelimit_left helper (RHEL-35703)

- manager: restrict Dump*() to privileged callers or ratelimit (RHEL-35703)

- ci: define `runas` function inline (RHEL-35703)

- Drop /dev test in test-mountpoint-util (RHEL-30372)

- core/manager: export manager_dbus_is_running (RHEL-40878)

- core: refuse dbus activation if dbus is not running (RHEL-40878)

- core: only refuse Type=dbus service enqueuing if dbus has stop job (RHEL-40878)

- Revert "core/manager: export manager_dbus_is_running" and partially "core: refuse dbus activation if dbus is not running" (RHEL-40878)

- manager: fix reloading in reload-or-restart --marked (RHEL-40878)

- rpm: add `systemd_postun_with_reload` and `systemd_user_postun_with_reload` (RHEL-40878)

- rpm: add `systemd_user_daemon_reexec` (RHEL-40878)

  

* Wed May 22 2024 Jan Macku <jamacku@redhat.com> - 252-35

- spec: return selinux dependencies (RHEL-35732)

  

* Mon May 20 2024 systemd maintenance team <systemd-maint@redhat.com> - 252-34

- ci: update actions/upload-artifact to v4 (RHEL-30372)

- journal-remote: code is of type enum MHD_RequestTerminationCode (RHEL-30372)

- resolve: dns_server_feature_level_*_string type is DnsServerFeatureLevel (RHEL-30372)

- shared|install: Use InstallChangeType consistently (RHEL-30372)

- test: temporarily disable coredumps in testsuite-17.03.sh (RHEL-30372)

- ci: update manpage deployment workflow (RHEL-30372)

- bootspec: fix null-dereference-read (RHEL-36284)

- units: don't install pcrphase-related units without gnu-efi (RHEL-33384)

- kernel-install: fix uki-copy deinstall (RHEL-36505)

- ci(packit): explicitly clone `c9s` branch (RHEL-30372)

  

* Fri Apr 26 2024 systemd maintenance team <systemd-maint@redhat.com> - 252-33

- execute: Pass AT_FDCWD instead of -1 (RHEL-31783)

- ci(src-git): update list of supported products (RHEL-30372)

- coredump: by default process and store core files up to 1GiB (RHEL-15501)

- coredump: keep core files for two weeks (RHEL-15501)

- ukify: make the test happy with the latest OpenSSL (RHEL-30372)

- test_ukify: use raw string for the regex (RHEL-30372)

- coredump: generate stacktraces also for processes running in containers w/o coredump forwarding (RHEL-29430)

- test: add a couple of tests for systemd-coredump (RHEL-29430)

- test: don't expand the subshell expression prematurely (RHEL-29430)

- coredump filter: fix stack overflow with =all (RHEL-29430)

- coredump filter: add mask for 'all' using UINT32_MAX, not UINT64_MAX (RHEL-29430)

- test: add coverage for CoredumpFilter=all (RHEL-29430)

- test: rotate journal before storing coredumps (RHEL-29430)

- test: sync with the fake binary before killing it (RHEL-29430)

- test: check coredump handling in containers & namespaces (RHEL-29430)

  

* Mon Mar 18 2024 Jan Macku <jamacku@redhat.com> - 252-32

- rebase rhel-net-naming-sysattrs to v0.5

  

* Fri Mar 15 2024 systemd maintenance team <systemd-maint@redhat.com> - 252-31

- bootctl: rework random seed logic to use open_mkdir_at() and openat() (RHEL-16952)

- bootctl: properly sync fs before/after moving random seed file into place (RHEL-16952)

- bootctl: when updating EFI random seed file, hash old seed with new one (RHEL-16952)

- sha256: add helper than hashes a buffer *and* its size (RHEL-16952)

- random-seed: don't refresh EFI random seed from random-seed.c anymore (RHEL-16952)

- bootctl: downgrade graceful messages to LOG_NOTICE (RHEL-16952)

- units: rename/rework systemd-boot-system-token.service → systemd-boot-random-seed.service (RHEL-16952)

- bootctl: split out setting of system token into function of its own (RHEL-16952)

  

* Mon Mar 11 2024 systemd maintenance team <systemd-maint@redhat.com> - 252-30

- resolved: limit the number of signature validations in a transaction (RHEL-26643)

- resolved: reduce the maximum nsec3 iterations to 100 (RHEL-26643)

- efi: alignment of the PE file has to be at least 512 bytes (RHEL-26133)

- units: change assert to condition to skip running in initrd/os (RHEL-16182)

- ci: add configuration for regression sniffer GA (RHEL-1086)

  

* Mon Feb 26 2024 systemd maintenance team <systemd-maint@redhat.com> - 252-29

- units: fix typo in Condition in systemd-boot-system-token (RHEL-16952)

  

* Tue Feb 20 2024 systemd maintenance team <systemd-maint@redhat.com> - 252-28

- random-seed: shorten a bit may_credit() (RHEL-16952)

- random-seed: make one more use of random_write_entropy() (RHEL-16952)

- random-seed: use getopt() (RHEL-16952)

- random-seed: make the logic to calculate the number of bytes read from the random seed file clearer (RHEL-16952)

- random-seed: no need to pass 'mode' argument when opening /dev/urandom (RHEL-16952)

- random-seed: split out run() (RHEL-16952)

- random_seed: minor improvement in run() (RHEL-16952)

- random-seed: downgrade some messages (RHEL-16952)

- random-seed: clarify one comment (RHEL-16952)

- random-seed: make sure to load machine id even if the seed file is missing (RHEL-16952)

- chase-symlinks: add new flag for prohibiting any following of symlinks (RHEL-16952)

- bootctl,bootspec: make use of CHASE_PROHIBIT_SYMLINKS whenever we access the ESP/XBOOTLDR (RHEL-16952)

- boot: implement kernel EFI RNG seed protocol with proper hashing (RHEL-16952)

- random-seed: refresh EFI boot seed when writing a new seed (RHEL-16952)

- random-seed: handle post-merge review nits (RHEL-16952)

- boot: do not truncate random seed file (RHEL-16952)

- bootctl: install system token on virtualized systems (RHEL-16952)

- boot: remove random-seed-mode (RHEL-16952)

- stub: handle random seed like sd-boot does (RHEL-16952)

- efi: add efi_guid_equal() helper (RHEL-16952)

- efi: add common implementation for loop finding EFI configuration tables (RHEL-16952)

- boot: Detect hypervisors using SMBIOS info (RHEL-16952)

- boot: Skip soft-brick warning when in a VM (RHEL-16952)

- boot: Replace UINTN with size_t (RHEL-16952)

- boot: Use unsigned for beep counting (RHEL-16952)

- boot: Use unicode literals (RHEL-16952)

- macro: add generic IS_ALIGNED32() anf friends (RHEL-16952)

- meson: use 0|1 for SD_BOOT (RHEL-16952)

- boot: Add printf functions (RHEL-16952)

- boot: Use printf for error logging (RHEL-16952)

- boot: Introduce log_wait (RHEL-16952)

- boot: Add log_trace debugging helper (RHEL-16952)

- tree-wide: Use __func__ in asserts (RHEL-16952)

- boot: Drop use of xpool_print/SPrint (RHEL-16952)

- boot: Drop use of Print (RHEL-16952)

- boot: Rework GUID handling (RHEL-16952)

- efi-string: Fix strchr() null byte handling (RHEL-16952)

- efi-string: Add startswith8() (RHEL-16952)

- efi-string: Add efi_memchr() (RHEL-16952)

- vmm: Add more const (RHEL-16952)

- vmm: Add smbios_find_oem_string() (RHEL-16952)

- stub: Read extra kernel command line items from SMBIOS (RHEL-16952)

- vmm: Modernize get_smbios_table() (RHEL-16952)

- stub: measure SMBIOS kernel-cmdline-extra in PCR12 (RHEL-16952)

- efi: support passing empty cmdline to mangle_stub_cmdline() (RHEL-16952)

- efi: set EFIVAR to stop Shim from uninstalling its protocol (RHEL-16952)

- ukify: use empty stub for addons (RHEL-16952)

- stub: allow loading and verifying cmdline addons (RHEL-16952)

- TODO: remove fixed item (RHEL-16952)

- fix: do not check/verify slice units if recursive errors are to be ignored (RHEL-1086)

  

* Thu Feb 15 2024 systemd maintenance team <systemd-maint@redhat.com> - 252-27

- test: merge TEST-20-MAINPIDGAMES into TEST-07-PID1 (fixup) (RHEL-1086)

- test: use the default nsec3-iterations value (RHEL-1086)

- test: explicitly set nsec3-iterations to 0 (RHEL-1086)

- core: mount namespaces: Remove auxiliary bind mounts directory after unit termination (RHEL-19483)

- ci: deploy systemd man to GitHub Pages (RHEL-1086)

- doc: add missing `<listitem>` to `systemd.net-naming-scheme.xml` (RHEL-7026)

- man: reorder the list of supported naming schemes (RHEL-7026)

- tree-wide: fix return value handling of base64mem() (RHEL-16182)

- Consolidate various TAKE_* into TAKE_GENERIC(), add TAKE_STRUCT() (RHEL-16182)

- pcrphase: add $SYSTEMD_PCRPHASE_STUB_VERIFY env var for overriding stub check (RHEL-16182)

- pcrphase: gracefully exit if TPM2 support is incomplete (RHEL-16182)

- tpm2-util: split out code that derives "good" TPM2 banks into an strv from pcrphase and generalize it in tpm2-util.c (RHEL-16182)

- tpm2-util: split out code that extends a PCR from pcrphase (RHEL-16182)

- tpm2-util: optionally do HMAC in tpm2_extend_bytes() in case we process sensitive data (RHEL-16182)

- cryptsetup: add tpm2-measure-pcr= and tpm2-measure-bank= crypttab options (RHEL-16182)

- man: document the new crypttab measurement options (RHEL-16182)

- gpt-auto-generator: automatically measure root/var volume keys into PCR 15 (RHEL-16182)

- blkid-util: define enum for blkid_do_safeprobe() return values (RHEL-16182)

- pcrphase: make tool more generic, reuse for measuring machine id/fs uuids (RHEL-16182)

- units: measure /etc/machine-id into PCR 15 during early boot (RHEL-16182)

- generators: optionally, measure file systems at boot (RHEL-16182)

- tpm2: add common helper for checking if we are running on UKI with TPM measurements (RHEL-16182)

- man: document new machine-id/fs measurement options (RHEL-16182)

- test: add simple integration test for checking PCR extension works as it should (RHEL-16182)

- update TODO (RHEL-16182)

- cryptsetup: retry TPM2 unseal operation if it fails with TPM2_RC_PCR_CHANGED (RHEL-16182)

- boot: Simplify object erasure (RHEL-16182)

- tree-wide: use CLEANUP_ERASE() at various places (RHEL-16182)

- dlfcn: add new safe_dclose() helper (RHEL-16182)

- tpm2: rename tpm2 alg id<->string functions (RHEL-16182)

- tpm2: rename struct tpm2_context to Tpm2Context (RHEL-16182)

- tpm2: use ref counter for Tpm2Context (RHEL-16182)

- tpm2: use Tpm2Context* instead of ESYS_CONTEXT* (RHEL-16182)

- tpm2: add Tpm2Handle with automatic cleanup (RHEL-16182)

- tpm2: simplify tpm2_seal() blob creation (RHEL-16182)

- tpm2: add salt to pin (RHEL-16182)

- basic/macro: add macro to iterate variadic args (RHEL-16182)

- test/test-macro: add tests for FOREACH_VA_ARGS() (RHEL-16182)

- basic/bitfield: add bitfield operations (RHEL-16182)

- test/test-bitfield: add tests for bitfield macros (RHEL-16182)

- tpm2: add tpm2_get_policy_digest() (RHEL-16182)

- tpm2: add TPM2_PCR_VALID() (RHEL-16182)

- tpm2: add/rename functions to manage pcr selections (RHEL-16182)

- test/test-tpm2: add tests for pcr selection functions (RHEL-16182)

- tpm2: add tpm2_pcr_read() (RHEL-16182)

- tpm2: move openssl-required ifdef code out of policy-building function (RHEL-16182)

- tpm2: add tpm2_is_encryption_session() (RHEL-16182)

- tpm2: move policy building out of policy session creation (RHEL-16182)

- tpm2: add support for a trusted SRK (RHEL-16182)

- tpm2: fix nits from PR #26185 (RHEL-16182)

- tpm2: replace magic number (RHEL-16182)

- tpm2: add tpm2_digest_*() functions (RHEL-16182)

- tpm2: replace hash_pin() with tpm2_digest_*() functions (RHEL-16182)

- tpm2: add tpm2_set_auth() (RHEL-16182)

- tpm2: add tpm2_get_name() (RHEL-16182)

- tpm2: rename pcr_values_size vars to n_pcr_values (RHEL-16182)

- tpm2: add tpm2_policy_pcr() (RHEL-16182)

- tpm2: add tpm2_policy_auth_value() (RHEL-16182)

- tpm2: add tpm2_policy_authorize() (RHEL-16182)

- tpm2: use tpm2_policy_authorize() (RHEL-16182)

- tpm2: add tpm2_calculate_sealing_policy() (RHEL-16182)

- tpm: remove external calls to dlopen_tpm2() (RHEL-16182)

- tpm2: remove all extern tpm2-tss symbols (RHEL-16182)

- tpm2: add tpm2_get_capability(), tpm2_cache_capabilities(), tpm2_capability_pcrs() (RHEL-16182)

- tpm2: verify symmetric parms in tpm2_context_new() (RHEL-16182)

- tpm2: replace _cleanup_tpm2_* macros with _cleanup_() (RHEL-16182)

- tpm2-util: use compound initialization when allocating tpm2 objects (RHEL-16182)

- tpm2: add tpm2_get_capability_handle(), tpm2_esys_handle_from_tpm_handle() (RHEL-16182)

- tpm2: add tpm2_read_public() (RHEL-16182)

- tpm2: add tpm2_get_legacy_template() and tpm2_get_srk_template() (RHEL-16182)

- tpm2: add tpm2_load() (RHEL-16182)

- tpm2: add tpm2_load_external() (RHEL-16182)

- tpm2: move local vars in tpm2_seal() to point of use (RHEL-16182)

- tpm2: replace magic number in hmac_sensitive initialization (RHEL-16182)

- tpm2: add tpm2_create() (RHEL-16182)

- tpm2: replace tpm2_capability_pcrs() macro with direct c->capaiblity_pcrs use (RHEL-16182)

- basic/alloc-util: add greedy_realloc_append() (RHEL-16182)

- tpm2: cache the TPM supported commands, add tpm2_supports_command() (RHEL-16182)

- tpm2: cache TPM algorithms (RHEL-16182)

- tpm2: add tpm2_persist_handle() (RHEL-16182)

- tpm2: add tpm2_get_or_create_srk() (RHEL-16182)

- tpm2: move local vars in tpm2_unseal() to point of use (RHEL-16182)

- tpm2: remove tpm2_make_primary() (RHEL-16182)

- tpm2: use CreatePrimary() to create primary keys instead of Create() (RHEL-16182)

- cryptsetup: downgrade a bunch of log messages that to LOG_WARNING (RHEL-16182)

- boot/measure: replace TPM PolicyPCR session with calculation (RHEL-16182)

- core: imply DeviceAllow=/dev/tpmrm0 with LoadCredentialEncrypted (RHEL-16182)

- added more test cases (RHEL-16182)

- test: fixed negative checks in TEST-70-TPM2. Use in-line error handling rather than redirections. Follow up on #27020 (RHEL-16182)

- systemd-cryptenroll: add string aliases for tpm2 PCRs Fixes #26697. RFE. (RHEL-16182)

- cryptenroll: fix an assertion with weak passwords (RHEL-16182)

- man/systemd-cryptenroll: update list of PCRs, link to uapi docs (RHEL-16182)

- tpm2: add debug logging to functions converting hash or asym algs to/from strings or ids (RHEL-16182)

- tpm2: add tpm2_hash_alg_to_size() (RHEL-16182)

- tpm2: change tpm2_tpm*_pcr_selection_to_mask() to return mask (RHEL-16182)

- tpm2: add more helper functions for managing TPML_PCR_SELECTION and TPMS_PCR_SELECTION (RHEL-16182)

- tpm2: add Tpm2PCRValue struct and associated functions (RHEL-16182)

- tpm2: move declared functions in header lower down (RHEL-16182)

- tpm2: declare tpm2_log_debug_*() functions in tpm2_util.h (RHEL-16182)

- tpm2: change tpm2_calculate_policy_pcr(), tpm2_calculate_sealing_policy() to use Tpm2PCRValue array (RHEL-16182)

- tpm2: change tpm2_parse_pcr_argument() parameters to parse to Tpm2PCRValue array (RHEL-16182)

- tpm2: add TPM2B_*_MAKE(), TPM2B_*_CHECK_SIZE() macros (RHEL-16182)

- tpm2: add tpm2_pcr_read_missing_values() (RHEL-16182)

- openssl: add openssl_pkey_from_pem() (RHEL-16182)

- openssl: add rsa_pkey_new(), rsa_pkey_from_n_e(), rsa_pkey_to_n_e() (RHEL-16182)

- openssl: add ecc_pkey_new(), ecc_pkey_from_curve_x_y(), ecc_pkey_to_curve_x_y() (RHEL-16182)

- test: add DEFINE_HEX_PTR() helper function (RHEL-16182)

- openssl: add test-openssl (RHEL-16182)

- tpm2: add functions to convert TPM2B_PUBLIC to/from openssl pkey or PEM (RHEL-16182)

- tpm2: move policy calculation out of tpm2_seal() (RHEL-16182)

- man: update systemd-cryptenroll man page with details on --tpm2-pcrs format change (RHEL-16182)

- tpm2: update TEST-70-TPM2 to test passing PCR value to systemd-cryptenroll (RHEL-16182)

- tpm2: change *alg_to_* functions to use switch() (RHEL-16182)

- tpm2: lowercase TPM2_PCR_VALUE[S]_VALID functions (RHEL-16182)

- tpm2: move cast from lhs to rhs in uint16_t/int comparison (RHEL-16182)

- tpm2: in validator functions, return false instead of assert failure (RHEL-16182)

- tpm2: in tpm2_pcr_values_valid() use FOREACH_ARRAY() (RHEL-16182)

- tpm2: use SIZE_MAX instead of strlen() for unhexmem() (RHEL-16182)

- tpm2: put !isempty() check inside previous !isempty() check (RHEL-16182)

- tpm2: simplify call to asprintf() (RHEL-16182)

- tpm2: check pcr value hash != 0 before looking up hash algorithm name (RHEL-16182)

- tpm2: use strempty() (RHEL-16182)

- tpm2: split TPM2_PCR_VALUE_MAKE() over multiple lines (RHEL-16182)

- tpm2: remove ret_ prefix from input/output params (RHEL-16182)

- tpm2: use memcpy_safe() instead of memcpy() (RHEL-16182)

- openssl: use new(char, size) instead of malloc(size) (RHEL-16182)

- tpm2: use table for openssl<->tpm2 ecc curve id mappings (RHEL-16182)

- tpm2: use switch() instead of if-else (RHEL-16182)

- tpm2: make logging level consistent at debug for some functions (RHEL-16182)

- tpm2: remove unnecessary void* cast (RHEL-16182)

- tpm2: add tpm2_pcr_values_has_(any|all)_values() functions (RHEL-16182)

- tpm2: wrap (7) in UINT32_C() (RHEL-16182)

- cryptenroll: change man page example to remove leading 0x and lowercase hex (RHEL-16182)

- openssl: add log_openssl_errors() (RHEL-16182)

- openssl: add openssl_digest_size() (RHEL-16182)

- openssl: add openssl_digest_many() (RHEL-16182)

- openssl: replace openssl_hash() with openssl_digest() (RHEL-16182)

- openssl: add openssl_hmac_many() (RHEL-16182)

- openssl: add rsa_oaep_encrypt_bytes() (RHEL-16182)

- openssl: add kdf_kb_hmac_derive() (RHEL-16182)

- openssl: add openssl_cipher_many() (RHEL-16182)

- openssl: add ecc_edch() (RHEL-16182)

- openssl: add kdf_ss_derive() (RHEL-16182)

- dlfcn-util: add static asserts ensuring our sym_xyz() func ptrs match the types from the official headers (RHEL-16182)

- tpm2: add tpm2_marshal_blob() and tpm2_unmarshal_blob() (RHEL-16182)

- tpm2: add tpm2_serialize() and tpm2_deserialize() (RHEL-16182)

- tpm2: add tpm2_index_to_handle() and tpm2_index_from_handle() (RHEL-16182)

- tpm2: fix build failure without openssl (RHEL-16182)

- tpm2-util: look for tpm2-pcr-signature.json directly in /.extra/ (RHEL-16182)

- tpm2: downgrade most log functions from error to debug (RHEL-16182)

- tpm2: handle older tpm enrollments without a saved pcr bank (RHEL-16182)

- tpm2: allow tpm2_make_encryption_session() without bind key (RHEL-16182)

- tpm2: update tpm2 test for supported commands (RHEL-16182)

- tpm2: use GREEDY_REALLOC_APPEND() in tpm2_get_capability_handles(), cap max value (RHEL-16182)

- tpm2: change tpm2_unseal() to accept Tpm2Context instead of device string (RHEL-16182)

- tpm2: cache TPM's supported ECC curves (RHEL-16182)

- tpm2-util: make tpm2_marshal_blob()/tpm2_unmarshal_blob() static (RHEL-16182)

- tpm2-util: make tpm2_read_public() static, as we use it only internally in tpm2-util.c (RHEL-16182)

- cryptenroll: allow specifying handle index of key to use for sealing (RHEL-16182)

- test: add tests for systemd-cryptenroll --tpm2-seal-key-handle (RHEL-16182)

- tpm2: do not call Esys_TR_Close() (RHEL-16182)

- tpm2: don't use GetCapability() to check transient handles (RHEL-16182)

- tpm2-util: pick up a few new symbols from tpm2-tss (RHEL-16182)

- tpm2: add tpm2_get_pin_auth() (RHEL-16182)

- tpm2: instead of adjusting authValue trailing 0(s), trim them as required by tpm spec (RHEL-16182)

- tpm2-util: rename tpm2_calculate_name() → tpm2_calculate_pubkey_name() (RHEL-16182)

- cryptenroll: do not implicitly verify with default tpm policy signature (RHEL-16182)

- cryptenroll: drop deadcode (RHEL-16182)

- tpm2: allow using tpm2_get_srk_template() without tpm (RHEL-16182)

- tpm2: add test to verify srk templates (RHEL-16182)

- tpm2: add tpm2_sym_alg_*_string() and tpm2_sym_mode_*_string() (RHEL-16182)

- tpm2: add tpm2_calculate_seal() and helper functions (RHEL-16182)

- tpm2: update test-tpm2 for tpm2_calculate_seal() (RHEL-16182)

- cryptenroll: add support for calculated TPM2 enrollment (RHEL-16182)

- test: update TEST-70 with systemd-cryptenroll calculated TPM2 enrollment (RHEL-16182)

- openssl-util: avoid freeing invalid pointer (RHEL-16182)

- creds-util: check for CAP_DAC_READ_SEARCH (RHEL-16182)

- creds-util: do not try TPM2 if there is not support (RHEL-16182)

- creds-util: merge the TPM2 detection for initrd (RHEL-16182)

- cryptenroll: fix a memory leak (RHEL-16182)

- sd-journal: introduce sd_journal_step_one() (RHEL-11591)

- test: modernize test-journal-flush (RHEL-11591)

- journal-file-util: do not fail when journal_file_set_offline() called more than once (RHEL-11591)

- journal-file-util: Prefer punching holes instead of truncating (RHEL-11591)

- test: add reproducer for SIGBUS issue caused by journal truncation (RHEL-11591)

  

* Wed Jan 31 2024 systemd maintenance team <systemd-maint@redhat.com> - 252-26

- spec: update rhel-net-naming-sysattrs to v0.4 (RHEL-22278)

  

* Tue Jan 30 2024 systemd maintenance team <systemd-maint@redhat.com> - 252-25

- spec: add new package with RHEL-specific network naming sysattrs (RHEL-22278)

  

* Wed Jan 24 2024 systemd maintenance team <systemd-maint@redhat.com> - 252-24

- ci: use source-git-automation composite Action (RHEL-1086)

- ci: increase the cron interval to 45 minutes (RHEL-1086)

- ci: add all Z-Stream versions to array of allowed versions (RHEL-1086)

- udev/net_id: introduce naming scheme for RHEL-9.4 (RHEL-22427)

- basic/errno-util: add wrappers which only accept negative errno (RHEL-22443)

- errno-util: allow ERRNO_IS_* to accept types wider than int (RHEL-22443)

- udev: add new builtin net_driver (RHEL-22443)

- udev/net_id: introduce naming scheme for RHEL-8.10 (RHEL-22427)

  

* Fri Jan 12 2024 systemd maintenance team <systemd-maint@redhat.com> - 252-23

- logind: don't setup idle session watch for lock-screen and greeter (RHEL-20757)

- logind: don't make idle action timer accuracy more coarse than timeout (RHEL-20757)

- logind: do TTY idle logic only for sessions marked as "tty" (RHEL-20757)

- meson: Properly install 90-uki-copy.install (RHEL-16354)

  

* Mon Jan 08 2024 systemd maintenance team <systemd-maint@redhat.com> - 252-22

- Revert "man: mention System Administrator's Guide in systemctl manpage" (RHEL-19436)

- man: mention RHEL documentation in systemctl's man page (RHEL-19436)

- resolved: actually check authenticated flag of SOA transaction (RHEL-6216)

- udev: allow/denylist for reading sysfs attributes when composing a NIC name (RHEL-1317)

- man: environment value -> udev property (RHEL-1317)

  

* Mon Dec 11 2023 systemd maintenance team <systemd-maint@redhat.com> - 252-21

- meson: fix installation of ukify (RHEL-13199)

- sd-id128: introduce id128_hash_ops_free (RHEL-5988)

- udevadm-trigger: allow to fallback without synthetic UUID only first time (RHEL-5988)

- udevadm-trigger: settle with synthetic UUID if the kernel support it (RHEL-5988)

- udevadm-trigger: also check with the original syspath if device is renamed (RHEL-5988)

- test: use 'udevadm trigger --settle' even if device is renamed (RHEL-5988)

- sd-event: don't mistake USEC_INFINITY passed in for overflow (RHEL-6090)

- pid1: rework service_arm_timer() to optionally take a relative time value (RHEL-6090)

- manager: add one more assert() (RHEL-6090)

- pid1: add new Type=notify-reload service type (RHEL-6090)

- man: document Type=notify-reload (RHEL-6090)

- pid1: make sure we send our calling service manager RELOADING=1 when reloading (RHEL-6090)

- networkd: implement Type=notify-reload protocol (RHEL-6090)

- udevd: implement the full Type=notify-reload protocol (RHEL-6090)

- logind: implement Type=notify-reload protocol properly (RHEL-6090)

- notify: add --stopping + --reloading switches (RHEL-6090)

- test: add Type=notify-reload testcase (RHEL-6090)

- update TODO (RHEL-6090)

- core: check for SERVICE_RELOAD_NOTIFY in manager_dbus_is_running (RHEL-6090)

  

* Fri Dec 08 2023 systemd maintenance team <systemd-maint@redhat.com> - 252-20

- udev/net: allow new link name as an altname before renaming happens (RHEL-5988)

- sd-netlink: do not swap old name and alternative name (RHEL-5988)

- sd-netlink: restore altname on error in rtnl_set_link_name (RHEL-5988)

- udev: attempt device rename even if interface is up (RHEL-5988)

- sd-netlink: add a test for rtnl_set_link_name() (RHEL-5988)

- test-network: add a test for renaming device to current altname (RHEL-5988)

- udev: align table (RHEL-5988)

- sd-device: make device_set_syspath() clear sysname and sysnum (RHEL-5988)

- sd-device: do not directly access entry in sd-device object (RHEL-5988)

- udev: move device_rename() from device-private.c (RHEL-5988)

- udev: restore syspath and properties on failure (RHEL-5988)

- sd-device: introduce device_get_property_int() (RHEL-5988)

- core/device: downgrade log level for ignored errors (RHEL-5988)

- core/device: ignore failed uevents (RHEL-5988)

- test: add tests for failure in renaming network interface (RHEL-5988)

- test: modernize test-netlink.c (RHEL-5988)

- test-netlink: use dummy interface to test assigning new interface name (RHEL-5988)

- udev: use SYNTHETIC_ERRNO() at one more place (RHEL-5988)

- udev: make udev_builtin_run() take UdevEvent* (RHEL-5988)

- udev/net: verify ID_NET_XYZ before trying to assign it as an alternative name (RHEL-5988)

- udev/net: generate new network interface name only on add uevent (RHEL-5988)

- sd-netlink: make rtnl_set_link_name() optionally append alternative names (RHEL-5988)

- udev/net: assign alternative names only on add uevent (RHEL-5988)

- test: add tests for renaming network interface (RHEL-5988)

- Backport ukify from upstream (RHEL-13199)

- bootctl: make --json output normal json (RHEL-13199)

- test: replace readfp() with read_file() (RHEL-13199)

- stub/measure: document and measure .uname UKI section (RHEL-13199)

- boot: measure .sbat section (RHEL-13199)

- Revert "test_ukify: no stinky root needed for signing" (RHEL-13199)

- ukify: move to /usr/bin and mark as non non-experimental (RHEL-13199)

- kernel-install: Add uki layout (RHEL-16354)

- kernel-install: remove math slang from man page (RHEL-16354)

- kernel-install: handle uki installs automatically (RHEL-16354)

- 90-uki-copy.install: create $BOOT/EFI/Linux directory if needed (RHEL-16354)

- kernel-install: Log location that uki is installed in (RHEL-16354)

- bootctl: fix errno logging (RHEL-16354)

- bootctl: add kernel-identity command (RHEL-16354)

- bootctl: add kernel-inspect command (RHEL-16354)

- bootctl: add kernel-inspect to --help text (RHEL-16354)

- bootctl: drop full stop at end of --help texts (RHEL-16354)

- bootctl: change section title for kernel image commands (RHEL-16354)

- bootctl: remove space that should not be there (RHEL-16354)

- bootctl: kernel-inspect: print os info (RHEL-16354)

- bootctl-uki: several coding style fixlets (RHEL-16354)

- tree-wide: unify how we pick OS pretty name to display (RHEL-16354)

- bootctl-uki: several follow-ups for inspect_osrel() (RHEL-16354)

- bootctl: Add missing %m (RHEL-16354)

- bootctl: tweak DOS header magic check (RHEL-16354)

  

* Mon Nov 13 2023 systemd maintenance team <systemd-maint@redhat.com> - 252-19

- ci: Extend source-git-automation (RHEL-1086)

- netif-naming-scheme: let's also include rhel8 schemes (RHEL-7026)

- systemd-analyze: Add table and JSON output implementation to plot (RHEL-5070)

- systemd-analyze: Update man/systemd-analyze.xml with Plot JSON and table (RHEL-5070)

- systemd-analyze: Add tab complete logic for plot (RHEL-5070)

- systemd-analyze: Add --json=, --table and -no-legend tests for plot (RHEL-5070)

- ci: enable source-git automation to validate reviews and ci results (RHEL-1086)

- ci: remove Mergify config - replaced by Pull Request Validator (RHEL-1086)

- ci: enable auto-merge GH Action (RHEL-1086)

- ci: add missing permissions (RHEL-1086)

- ci: `permissions: write-all` (RHEL-1086)

- ci(lint): exclude `.in` files from ShellCheck lint (RHEL-1086)

- udev: raise RLIMIT_NOFILE as high as we can (RHEL-11040)

  

* Tue Aug 22 2023 systemd maintenance team <systemd-maint@redhat.com> - 252-18

- doc: add downstream CONTRIBUTING document (#2170883)

- doc: improve CONTRIBUTING document (#2170883)

- doc: use link with prefilled Jira issue (#2170883)

- docs: link downstream CONTRIBUTING in README (#2170883)

- bpf: fix restrict_fs on s390x (#2230364)

- udev/net_id: use naming scheme for RHEL-9.3 (#2231845)

- core/timer: Always use inactive_exit_timestamp if it is set (#2211065)

- timer: Use dual_timestamp_is_set() in one more place (#2211065)

- loginctl: list-users: also show state (#2209912)

- loginctl: list-sessions: minor modernization (#2209912)

- loginctl: list-sessions: also show state (#2209912)

- test: add test for state in loginctl list-{users,sessions} (#2209912)

- test: add a missing session activation (#2209912)

- test: extend test for loginctl list-* (#2209912)

- loginctl: shorten variable name (#2209912)

- loginctl: use bus_map_all_properties (#2209912)

- loginctl: show session idle status in list-sessions (#2209912)

- loginctl: some modernizations (#2209912)

- loginctl: list-sessions: fix timestamp for idle hint (#2209912)

- loginctl: list-users: use bus_map_all_properties (#2209912)

- loginctl: also show idle hint in session-status (#2209912)

- memory-util: make ArrayCleanup passed to array_cleanup() const (#2190226)

- static-destruct: several cleanups (#2190226)

- static-destruct: introduce STATIC_ARRAY_DESTRUCTOR_REGISTER() (#2190226)

- macro: support the case that the number of elements has const qualifier (#2190226)

- shared/generator: apply similar config reordering of generated units (#2190226)

- nulstr-util: make ret_size in strv_make_nulstr() optional (#2190226)

- generator: teach generator_add_symlink() to instantiate specified unit (#2190226)

- units: rework growfs units to be just a regular unit that is instantiated (#2190226)

- fstab-generator: use correct targets when /sysroot is specificied in fstab only (#2190226)

- fstab-generator: add SYSTEMD_SYSFS_CHECK env var (#2190226)

- test: add fstab file support for fstab-generator tests (#2190226)

- test-fstab-generator: also check file contents (#2190226)

- test-fstab-generator: add tests for mount options (#2190226)

- fstab-generator: split out several functions from parse_fstab() (#2190226)

- fstab-generator: call add_swap() earlier (#2190226)

- fstab-generator: refuse to add swap earlier if disabled (#2190226)

- fstab-generator: refuse invalid mount point path in fstab earlier (#2190226)

- fstab-generator: fix error code propagation in run_generator() (#2190226)

- fstab-generator: support defining mount units through kernel command line (#2190226)

- test: add test cases for defining mount and swap units from kernel cmdline (#2190226)

- generators: change TimeoutSec=0 to TimeoutSec=infinity (#2190226)

- units: change TimeoutSec=0 to TimeoutSec=infinity (#2190226)

- fstab-generator: use correct swap name var (#2190226)

- fstab-generator: add more parameter name comments (#2190226)

- fstab-generator: unify initrd-root-device.target dependency handling code (#2190226)

- fstab-util: add fstab_is_bind (#2190226)

- fstab-generator: resolve bind mount source when in initrd (#2190226)

- fstab-generator: rename 'initrd' flag to 'prefix_sysroot' (#2190226)

- fstab-generator: fix target of /sysroot/usr (#2190226)

- fstab-generator: add rd.systemd.mount-extra= and friends (#2190226)

- fstab-generator: add a flag to accept entry for "/" in initrd (#2190226)

- test-fstab-generator: extract core part as a function (#2190226)

- test-fstab-generator: also test with SYSTEMD_IN_INITRD=no (#2190226)

- test-fstab-generator: add more tests for systemd.mount-extra= and friends (#2190226)

- fstab-generator: enable fsck for block device mounts specified in systemd.mount-extra= (#2190226)

- core: use correct scope of looking up units (#2226980)

- test: merge unit file related tests into TEST-23-UNIT-FILE (#2213521)

- test: rename TEST-07-ISSUE-1981 to TEST-07-PID1 (#2213521)

- test: merge TEST-08-ISSUE-2730 into TEST-07-PID1 (#2213521)

- test: merge TEST-09-ISSUE-2691 into TEST-07-PID1 (#2213521)

- test: merge TEST-10-ISSUE-2467 with TEST-07-PID1 (#2213521)

- test: merge TEST-11-ISSUE-3166 into TEST-07-PID1 (#2213521)

- test: merge TEST-12-ISSUE-3171 into TEST-07-PID1 (#2213521)

- test: move TEST-23's units into a dedicated subfolder (#2213521)

- test: merge TEST-47-ISSUE-14566 into TEST-07-PID1 (#2213521)

- test: merge TEST-51-ISSUE-16115 into TEST-07-PID1 (#2213521)

- test: merge TEST-20-MAINPIDGAMES into TEST-07-PID1 (#2213521)

- test: abstract the common test parts into a utility script (#2213521)

- test: add tests for JoinsNamespaceOf= (#2213521)

- core/unit: drop doubled empty line (#2213521)

- core/unit: make JoinsNamespaceOf= implies the inverse dependency (#2213521)

- core/unit: search shared namespace in transitive relation of JoinsNamespaceOf= (#2213521)

- core/unit: update bidirectional dependency simultaneously (#2213521)

- resolvectl: fix type of ifindex D-Bus field, and make sure to initialize to zero in all code paths (#2161260)

- resolved: add some line-breaks/comments (#2161260)

- resolvectl: don't filter loopback DNS server from global DNS server list (#2161260)

- blockdev-util: add simple wrapper around BLKSSZGET (#2170883)

- loop-util: insist on setting the sector size correctly (#2170883)

- dissect-image: add probe_sector_size() helper for detecting sector size of a GPT disk image (#2170883)

- loop-util: always tell kernel explicitly about loopback sector size (#2170883)

- Revert "Treat EPERM as "not available" too" (#2178222)

- Revert "test: accept EPERM for unavailable idmapped mounts as well" (#2178222)

  

* Fri Aug 04 2023 systemd maintenance team <systemd-maint@redhat.com> - 252-17

- Revert "core/service: when resetting PID also reset known flag" (#2225667

- ci: explicitly install python3-lldb-$COMPILER_VERSION (#2225667)

  

* Mon Jul 17 2023 systemd maintenance team <systemd-maint@redhat.com> - 252-16

- ci: update permissions for source-git automation workflows (#2170883)

- pstore: fixes for dmesg.txt reconstruction (#2170883)

- pstore: explicitly set the base when converting record ID (#2170883)

- pstore: avoid opening the dmesg.txt file if not requested (#2170883)

- test: add a couple of tests for systemd-pstore (#2170883)

- test: match all messages with the FILE field (#2170883)

- test: build the SELinux test module on the host (#2170883)

- test: make the stress test slightly less stressful on slower machines (#2170883)

- coredump: use unaligned_read_ne{32,64}() to parse auxv (#2170883)

- core/transaction: make merge_unit_ids() always return NUL-terminated string (#2170883)

- core/transaction: make merge_unit_ids() return non-NULL on success (#2170883)

- core/transaction: do not log "(null)" (#2170883)

- ci: allow `RHEL-only` labels to mark downstream-only commits (#2170883)

- elf-util: discard PT_LOAD segment early based on the start address. (#2215412)

- elf-util: check for overflow when computing end of core's PT_LOAD segments (#2215412)

- sulogin: use DEFINE_MAIN_FUNCTION() (#2169959)

- sulogin: fix control lost of the current terminal when default.target is rescue.target (#2169959)

- journal-vacuum: count size of all journal files (#2182632)

- memory-util: add a concept for gcc cleanup attribute based array destruction (#2182632)

- macro: introduce FOREACH_ARRAY() macro (#2182632)

- journal-vacuum: rename function to match struct name (#2182632)

- journal-vacuum: use CLEANUP_ARRAY (#2182632)

- pam: add call to pam_umask (#2210145)

- udev-builtin-net_id: align VF representor names with VF names (#2218886)

- pam: add a call to pam_namespace (#2218184)

- rules: online CPU automatically on IBM s390x platforms when configured (#2212612)

- core/mount: escape invalid UTF8 char in dbus reply (#2208240)

- Revert "user: delegate cpu controller, assign weights to user slices" (#2176899)

- udev-rules: fix nvme symlink creation on namespace changes (#2172509)

- rules: add whitespace after comma before the line continuation (#2172509)

- udev: restore compat symlink for nvme devices (#2172509)

- rules: drop doubled space (#2172509)

- manager: don't taint the host if cgroups v1 is used (#2193456)

- core/service: when resetting PID also reset known flag (#2210237)

- ci: drop systemd-stable from advanced-commit-linter config (#2170883)

  

* Thu May 18 2023 systemd maintenance team <systemd-maint@redhat.com> - 252-15

- ci: trigger `differential-shellcheck` workflow on push (#2100440)

- ci: workflow for gathering metadata for source-git automation (#2100440)

- ci: first part of the source-git automation - commit linter (#2100440)

- ci(Mergify): check CodeQL and build workflows based on changed files (#2100440)

- ci: add NOTICE to also update regexp in `.mergify.yml` when updating `paths` property (#2100440)

- Support /etc/system-update for OSTree systems (#2203133)

- journal-def: fix type of signature to match the actual field in the Header structure (#2183546)

- journal: use compound initialization for journal file Header structure (#2183546)

- journald: fix log message (#2183546)

- sd-journal: cache results of parsing environment variables (#2183546)

- compress: introduce compression_supported() helper function (#2183546)

- sd-journal: always use the compression algorithm specified in the header (#2183546)

- sd-journal: allow to specify compression algorithm through env (#2183546)

- test: add test case that journal file is created with the requested compression algorithm (#2183546)

- rules: do not online CPU automatically on IBM platforms (#2143107)

  

* Tue Mar 21 2023 systemd maintenance team <systemd-maint@redhat.com> - 252-14

- systemd: Support OOMPolicy in scope units (#2176918)

- systemd: Default to OOMPolicy=continue for login session scopes (#2176918)

- man: rework description of OOMPolicy= a bit (#2176918)

- core,man: add missing integration of OOMPolicy= in scopes (#2176918)

- meson: Store fuzz tests in structured way (#2176918)

- meson: Generate fuzzer inputs with directives (#2176918)

- oss-fuzz: include generated corpora in the final zip file (#2176918)

- unit: In cgroupv1, gracefully terminate delegated scopes again (#2180120)

  

* Mon Feb 27 2023 systemd maintenance team <systemd-maint@redhat.com> - 252-8

- journal-file: Fix return value in bump_entry_array() (#2173682)

  

* Mon Feb 27 2023 systemd maintenance team <systemd-maint@redhat.com> - 252-7

- test: add coverage for #24177 (#1985288)

- logind-session: make stopping of idle session visible to admins (#2172401)

  

* Wed Feb 22 2023 systemd maintenance team <systemd-maint@redhat.com> - 252-6

- journalctl: actually run the static destructors (#2122500)

- efi: drop executable-stack bit from .elf file (#2140646)

- install: fail early if specifier expansion failed (#2138081)

- test: add coverage for #26467 (#2138081)

  

* Fri Feb 17 2023 systemd maintenance team <systemd-maint@redhat.com> - 252-5

- nss-myhostname: fix inverted condition in (#2167468)

- nss-myhostname: do not return empty result with NSS_STATUS_SUCCESS (#2167468)

- sleep: rename hibernate_delay_sec -> _usec (#2151612)

- sleep: fetch_batteries_capacity_by_name() does not return -ENOENT (#2151612)

- sleep: drop unnecessary temporal vaiable and initialization (#2151612)

- sleep: introduce SuspendEstimationSec= (#2151612)

- sleep: coding style fixlets (#2151612)

- sleep: simplify code a bit (#2151612)

- sleep: fix indentation (#2151612)

- sleep: enumerate only existing and non-device batteries (#2151612)

- core: when isolating to a unit, also keep units running that are triggered by units we keep running (#1952378)

- udev/net_id: introduce naming scheme for RHEL-9.2 (#2170500)

  

* Mon Feb 06 2023 systemd maintenance team <systemd-maint@redhat.com> - 252-4

- udev: make get_virtfn_info() provide physical PCI device (#2159448)

- test: make helper_check_device_units() log unit name (#2138081)

- test: add a testcase for lvextend (#2138081)

- pid1: fix segv triggered by status query (#26279) (#2138081)

- test: create config under /run (#2138081)

- test: add tests for mDNS and LLMNR settings (#2138081)

- resolved: introduce the _localdnsstub and _localdnsproxy special hostnames for 127.0.0.54 + 127.0.0.53 (#2138081)

- test: wait for the monitoring service to become active (#2138081)

- test: suppress echo in monitor_check_rr() (#2138081)

- Revert "test: wait for the monitoring service to become active" (#2138081)

- test: show and check almost all journal entries since the relevant command being invoked (#2138081)

- test: cover IPv6 in the resolved test suite (#2138081)

- test: add a couple of SRV records to check service resolution (#2138081)

- test: add a test for the OPENPGPKEY RR (#2138081)

- test: don't hang indefinitely on no match (#2138081)

- test-ndisc: fix memleak and fd leak (#2138081)

- test-unit-name: fix fd leak (#2138081)

- test: bump D-Bus service start timeout if we run without accel (#2138081)

- test: bump the client-side timeout in sd-bus as well (#2138081)

- test: bump the container spawn timeout to 60s (#2138081)

- network: fix memleak (#2138081)

- busctl: fix introspecting DBus properties (#2138081)

- busctl: simplify peeking the type (#2138081)

- resolve: drop redundant call of socket_ipv6_is_supported() (#2138081)

- resolve: introduce link_get_llmnr_support() and link_get_mdns_support() (#2138081)

- resolve: provide effective supporting levels of mDNS and LLMNR (#2138081)

- resolvectl: warn if the global mDNS or LLMNR support level is lower than the requested one (#2138081)

- resolve: enable per-link mDNS setting by default (#2138081)

  

* Mon Jan 16 2023 systemd maintenance team <systemd-maint@redhat.com> - 252-3

- swap: tell swapon to reinitialize swap if needed (#2151993)

- coredump: adjust whitespace (#2155517)

- coredump: do not allow user to access coredumps with changed uid/gid/capabilities (#2155517)

- Revert "basic: add fallback in chase_symlinks_and_opendir() for cases when /proc is not mounted" (#2138081)

- glyph-util: add warning sign special glyph (#2138081)

- chase-symlink: when converting directory O_PATH fd to real fd, don't bother with /proc/ (#2138081)

- systemctl: print a clear warning if people invoke systemctl without /proc/ (#2138081)

- TEST-65: check cat-config operation in chroot (#2138081)

- TEST-65: use [[ -v ]] more (#2138081)

- systemctl: warn if trying to disable a unit with no install info (#2141979)

- systemctl: allow suppress the warning of no install info using --no-warn (#2141979)

- rpm/systemd-update-helper: use --no-warn when disabling units (#2141979)

- systemctl: suppress warning about missing /proc/ when --no-warn (#2141979)

- shell-completion: systemctl: add --no-warn (#2141979)

- core/unit: drop doubled empty line (#2160477)

- core/unit: drop dependency to the unit being merged (#2160477)

- core/unit: fix logic of dropping self-referencing dependencies (#2160477)

- core/unit: merge two loops into one (#2160477)

- test: add test case for sysv-generator and invalid dependency (#2160477)

- core/unit: merge unit names after merging deps (#2160477)

- core/unit: fix log message (#2160477)

- test: explicitly create the /etc/init.d directory (#2160477)

- test: support a non-default SysV directory (#2160477)

  

* Fri Dec 09 2022 systemd maintenance team <systemd-maint@redhat.com> - 252-2

- test: check if we can use SHA1 MD for signing before using it (#2141979)

- boot: cleanups for efivar_get() and friends (#2141979)

- boot: fix false maybe-uninitialized warning (#2141979)

- tree-wide: modernizations with RET_NERRNO() (#2137584)

- sd-bus: handle -EINTR return from bus_poll() (#2137584)

- stdio-bridge: don't be bothered with EINTR (#2137584)

- varlink: also handle EINTR gracefully when waiting for EIO via ppoll() (#2137584)

- sd-netlink: handle EINTR from poll() gracefully, as success (#2137584)

- resolved: handle -EINTR returned from fd_wait_for_event() better (#2137584)

- homed: handle EINTR gracefully when waiting for device node (#2137584)

- utmp-wtmp: fix error in case isatty() fails (#2137584)

- utmp-wtmp: handle EINTR gracefully when waiting to write to tty (#2137584)

- io-util: document EINTR situation a bit (#2137584)

- terminal-util: Set OPOST when setting ONLCR (#2138081)

- cgtop: Do not rewrite -P or -k options (#2138081)

- test: Add tests for systemd-cgtop args parsing (#2138081)

- resolved: remove inappropriate assert() (#2138081)

- boot: Add xstrn8_to_16 (#2138081)

- boot: Use xstr8_to_16 (#2138081)

- boot: Use xstr8_to_16 for path conversion (#2138081)

-    stub: Fix cmdline handling (#2138081)

- stub: Detect empty LoadOptions when run from EFI shell (#2138081)

- boot: Use EFI_BOOT_MANAGER_POLICY_PROTOCOL to connect console devices (#2138081)

- boot: Make sure all partitions drivers are connected (#2138081)

- boot: improve support for qemu (#2138081)

- systemd-boot man page: add section for virtual machines (#2138081)

- boot: Only do full driver initialization in VMs (#2138081)

- dissect: rework DISSECT_IMAGE_ADD_PARTITION_DEVICES + DISSECT_IMAGE_OPEN_PARTITION_DEVICES (#2138081)

- ci(Mergify): v252 configuration update (#2138081)

- ci: Run GitHub workflows on rhel branches (#2138081)

- ci: Drop scorecards workflow, not relevant (#2138081)

  

* Fri Dec 02 2022 systemd maintenance team <systemd-maint@redhat.com> - 252-1

- Rebase to systemd v252 + systemd-stable v252.2 (#2138081)

  

* Fri Dec 02 2022 systemd maintenance team <systemd-maint@redhat.com> - 250-13

- build systemd-boot EFI tools (#2140646)

  

[root@rocky14 ~]# rpm -q -changelog systemd | more

* Sat Nov 16 2024 Release Engineering <releng@rockylinux.org> - 252-46.0.1

- Set support URL to the wiki

- Set sbat mail to security@rockylinux.org

  

* Tue Sep 10 2024 systemd maintenance team <systemd-maint@redhat.com> - 252-46.2

- add %posttrans scriptlet to make sure our SELinux policy module is actually installed (RHEL-46339)

  

* Tue Sep 03 2024 systemd maintenance team <systemd-maint@redhat.com> - 252-46.1

- version bump (RHEL-56019)

  

* Fri Aug 30 2024 systemd maintenance team <systemd-maint@redhat.com> - 252-46

- ukify: Skip test on architectures without UEFI (RHEL-56019)

  

* Sat Aug 24 2024 systemd team <systemd-maint@redhat.com> - 252-45

- build ukify without noarch

  

* Thu Aug 22 2024 systemd maintenance team <systemd-maint@redhat.com> - 252-44

- Revert "udev-builtin-net_id: use firmware_node/sun for ID_NET_NAME_SLOT" (RHEL-50103)

- fundamental: share constants for confidential virt detection (RHEL-50651)

- efi: add helper API for detecting confidential virtualization (RHEL-50651)

- efi: don't pull kernel cmdline from SMBIOS in a confidential VM (RHEL-50651)

- Fix detection of TDX confidential VM on Azure platform (RHEL-50651)

  

* Thu Aug 22 2024 systemd maintenance team <systemd-maint@redhat.com> - 252-43

- udev-builtin-net_id: skip non-directory entry earlier (RHEL-50103)

- udev-builtin-net_id: return earlier when hotplug slot is not found (RHEL-50103)

- udev-builtin-net_id: split-out pci_get_hotplug_slot() and pci_get_hotplug_slot_from_address() (RHEL-50103)

- udev-builtin-net_id: use firmware_node/sun for ID_NET_NAME_SLOT (RHEL-50103)

- Include <threads.h> if possible to get thread_local definition (RHEL-50651)

- add APIs for detecting confidential virtualization (RHEL-50651)

- detect-virt: add --cvm option (RHEL-50651)

- detect-virt: add --list-cvm option (RHEL-50651)

- unit: add "cvm" option for ConditionSecurity (RHEL-50651)

- dbus: add 'ConfidentialVirtualization' property to manager object (RHEL-50651)

- core: log detected confidential virtualization type (RHEL-50651)

- core: set SYSTEMD_CONFIDENTIAL_VIRTUALIZATION env for generators (RHEL-50651)

- udev: add 'conf-virt' constant for confidential virtualization tech (RHEL-50651)

- confidential-virt: split caching of CVM detection into separate method (RHEL-50651)

- confidential-virt: add detection for s390x target (RHEL-50651)

- man/systemd-detect-virt: list known CVM technologies (RHEL-50651)

  

* Mon Aug 19 2024 systemd team <systemd-maint@redhat.com>

- fix applying patches

  

* Thu Aug 15 2024 systemd maintenance team <systemd-maint@redhat.com> - 252-41

- timedatectl: setting set_local_rtc to 1 will throw Warning as well, use log_warning() (#33489) (RHEL-45020)

- cryptsetup-tokens: fix pin asserts (RHEL-36276)

- cryptenroll: Use CTAP2.1 credProtect extension (RHEL-36276)

- kernel-install: check machine ID (RHEL-50672)

- kernel-install: ignore errors when reading /etc/machine-id (RHEL-50672)

- hwdb: Add Lenovo G580 (RHEL-5950)

- Fix key toggle and programmable button for Positivo N14ZP (RHEL-5950)

- hwdb: Add accel orientation quirk for the Acer Switch V 10 SW5-017 2-in-1 (RHEL-5950)

- hwdb: fix Compaq N14KP6 key toggle touchpad (#25404) (RHEL-5950)

- hwdb: remove fuzz and deadzone for Simucube wheel bases. (RHEL-5950)

- hwdb: Add support for Elgato Stream Pedal (#25550) (RHEL-5950)

- hwdb: add Clevo touchpad toggle key quirks (RHEL-5950)

- hwdb: add Dell Inspiron N4010 touchpad corrections (RHEL-5950)

- hwdb: add Positivo-vaio Pro PW key toggle touchpad (#25669) (RHEL-5950)

- Add mount matrix for VisionBook 12Wr Tab (RHEL-5950)

- Update 60-evdev.hwdb (#25704) (RHEL-5950)

- hwdb: Add additional Dell models that require ACCEL_LOCATION=base (#25724) (RHEL-5950)

- hwdb: drop trailing space (RHEL-5950)

- hwdb: add comments about matching entries (RHEL-5950)

- hwdb: also add a generic entry for DualPoint Stick (RHEL-5950)

- hwdb: Add mount matrix for CSL Panther Tab HD (RHEL-5950)

- hwdb: Fix mount matrix for CSL Panther Tab HD (#25752) (RHEL-5950)

- hwdb: Fn+F5 fix for MSI Bravo 15-B5DX (#25788) (RHEL-5950)

- hwdb: change definition of PROXIMITY_NEAR_LEVEL for sensors (RHEL-5950)

- hwdb: Add mic-mute, control-center and screen-rotation mappings for MSI laptops (RHEL-5950)

- Prevents airplane mode toggle for HP Spectre 16 (RHEL-5950)

- Update 60-sensor.hwdb (RHEL-5950)

- Added Tablet Teclast X98 Air 3G (C5J6) (RHEL-5950)

- hwdb: remove spurious whitespace (RHEL-5950)

- hwdb: Add Dell models that require ACCEL_LOCATION=base (RHEL-5950)

- Fix Positivo MASTER-N1110 key toggle touchpad (RHEL-5950)

- hwdb: Mark Dell platform accel sensor location to base (RHEL-5950)

- hwdb: Add mount matrix for Linx 1020 (RHEL-5950)

- hwdb: Add mic mute key mappings for Dell G16 Series (RHEL-5950)

- hwdb: Add Chuwi Hi10X (N4120 version) iio matrix (RHEL-5950)

- hwdb: Add touchpad toggle mapping for System76 Pangolin 12 (RHEL-5950)

- hwdb: Prevent activation of airplane mode on HP ENVY x360 (RHEL-5950)

- Update hwdb (RHEL-5950)

- hwdb: update (RHEL-5950)

- hwdb: update autosuspend db (RHEL-5950)

- hwdb: ieee1394-unit-function: add MOTU 896 mk3 Hybrid (RHEL-5950)

- Add hwdb sensor entry for Lenovo IdeaPad Duet 3 10IGL5 (82AT). (RHEL-5950)

- Fix Positivo-vaio VJPW12F11X key toggle touchpad (RHEL-5950)

- hwdb: Add HP Envy x360 Convertible 15-cn0xxx to existing entry (RHEL-5950)

- hwdb: add override for IdeaPad5 insert key (RHEL-5950)

- hwdb: update database (RHEL-5950)

- hwdb: Add HP ENVY x360 2-in-1 (RHEL-5950)

- hwdb: update (RHEL-5950)

- hwdb: fix swapped buttons for Logitech Lift left (RHEL-5950)

- Revert "hwdb: fix swapped buttons for Logitech Lift left" (RHEL-5950)

- hwdb: update 70-mouse.hwdb (#26782) (RHEL-5950)

- hwdb: 60-keyboard.hwdb: Fix modalias for Thinkpad X200 Tablet (#26795) (RHEL-5950)

- Add rebrands of Medion Akoya notebooks/tablets (RHEL-5950)

- hwdb: fix Wifi toggling for Haier 7G-Series/JWU (#25293) (#26878) (RHEL-5950)

- hwdb: drop boilerplate about match patterns in two more cases (RHEL-5950)

- hwdb: Fix incorrect touchpad dimensions on Thinkpad L14 Gen1 (#26937) (RHEL-5950)

- hwdb: drop redundant entry (RHEL-5950)

- hwdb: Fixed thumb buttons reversed on CHERRY MW 2310 (#26992) (RHEL-5950)

- hwdb: Move MSI touchpad-toggle mapping to generic MSI section (RHEL-5950)

- update 60-sensor.hwdb with toshiba tablet (#27103) (RHEL-5950)

- hwdb: Add support for "Passion Model P612F" (RHEL-5950)

- hwdb: fix ambiguous glob pattern for Lenovo machines (RHEL-5950)

- hwdb: add matrix for Asus BR1100F (#27197) (RHEL-5950)

- hwdb: add accelerometer mount matrix for Lenovo Yoga Tablet 2 851F/L (RHEL-5950)

- hwdb: Fix rotation for BMAX Y13 (RHEL-5950)

- hwdb: disable entry for Logitech USB receiver used by G502 X (RHEL-5950)

- hwdb: add hardware rfkill key for Dell Latitude E6* models (#27462) (RHEL-5950)

- hwdb: do not include '#' in modalias (RHEL-5950)

- hwdb: add landscape IdeaPad Miix 310 sensor orientation (#27555) (RHEL-5950)

- Fix Positivo CF40CM-V2 key toggle touchpad (RHEL-5950)

- hwdb: fix keyboard entry for IdeapadFlex5 (#27643) (RHEL-5950)

- hwdb: fix Positivo CG15D key toggle touchpad and programmable keys (#27689) (RHEL-5950)

- hwdb: add support for Elgato Stream Deck mini (gen 2) (RHEL-5950)

- hwdb: fix arrow keys on HP Elite Dragonfly G3 (RHEL-5950)

- hwdb: add support for Jun Tab2/Dere T11 to 60-sensor.hwdb (#28092) (RHEL-5950)

- hwdb: fix volume control keys on Lenovo IdeaPad Flex 5 (14ARE05) (RHEL-5950)

- hwdb: Add override for headset form-factors (RHEL-5950)

- hwdb : add support for Archos 101 Cesium Educ to 60-sensor.hwdb (RHEL-5950)

- hwdb: drop trailing white space (RHEL-5950)

- hwdb: merge multiple keyboard entries with same setting (RHEL-5950)

- hwdb: make matching modalias for Archos 101 Cesium Educ more strict (RHEL-5950)

- hwdb update for v246-rc1 (RHEL-5950)

- update hwdb autosuspend data for v254 (RHEL-5950)

- hwdb: add support for Archos 101 Cesium to 60-sensor.hwdb (#28270) (RHEL-5950)

- Hwdb: Add Sanwa Direct 400-MA128 external trackpad (#28272) (RHEL-5950)

- hwdb: drop POINTINGSTICK_CONST_ACCEL (RHEL-5950)

- Add alternate name for MX Ergo as found on some devices (RHEL-5950)

- Update hwdb (RHEL-5950)

- hwdb: run update-hwdb (RHEL-5950)

- hwdb: run update-hwdb (RHEL-5950)

- hwdb: Mute SW rfkill keys on MSI Wind U100 (RHEL-5950)

- Update 60-sensor.hwdb (#28804) (RHEL-5950)

- hwdb: Added config for RCA W101SA23T1 (#29041) (RHEL-5950)

- Update 60-input-id.hwdb: add TEX Shinobi (#29068) (RHEL-5950)

- hwdb: keyboard: D330 FnLk toggle (RHEL-5950)

- hwdb: Add Logitech G502 X (RHEL-5950)

- hwdb: ieee1394-unit-function: remove superfluous Weiss Engineering DAC1 entry (RHEL-5950)

- hwdb: ieee1394-unit-function: add Weiss Engineering DAC202 (Maya edition) (RHEL-5950)

- hwdb: ieee1394-unit-function: add Weiss Engineering INT203 entry with older firmware (RHEL-5950)

- hwdb: ieee1394-unit-function: add Weiss Engieering MAN301 (RHEL-5950)

- hwdb: Add quirk for teclast x3 plus (G4K3) rotation (#29202) (RHEL-5950)

- hwdb: add mic mute key mappings for Acer Predator Triton 300 SE (RHEL-5950)

- hwdb: Bush tablet rotation support (#29268) (RHEL-5950)

- hwdb: ieee1394-unit-function: add Miglia Technology Harmony Audio (HA02) (RHEL-5950)

- add support for hp pavilion gaming 15 lid switch (#29304) (RHEL-5950)

- Fix Positivo N14EP6 key toggle touchpad and programmable keys (#29448) (RHEL-5950)

- add udev rule for micmute (f20) (RHEL-5950)

- hwdb,rules: mark host-to-host network devices as only requiring link local addressing (RHEL-5950)

- Update hwdb (RHEL-5950)

- Update hwdb autosuspend rules (RHEL-5950)

- Update hwdb (RHEL-5950)

- hwdb: Add accelerometer data for Librem11 (#29974) (RHEL-5950)

- hwdb: PNP/ACPI lists on uefi.org are now in CSV format (RHEL-5950)

- Update hwdb (RHEL-5950)

- hwdb: rename .html=>.csv (RHEL-5950)

- hwdb/acpi-update.py: streamline python code (RHEL-5950)

- hwdb: Mark Dell platform accel sensor location to base (RHEL-5950)

- hwdb: add Predator PHN16-71 (RHEL-5950)

- Update 60-autosuspend.hwdb (#30131) (RHEL-5950)

- hwdb: update (RHEL-5950)

- hwdb: ieee1394-unit-function: add Sony DVMC-DA1 (RHEL-5950)

- hwdb: ieee1394-unit-function: arrangement for Sony DVMC-DA1 (RHEL-5950)

- hwdb: update (RHEL-5950)

- hwdb: update (RHEL-5950)

- Adding Trekstor Primebook C13 rotation to 60-sensor.hwdb (#30415) (RHEL-5950)

- Add three Dell platforms to sensor accel location base (RHEL-5950)

- Add Bosto BT-12HD series to hwdb (RHEL-5950)

- hwdb: Add override for headset form-factor for the Corsair Void Elite (RHEL-5950)

- hwdb: add Teclast X98 Pro sensor info (#30859) (RHEL-5950)

- hwdb: Correct display rotation on Chuwi Ubook X N4100 (#24248) (RHEL-5950)

- hwdb: ieee1394-unit-function: adjustment of entries with device attributes available in Linux v6.8 (RHEL-5950)

- 60-evdev.hwdb: Add support for Huion Inspiroy 2 L (#31241) (RHEL-5950)

- hwdb: add resolution setting for GAOMON S620 (RHEL-5950)

- hwdb: Remove version check in CH Pro Pedals rule (RHEL-5950)

- hwdb: Add support for MetawillBook01 to 60-sensor.hwdb Add accel orientation quirk for the METAPHYUNI MetawillBook01 2-in-1 laptop (RHEL-5950)

- hwdb: Add headset form-factor override for Xbox Wireless Dongle (RHEL-5950)

- hwdb: Add support for Elgato Stream Deck Plus (RHEL-5950)

- Fix: Chuwi UBook X (CWI535) screen rotation matrix (RHEL-5950)

- hwdb: Add touchpad toggle mapping for Kvadra LE14U/LE15U (RHEL-5950)

- hwdb: Add touchpad configuration for ThinkPad E495 (RHEL-5950)

- Fix Positivo N14NPE-N and N15NPE-N key toggle touchpad and search key (RHEL-5950)

- Update USB ids of hwdb (RHEL-5950)

- Added resolution for Huion Kamvas Pro 19 (RHEL-5950)

- hwdb: Add mapping for ACPI quickstart keys on Toshiba Z830 (RHEL-5950)

- hwdb: fix Asus T300FA rotation matrix (#31973) (RHEL-5950)

- Fixed resolution for pen and touchpad (RHEL-5950)

- hwdb: fix missing colon (#32108) (RHEL-5950)

- hwdb: update for v256 (RHEL-5950)

- autosuspend: update for v256 (RHEL-5950)

- Update hwdb (RHEL-5950)

- Update autosuspend hwdb (RHEL-5950)

- Update hwdb (RHEL-5950)

- hwdb: Add a common Logitech M185/M225 mouse variant (RHEL-5950)

- hwdb: Add mapping for Samsung GalaxyBook - 550X (#32616) (RHEL-5950)

- hwdb: Add mapping for Xiaomi Mipad 2 bottom bezel capacitive buttons (RHEL-5950)

- hwdb: ieee1394-unit-function: add Tascam IF-FW/DM mkII (RHEL-5950)

- hwdb: Add a Logitech MX Master 3S (connected via Bolt Receiver) (RHEL-5950)

- Fix Positivo N14EPE and N15EPE key toggle touchpad and search key (RHEL-5950)

- hwdb: update Dere N12 / Juno Tablet 3 accelerometer (#32765) (RHEL-5950)

- hwdb: updated Librem 11 accelerometer (#32772) (RHEL-5950)

- hwdb: ID_INPUT_XYZ allows an empty string (RHEL-5950)

- hwdb: ASRock LED Controller classified incorrectly as joystick due to buttons and axis (#32775) (RHEL-5950)

- Update hwdb (RHEL-5950)

- hwdb.d/60-keyboard.hwdb: enable Clevo quirk for model V5x0TU (RHEL-5950)

- hwdb: Enable JP-IK LEAP W502's touchpad toggle key (RHEL-5950)

- Update hwdb (RHEL-5950)

- Update autosuspend hwdb (RHEL-5950)

- hwdb: Lenovo IdeaPad Z500 Touchpad Toggle (#33039) (RHEL-5950)

- hwdb: add a vmbus id for HyperV Video device (RHEL-5950)

- hwdb: Add Logitech MX Master 3S Bluetooth ID (RHEL-5950)

- hwdb: Lenovo 16G6IRL volume keys and friends (#33107) (RHEL-5950)

- hwdb: added hwdb rules for micmute and power button on Acer Nitro AN 515-58 (#32867) (RHEL-5950)

- Fix key toggle touchpad and programmable buttom for Positivo N14AP7 (RHEL-5950)

- Update hwdb (RHEL-5950)

- hwdb: add keyboard mappings for the Ayaneo Kun face buttons (RHEL-5950)

- Update hwdb (RHEL-5950)

- hwdb: add support for AIPTEK Media Tablet Ultimate (#33371) (RHEL-5950)

- hwdb: add scancodes for AYANEO devices (#33378) (RHEL-5950)

- Add OrangePi NEO Scancodes (RHEL-5950)

- hwdb: Fix Logitech G915 TKL (Bluetooth) appearing as a mouse (RHEL-5950)

- hwdb: fix keyboard of RedmiBook Pro 15 2022 (#33465) (RHEL-5950)

- Added mised EVDEV_ABS_35 & EVDEV_ABS_36 for GAOMON s620 (RHEL-5950)

- hwdb: Add some HP IR cameras (RHEL-5950)

- hwdb: add more AV controllers (RHEL-5950)

- Fix key toggle touchpad button for multilaser ul154 (#33630) (RHEL-5950)

- hwdb: Added StarLabs StarLite position sensor mapping (RHEL-5950)

- 70-mouse.hwdb: Added Glorious Model O DPI (RHEL-5950)

- Update 60-sensor.hwdb (RHEL-5950)

- Add MSI Claw AT Keyboard Scancodes. (RHEL-5950)

- Add or fix mount matrix for multiple handhelds. (#33586) (RHEL-5950)

- Revert "hwdb: Added StarLabs StarLite position sensor mapping" (RHEL-5950)

- hwdb: fix accelerometer mount matrix for Aquarius Cmp NS483 (RHEL-5950)

- hwdb: add backslash and touchpad toggle mapping for Aquarius Cmp NS483 (RHEL-5950)

- hwdb: Add mic mute key mapping for Dell Pro Rugged series (RHEL-5950)

- hwdb: fix MXC6655 accelerometer mount matrix for Aquarius Cmp NS483 (RHEL-5950)

- add udev rules for trezor hw wallet devices (RHEL-5950)

- hwdb: add axis range corrections for the Lenovo Thinkpad E16 (RHEL-5950)

- hwdb: fix auto rotate on Asus Q551LB (#33921) (RHEL-5950)

- udev: add hwdb execution for hidraw subsystem devices (RHEL-5950)

  

* Wed Aug 07 2024 systemd maintenance team <systemd-maint@redhat.com> - 252-40

- add Requires(post) on selinux-policy (RHEL-46339)

  

* Wed Jul 17 2024 systemd maintenance team <systemd-maint@redhat.com> - 252-39

- enable FIDO2 support (RHEL-36276)

- netif-naming-scheme: disable NAMING_BRIDGE_MULTIFUNCTION_SLOT (RHEL-44630)

- netif-naming-scheme: make actually possible to use rhel-9.5 scheme (RHEL-44630)

- generator: "uninline" generator_open_unit_file and generator_add_symlink (RHEL-33436)

- ci: add support for rhel-only parameters (RHEL-30372)

  

* Wed Jun 19 2024 systemd maintenance team <systemd-maint@redhat.com> - 252-38

- tools: fix the file name that "meson setup" generates (RHEL-30372)

- tools: explicitly specify "setup" subcommand (RHEL-30372)

- fuzz: pass -Dc_args=/-Dcpp_args= to fuzzer targets (RHEL-30372)

- fuzz: don't panic without a C++ compiler (RHEL-30372)

- meson: use ternary op for brevity (RHEL-30372)

  

* Thu Jun 13 2024 systemd maintenance team <systemd-maint@redhat.com> - 252-37

- ci(src-git): add RHEL-9.1 and RHEL-9.1.z to allowed versions (RHEL-30372)

- libsystemd: link with '-z nodelete' (RHEL-6589)

- basic/utf8: make utf8_encoded_to_unichar() return length of the codepoint (RHEL-31219)

- test-gunicode: add new test to show that unichar_iswide() is borked (RHEL-31219)

- string-util: pass ANSI sequences through unchanged (RHEL-31219)

- cryptsetup: do not assert when unsealing token without salt (RHEL-38864)

- cryptsetup: check the existence of salt by salt_size > 0 (RHEL-38864)

- core/mount: if umount(8) fails but mount disappeared, assume success (RHEL-13159)

- Drop log level of header limits log message (RHEL-33890)

- journal: do not rotate unrelated journal files when full or corrupted (RHEL-33890)

- man: suffix --unit with an equal sign, since it expects an argument (RHEL-31070)

- shared: move uid-alloc-range.[ch] from src/shared/ → src/basic/ (RHEL-31070)

- journald: move uid_for_system_journal() to uid-alloc-range.h (RHEL-31070)

- sd-journal: when SD_JOURNAL_CURRENT_USER is set, and called from system UID, imply SD_JOURNAL_SYSTEM (RHEL-31070)

- man: document that journalctl --user requires Storage=persistent (RHEL-31070)

- fix: prefix of dmesg pstore files (RHEL-20322)

- backport new mkosi (RHEL-27512)

- test: Skip various tests when /sys is not mounted (RHEL-27512)

- string-util: introduce ascii_ishex() (RHEL-27512)

- sd-id128: several cleanups (RHEL-27512)

- sd-id128: make id128_read() or friends return -ENOPKG when the file contents is "uninitialized" (RHEL-27512)

- test: add tests for "uninitialized" string handling by id128_read_fd() (RHEL-27512)

- man: mention sd_id128_get_machine() or friend may return -ENOPKG (RHEL-27512)

- sd-id128: make sd_id128_get_boot() and friend return -ENOMEDIUM (RHEL-27512)

- sd-id128: make sd_id128_get_boot() and friend return -ENOSYS when /proc/ is not mounted (RHEL-27512)

- man: mention that sd_id128_get_boot() and friend may return -ENOSYS (RHEL-27512)

- sd-id128: fold do_sync flag into Id128FormatFlag (RHEL-27512)

- sd-id128: make sd_id128_get_machine() or friends return -EUCLEAN when an ID is in an invalid format (RHEL-27512)

- sd-id128: allow sd_id128_get_machine() and friend to be called with NULL (RHEL-27512)

- sd-id128: also refuse an empty invocation ID (RHEL-27512)

- man: update documents for sd_id128_get_invocation() (RHEL-27512)

- test-id128: simplify machine-id check (RHEL-27512)

- test-fs-util: skip part of test_chase_symlinks if machine-id is not initialized (RHEL-27512)

- test-unit-name: simplify machine-id check (RHEL-27512)

- test-load-fragment: simplify machine-id check (RHEL-27512)

- journal: skip part of test-journal-interleaving if no machine-id exists (RHEL-27512)

- test: skip journal tests without valid /etc/machine-id (RHEL-27512)

- test-recurse-dir: work around nftw() ignoring symlinks() (RHEL-27512)

- test: Skip test-recurse-dir on overlayfs (RHEL-27512)

- test-specifier: Ignore -ENOPKG from specifier_printf() (RHEL-27512)

- test-execute: Skip when /sys is read-only (RHEL-27512)

- kernel-install: Make sure KERNEL_INSTALL_BYPASS is disabled in tests (RHEL-27512)

- tools: make sure $KERNEL_INSTALL_BYPASS is disabled when checking help (RHEL-27512)

- test-execute: drop capabilities when testing with user manager (RHEL-27512)

- tmpfiles: Add merge support for copy files action (RHEL-27512)

- generator: add generator_open_unit_file_full to allow creating temporary units (RHEL-27512)

- network-generator: rewrite unit if it already exists and its content changed (RHEL-27512)

- ci: drop super-linter's shellcheck (RHEL-27512)

- mkosi: make sure we build & use RHEL 9 stuff (RHEL-27512)

- ci: backport mkosi CI configuration from upstream (RHEL-27512)

- mkosi: explicitly enroll SecureBoot keys (RHEL-27512)

- test-execute: also mount tmpfs on /dev/shm (RHEL-27512)

- mkosi: fix UKI addons test (RHEL-27512)

- Revert "mkosi: Disable cmdline addon test for now" (RHEL-27512)

- Revert "mkosi: Don't fail on systemd-vconsole-setup.service failure for now" (RHEL-27512)

- mkosi: make shellcheck happy (RHEL-27512)

- mkosi: use pesign for signing UKI addons (RHEL-27512)

- test: copy out the necessary test data before we start overmounting stuff (RHEL-27512)

- ci: make the build dir accessible when running w/o privileges (RHEL-27512)

- ci: explicitly change oom-{score}-adj before running tests (RHEL-27512)

- ratelimit: add ratelimit_left helper (RHEL-35703)

- manager: restrict Dump*() to privileged callers or ratelimit (RHEL-35703)

- ci: define `runas` function inline (RHEL-35703)

- Drop /dev test in test-mountpoint-util (RHEL-30372)

- core/manager: export manager_dbus_is_running (RHEL-40878)

- core: refuse dbus activation if dbus is not running (RHEL-40878)

- core: only refuse Type=dbus service enqueuing if dbus has stop job (RHEL-40878)

- Revert "core/manager: export manager_dbus_is_running" and partially "core: refuse dbus activation if dbus is not running" (RHEL-40878)

- manager: fix reloading in reload-or-restart --marked (RHEL-40878)

- rpm: add `systemd_postun_with_reload` and `systemd_user_postun_with_reload` (RHEL-40878)

- rpm: add `systemd_user_daemon_reexec` (RHEL-40878)

  

* Wed May 22 2024 Jan Macku <jamacku@redhat.com> - 252-35

- spec: return selinux dependencies (RHEL-35732)

  

* Mon May 20 2024 systemd maintenance team <systemd-maint@redhat.com> - 252-34

- ci: update actions/upload-artifact to v4 (RHEL-30372)

- journal-remote: code is of type enum MHD_RequestTerminationCode (RHEL-30372)

- resolve: dns_server_feature_level_*_string type is DnsServerFeatureLevel (RHEL-30372)

- shared|install: Use InstallChangeType consistently (RHEL-30372)

- test: temporarily disable coredumps in testsuite-17.03.sh (RHEL-30372)

- ci: update manpage deployment workflow (RHEL-30372)

- bootspec: fix null-dereference-read (RHEL-36284)

- units: don't install pcrphase-related units without gnu-efi (RHEL-33384)

- kernel-install: fix uki-copy deinstall (RHEL-36505)

- ci(packit): explicitly clone `c9s` branch (RHEL-30372)

  

* Fri Apr 26 2024 systemd maintenance team <systemd-maint@redhat.com> - 252-33

- execute: Pass AT_FDCWD instead of -1 (RHEL-31783)

- ci(src-git): update list of supported products (RHEL-30372)

- coredump: by default process and store core files up to 1GiB (RHEL-15501)

- coredump: keep core files for two weeks (RHEL-15501)

- ukify: make the test happy with the latest OpenSSL (RHEL-30372)

- test_ukify: use raw string for the regex (RHEL-30372)

- coredump: generate stacktraces also for processes running in containers w/o coredump forwarding (RHEL-29430)

- test: add a couple of tests for systemd-coredump (RHEL-29430)

- test: don't expand the subshell expression prematurely (RHEL-29430)

- coredump filter: fix stack overflow with =all (RHEL-29430)

- coredump filter: add mask for 'all' using UINT32_MAX, not UINT64_MAX (RHEL-29430)

- test: add coverage for CoredumpFilter=all (RHEL-29430)

- test: rotate journal before storing coredumps (RHEL-29430)

- test: sync with the fake binary before killing it (RHEL-29430)

- test: check coredump handling in containers & namespaces (RHEL-29430)

  

* Mon Mar 18 2024 Jan Macku <jamacku@redhat.com> - 252-32

- rebase rhel-net-naming-sysattrs to v0.5

  

* Fri Mar 15 2024 systemd maintenance team <systemd-maint@redhat.com> - 252-31

- bootctl: rework random seed logic to use open_mkdir_at() and openat() (RHEL-16952)

- bootctl: properly sync fs before/after moving random seed file into place (RHEL-16952)

- bootctl: when updating EFI random seed file, hash old seed with new one (RHEL-16952)

- sha256: add helper than hashes a buffer *and* its size (RHEL-16952)

- random-seed: don't refresh EFI random seed from random-seed.c anymore (RHEL-16952)

- bootctl: downgrade graceful messages to LOG_NOTICE (RHEL-16952)

- units: rename/rework systemd-boot-system-token.service → systemd-boot-random-seed.service (RHEL-16952)

- bootctl: split out setting of system token into function of its own (RHEL-16952)

  

* Mon Mar 11 2024 systemd maintenance team <systemd-maint@redhat.com> - 252-30

- resolved: limit the number of signature validations in a transaction (RHEL-26643)

- resolved: reduce the maximum nsec3 iterations to 100 (RHEL-26643)

- efi: alignment of the PE file has to be at least 512 bytes (RHEL-26133)

- units: change assert to condition to skip running in initrd/os (RHEL-16182)

- ci: add configuration for regression sniffer GA (RHEL-1086)

  

* Mon Feb 26 2024 systemd maintenance team <systemd-maint@redhat.com> - 252-29

- units: fix typo in Condition in systemd-boot-system-token (RHEL-16952)

  

* Tue Feb 20 2024 systemd maintenance team <systemd-maint@redhat.com> - 252-28

- random-seed: shorten a bit may_credit() (RHEL-16952)

- random-seed: make one more use of random_write_entropy() (RHEL-16952)

- random-seed: use getopt() (RHEL-16952)

- random-seed: make the logic to calculate the number of bytes read from the random seed file clearer (RHEL-16952)

- random-seed: no need to pass 'mode' argument when opening /dev/urandom (RHEL-16952)

- random-seed: split out run() (RHEL-16952)

- random_seed: minor improvement in run() (RHEL-16952)

- random-seed: downgrade some messages (RHEL-16952)

- random-seed: clarify one comment (RHEL-16952)

- random-seed: make sure to load machine id even if the seed file is missing (RHEL-16952)

- chase-symlinks: add new flag for prohibiting any following of symlinks (RHEL-16952)

- bootctl,bootspec: make use of CHASE_PROHIBIT_SYMLINKS whenever we access the ESP/XBOOTLDR (RHEL-16952)

- boot: implement kernel EFI RNG seed protocol with proper hashing (RHEL-16952)

- random-seed: refresh EFI boot seed when writing a new seed (RHEL-16952)

- random-seed: handle post-merge review nits (RHEL-16952)

- boot: do not truncate random seed file (RHEL-16952)

- bootctl: install system token on virtualized systems (RHEL-16952)

- boot: remove random-seed-mode (RHEL-16952)

- stub: handle random seed like sd-boot does (RHEL-16952)

- efi: add efi_guid_equal() helper (RHEL-16952)

- efi: add common implementation for loop finding EFI configuration tables (RHEL-16952)

- boot: Detect hypervisors using SMBIOS info (RHEL-16952)

- boot: Skip soft-brick warning when in a VM (RHEL-16952)

- boot: Replace UINTN with size_t (RHEL-16952)

- boot: Use unsigned for beep counting (RHEL-16952)

- boot: Use unicode literals (RHEL-16952)

- macro: add generic IS_ALIGNED32() anf friends (RHEL-16952)

- meson: use 0|1 for SD_BOOT (RHEL-16952)

- boot: Add printf functions (RHEL-16952)

- boot: Use printf for error logging (RHEL-16952)

- boot: Introduce log_wait (RHEL-16952)

- boot: Add log_trace debugging helper (RHEL-16952)

- tree-wide: Use __func__ in asserts (RHEL-16952)

- boot: Drop use of xpool_print/SPrint (RHEL-16952)

- boot: Drop use of Print (RHEL-16952)

- boot: Rework GUID handling (RHEL-16952)

- efi-string: Fix strchr() null byte handling (RHEL-16952)

- efi-string: Add startswith8() (RHEL-16952)

- efi-string: Add efi_memchr() (RHEL-16952)

- vmm: Add more const (RHEL-16952)

- vmm: Add smbios_find_oem_string() (RHEL-16952)

- stub: Read extra kernel command line items from SMBIOS (RHEL-16952)

- vmm: Modernize get_smbios_table() (RHEL-16952)

- stub: measure SMBIOS kernel-cmdline-extra in PCR12 (RHEL-16952)

- efi: support passing empty cmdline to mangle_stub_cmdline() (RHEL-16952)

- efi: set EFIVAR to stop Shim from uninstalling its protocol (RHEL-16952)

- ukify: use empty stub for addons (RHEL-16952)

- stub: allow loading and verifying cmdline addons (RHEL-16952)

- TODO: remove fixed item (RHEL-16952)

- fix: do not check/verify slice units if recursive errors are to be ignored (RHEL-1086)

  

* Thu Feb 15 2024 systemd maintenance team <systemd-maint@redhat.com> - 252-27

- test: merge TEST-20-MAINPIDGAMES into TEST-07-PID1 (fixup) (RHEL-1086)

- test: use the default nsec3-iterations value (RHEL-1086)

- test: explicitly set nsec3-iterations to 0 (RHEL-1086)

- core: mount namespaces: Remove auxiliary bind mounts directory after unit termination (RHEL-19483)

- ci: deploy systemd man to GitHub Pages (RHEL-1086)

- doc: add missing `<listitem>` to `systemd.net-naming-scheme.xml` (RHEL-7026)

- man: reorder the list of supported naming schemes (RHEL-7026)

- tree-wide: fix return value handling of base64mem() (RHEL-16182)

- Consolidate various TAKE_* into TAKE_GENERIC(), add TAKE_STRUCT() (RHEL-16182)

- pcrphase: add $SYSTEMD_PCRPHASE_STUB_VERIFY env var for overriding stub check (RHEL-16182)

- pcrphase: gracefully exit if TPM2 support is incomplete (RHEL-16182)

- tpm2-util: split out code that derives "good" TPM2 banks into an strv from pcrphase and generalize it in tpm2-util.c (RHEL-16182)

- tpm2-util: split out code that extends a PCR from pcrphase (RHEL-16182)

- tpm2-util: optionally do HMAC in tpm2_extend_bytes() in case we process sensitive data (RHEL-16182)

- cryptsetup: add tpm2-measure-pcr= and tpm2-measure-bank= crypttab options (RHEL-16182)

- man: document the new crypttab measurement options (RHEL-16182)

- gpt-auto-generator: automatically measure root/var volume keys into PCR 15 (RHEL-16182)

- blkid-util: define enum for blkid_do_safeprobe() return values (RHEL-16182)

- pcrphase: make tool more generic, reuse for measuring machine id/fs uuids (RHEL-16182)

- units: measure /etc/machine-id into PCR 15 during early boot (RHEL-16182)

- generators: optionally, measure file systems at boot (RHEL-16182)

- tpm2: add common helper for checking if we are running on UKI with TPM measurements (RHEL-16182)

- man: document new machine-id/fs measurement options (RHEL-16182)

- test: add simple integration test for checking PCR extension works as it should (RHEL-16182)

- update TODO (RHEL-16182)

- cryptsetup: retry TPM2 unseal operation if it fails with TPM2_RC_PCR_CHANGED (RHEL-16182)

- boot: Simplify object erasure (RHEL-16182)

- tree-wide: use CLEANUP_ERASE() at various places (RHEL-16182)

- dlfcn: add new safe_dclose() helper (RHEL-16182)

- tpm2: rename tpm2 alg id<->string functions (RHEL-16182)

- tpm2: rename struct tpm2_context to Tpm2Context (RHEL-16182)

- tpm2: use ref counter for Tpm2Context (RHEL-16182)

- tpm2: use Tpm2Context* instead of ESYS_CONTEXT* (RHEL-16182)

- tpm2: add Tpm2Handle with automatic cleanup (RHEL-16182)

- tpm2: simplify tpm2_seal() blob creation (RHEL-16182)

- tpm2: add salt to pin (RHEL-16182)

- basic/macro: add macro to iterate variadic args (RHEL-16182)

- test/test-macro: add tests for FOREACH_VA_ARGS() (RHEL-16182)

- basic/bitfield: add bitfield operations (RHEL-16182)

- test/test-bitfield: add tests for bitfield macros (RHEL-16182)

- tpm2: add tpm2_get_policy_digest() (RHEL-16182)

- tpm2: add TPM2_PCR_VALID() (RHEL-16182)

- tpm2: add/rename functions to manage pcr selections (RHEL-16182)

- test/test-tpm2: add tests for pcr selection functions (RHEL-16182)

- tpm2: add tpm2_pcr_read() (RHEL-16182)

- tpm2: move openssl-required ifdef code out of policy-building function (RHEL-16182)

- tpm2: add tpm2_is_encryption_session() (RHEL-16182)

- tpm2: move policy building out of policy session creation (RHEL-16182)

- tpm2: add support for a trusted SRK (RHEL-16182)

- tpm2: fix nits from PR #26185 (RHEL-16182)

- tpm2: replace magic number (RHEL-16182)

- tpm2: add tpm2_digest_*() functions (RHEL-16182)

- tpm2: replace hash_pin() with tpm2_digest_*() functions (RHEL-16182)

- tpm2: add tpm2_set_auth() (RHEL-16182)

- tpm2: add tpm2_get_name() (RHEL-16182)

- tpm2: rename pcr_values_size vars to n_pcr_values (RHEL-16182)

- tpm2: add tpm2_policy_pcr() (RHEL-16182)

- tpm2: add tpm2_policy_auth_value() (RHEL-16182)

- tpm2: add tpm2_policy_authorize() (RHEL-16182)

- tpm2: use tpm2_policy_authorize() (RHEL-16182)

- tpm2: add tpm2_calculate_sealing_policy() (RHEL-16182)

- tpm: remove external calls to dlopen_tpm2() (RHEL-16182)

- tpm2: remove all extern tpm2-tss symbols (RHEL-16182)

- tpm2: add tpm2_get_capability(), tpm2_cache_capabilities(), tpm2_capability_pcrs() (RHEL-16182)

- tpm2: verify symmetric parms in tpm2_context_new() (RHEL-16182)

- tpm2: replace _cleanup_tpm2_* macros with _cleanup_() (RHEL-16182)

- tpm2-util: use compound initialization when allocating tpm2 objects (RHEL-16182)

- tpm2: add tpm2_get_capability_handle(), tpm2_esys_handle_from_tpm_handle() (RHEL-16182)

- tpm2: add tpm2_read_public() (RHEL-16182)

- tpm2: add tpm2_get_legacy_template() and tpm2_get_srk_template() (RHEL-16182)

- tpm2: add tpm2_load() (RHEL-16182)

- tpm2: add tpm2_load_external() (RHEL-16182)

- tpm2: move local vars in tpm2_seal() to point of use (RHEL-16182)

- tpm2: replace magic number in hmac_sensitive initialization (RHEL-16182)

- tpm2: add tpm2_create() (RHEL-16182)

- tpm2: replace tpm2_capability_pcrs() macro with direct c->capaiblity_pcrs use (RHEL-16182)

- basic/alloc-util: add greedy_realloc_append() (RHEL-16182)

- tpm2: cache the TPM supported commands, add tpm2_supports_command() (RHEL-16182)

- tpm2: cache TPM algorithms (RHEL-16182)

- tpm2: add tpm2_persist_handle() (RHEL-16182)

- tpm2: add tpm2_get_or_create_srk() (RHEL-16182)

- tpm2: move local vars in tpm2_unseal() to point of use (RHEL-16182)

- tpm2: remove tpm2_make_primary() (RHEL-16182)

- tpm2: use CreatePrimary() to create primary keys instead of Create() (RHEL-16182)

- cryptsetup: downgrade a bunch of log messages that to LOG_WARNING (RHEL-16182)

- boot/measure: replace TPM PolicyPCR session with calculation (RHEL-16182)

- core: imply DeviceAllow=/dev/tpmrm0 with LoadCredentialEncrypted (RHEL-16182)

- added more test cases (RHEL-16182)

- test: fixed negative checks in TEST-70-TPM2. Use in-line error handling rather than redirections. Follow up on #27020 (RHEL-16182)

- systemd-cryptenroll: add string aliases for tpm2 PCRs Fixes #26697. RFE. (RHEL-16182)

- cryptenroll: fix an assertion with weak passwords (RHEL-16182)

- man/systemd-cryptenroll: update list of PCRs, link to uapi docs (RHEL-16182)

- tpm2: add debug logging to functions converting hash or asym algs to/from strings or ids (RHEL-16182)

- tpm2: add tpm2_hash_alg_to_size() (RHEL-16182)

- tpm2: change tpm2_tpm*_pcr_selection_to_mask() to return mask (RHEL-16182)

- tpm2: add more helper functions for managing TPML_PCR_SELECTION and TPMS_PCR_SELECTION (RHEL-16182)

- tpm2: add Tpm2PCRValue struct and associated functions (RHEL-16182)

- tpm2: move declared functions in header lower down (RHEL-16182)

- tpm2: declare tpm2_log_debug_*() functions in tpm2_util.h (RHEL-16182)

- tpm2: change tpm2_calculate_policy_pcr(), tpm2_calculate_sealing_policy() to use Tpm2PCRValue array (RHEL-16182)

- tpm2: change tpm2_parse_pcr_argument() parameters to parse to Tpm2PCRValue array (RHEL-16182)

- tpm2: add TPM2B_*_MAKE(), TPM2B_*_CHECK_SIZE() macros (RHEL-16182)

- tpm2: add tpm2_pcr_read_missing_values() (RHEL-16182)

- openssl: add openssl_pkey_from_pem() (RHEL-16182)

- openssl: add rsa_pkey_new(), rsa_pkey_from_n_e(), rsa_pkey_to_n_e() (RHEL-16182)

- openssl: add ecc_pkey_new(), ecc_pkey_from_curve_x_y(), ecc_pkey_to_curve_x_y() (RHEL-16182)

- test: add DEFINE_HEX_PTR() helper function (RHEL-16182)

- openssl: add test-openssl (RHEL-16182)

- tpm2: add functions to convert TPM2B_PUBLIC to/from openssl pkey or PEM (RHEL-16182)

- tpm2: move policy calculation out of tpm2_seal() (RHEL-16182)

- man: update systemd-cryptenroll man page with details on --tpm2-pcrs format change (RHEL-16182)

- tpm2: update TEST-70-TPM2 to test passing PCR value to systemd-cryptenroll (RHEL-16182)

- tpm2: change *alg_to_* functions to use switch() (RHEL-16182)

- tpm2: lowercase TPM2_PCR_VALUE[S]_VALID functions (RHEL-16182)

- tpm2: move cast from lhs to rhs in uint16_t/int comparison (RHEL-16182)

- tpm2: in validator functions, return false instead of assert failure (RHEL-16182)

- tpm2: in tpm2_pcr_values_valid() use FOREACH_ARRAY() (RHEL-16182)

- tpm2: use SIZE_MAX instead of strlen() for unhexmem() (RHEL-16182)

- tpm2: put !isempty() check inside previous !isempty() check (RHEL-16182)

- tpm2: simplify call to asprintf() (RHEL-16182)

- tpm2: check pcr value hash != 0 before looking up hash algorithm name (RHEL-16182)

- tpm2: use strempty() (RHEL-16182)

- tpm2: split TPM2_PCR_VALUE_MAKE() over multiple lines (RHEL-16182)

- tpm2: remove ret_ prefix from input/output params (RHEL-16182)

- tpm2: use memcpy_safe() instead of memcpy() (RHEL-16182)

- openssl: use new(char, size) instead of malloc(size) (RHEL-16182)

- tpm2: use table for openssl<->tpm2 ecc curve id mappings (RHEL-16182)

- tpm2: use switch() instead of if-else (RHEL-16182)

- tpm2: make logging level consistent at debug for some functions (RHEL-16182)

- tpm2: remove unnecessary void* cast (RHEL-16182)

- tpm2: add tpm2_pcr_values_has_(any|all)_values() functions (RHEL-16182)

- tpm2: wrap (7) in UINT32_C() (RHEL-16182)

- cryptenroll: change man page example to remove leading 0x and lowercase hex (RHEL-16182)

- openssl: add log_openssl_errors() (RHEL-16182)

- openssl: add openssl_digest_size() (RHEL-16182)

- openssl: add openssl_digest_many() (RHEL-16182)

- openssl: replace openssl_hash() with openssl_digest() (RHEL-16182)

- openssl: add openssl_hmac_many() (RHEL-16182)

- openssl: add rsa_oaep_encrypt_bytes() (RHEL-16182)

- openssl: add kdf_kb_hmac_derive() (RHEL-16182)

- openssl: add openssl_cipher_many() (RHEL-16182)

- openssl: add ecc_edch() (RHEL-16182)

- openssl: add kdf_ss_derive() (RHEL-16182)

- dlfcn-util: add static asserts ensuring our sym_xyz() func ptrs match the types from the official headers (RHEL-16182)

- tpm2: add tpm2_marshal_blob() and tpm2_unmarshal_blob() (RHEL-16182)

- tpm2: add tpm2_serialize() and tpm2_deserialize() (RHEL-16182)

- tpm2: add tpm2_index_to_handle() and tpm2_index_from_handle() (RHEL-16182)

- tpm2: fix build failure without openssl (RHEL-16182)

- tpm2-util: look for tpm2-pcr-signature.json directly in /.extra/ (RHEL-16182)

- tpm2: downgrade most log functions from error to debug (RHEL-16182)

- tpm2: handle older tpm enrollments without a saved pcr bank (RHEL-16182)

- tpm2: allow tpm2_make_encryption_session() without bind key (RHEL-16182)

- tpm2: update tpm2 test for supported commands (RHEL-16182)

- tpm2: use GREEDY_REALLOC_APPEND() in tpm2_get_capability_handles(), cap max value (RHEL-16182)

- tpm2: change tpm2_unseal() to accept Tpm2Context instead of device string (RHEL-16182)

- tpm2: cache TPM's supported ECC curves (RHEL-16182)

- tpm2-util: make tpm2_marshal_blob()/tpm2_unmarshal_blob() static (RHEL-16182)

- tpm2-util: make tpm2_read_public() static, as we use it only internally in tpm2-util.c (RHEL-16182)

- cryptenroll: allow specifying handle index of key to use for sealing (RHEL-16182)

- test: add tests for systemd-cryptenroll --tpm2-seal-key-handle (RHEL-16182)

- tpm2: do not call Esys_TR_Close() (RHEL-16182)

- tpm2: don't use GetCapability() to check transient handles (RHEL-16182)

- tpm2-util: pick up a few new symbols from tpm2-tss (RHEL-16182)

- tpm2: add tpm2_get_pin_auth() (RHEL-16182)

- tpm2: instead of adjusting authValue trailing 0(s), trim them as required by tpm spec (RHEL-16182)

- tpm2-util: rename tpm2_calculate_name() → tpm2_calculate_pubkey_name() (RHEL-16182)

- cryptenroll: do not implicitly verify with default tpm policy signature (RHEL-16182)

- cryptenroll: drop deadcode (RHEL-16182)

- tpm2: allow using tpm2_get_srk_template() without tpm (RHEL-16182)

- tpm2: add test to verify srk templates (RHEL-16182)

- tpm2: add tpm2_sym_alg_*_string() and tpm2_sym_mode_*_string() (RHEL-16182)

- tpm2: add tpm2_calculate_seal() and helper functions (RHEL-16182)

- tpm2: update test-tpm2 for tpm2_calculate_seal() (RHEL-16182)

- cryptenroll: add support for calculated TPM2 enrollment (RHEL-16182)

- test: update TEST-70 with systemd-cryptenroll calculated TPM2 enrollment (RHEL-16182)

- openssl-util: avoid freeing invalid pointer (RHEL-16182)

- creds-util: check for CAP_DAC_READ_SEARCH (RHEL-16182)

- creds-util: do not try TPM2 if there is not support (RHEL-16182)

- creds-util: merge the TPM2 detection for initrd (RHEL-16182)

- cryptenroll: fix a memory leak (RHEL-16182)

- sd-journal: introduce sd_journal_step_one() (RHEL-11591)

- test: modernize test-journal-flush (RHEL-11591)

- journal-file-util: do not fail when journal_file_set_offline() called more than once (RHEL-11591)

- journal-file-util: Prefer punching holes instead of truncating (RHEL-11591)

- test: add reproducer for SIGBUS issue caused by journal truncation (RHEL-11591)

  

* Wed Jan 31 2024 systemd maintenance team <systemd-maint@redhat.com> - 252-26

- spec: update rhel-net-naming-sysattrs to v0.4 (RHEL-22278)

  

* Tue Jan 30 2024 systemd maintenance team <systemd-maint@redhat.com> - 252-25

- spec: add new package with RHEL-specific network naming sysattrs (RHEL-22278)

  

* Wed Jan 24 2024 systemd maintenance team <systemd-maint@redhat.com> - 252-24

- ci: use source-git-automation composite Action (RHEL-1086)

- ci: increase the cron interval to 45 minutes (RHEL-1086)

- ci: add all Z-Stream versions to array of allowed versions (RHEL-1086)

- udev/net_id: introduce naming scheme for RHEL-9.4 (RHEL-22427)

- basic/errno-util: add wrappers which only accept negative errno (RHEL-22443)

- errno-util: allow ERRNO_IS_* to accept types wider than int (RHEL-22443)

- udev: add new builtin net_driver (RHEL-22443)

- udev/net_id: introduce naming scheme for RHEL-8.10 (RHEL-22427)

  

* Fri Jan 12 2024 systemd maintenance team <systemd-maint@redhat.com> - 252-23

- logind: don't setup idle session watch for lock-screen and greeter (RHEL-20757)

- logind: don't make idle action timer accuracy more coarse than timeout (RHEL-20757)

- logind: do TTY idle logic only for sessions marked as "tty" (RHEL-20757)

- meson: Properly install 90-uki-copy.install (RHEL-16354)

  

* Mon Jan 08 2024 systemd maintenance team <systemd-maint@redhat.com> - 252-22

- Revert "man: mention System Administrator's Guide in systemctl manpage" (RHEL-19436)

- man: mention RHEL documentation in systemctl's man page (RHEL-19436)

- resolved: actually check authenticated flag of SOA transaction (RHEL-6216)

- udev: allow/denylist for reading sysfs attributes when composing a NIC name (RHEL-1317)

- man: environment value -> udev property (RHEL-1317)

  

* Mon Dec 11 2023 systemd maintenance team <systemd-maint@redhat.com> - 252-21

- meson: fix installation of ukify (RHEL-13199)

- sd-id128: introduce id128_hash_ops_free (RHEL-5988)

- udevadm-trigger: allow to fallback without synthetic UUID only first time (RHEL-5988)

- udevadm-trigger: settle with synthetic UUID if the kernel support it (RHEL-5988)

- udevadm-trigger: also check with the original syspath if device is renamed (RHEL-5988)

- test: use 'udevadm trigger --settle' even if device is renamed (RHEL-5988)

- sd-event: don't mistake USEC_INFINITY passed in for overflow (RHEL-6090)

- pid1: rework service_arm_timer() to optionally take a relative time value (RHEL-6090)

- manager: add one more assert() (RHEL-6090)

- pid1: add new Type=notify-reload service type (RHEL-6090)

- man: document Type=notify-reload (RHEL-6090)

- pid1: make sure we send our calling service manager RELOADING=1 when reloading (RHEL-6090)

- networkd: implement Type=notify-reload protocol (RHEL-6090)

- udevd: implement the full Type=notify-reload protocol (RHEL-6090)

- logind: implement Type=notify-reload protocol properly (RHEL-6090)

- notify: add --stopping + --reloading switches (RHEL-6090)

- test: add Type=notify-reload testcase (RHEL-6090)

- update TODO (RHEL-6090)

- core: check for SERVICE_RELOAD_NOTIFY in manager_dbus_is_running (RHEL-6090)

  

* Fri Dec 08 2023 systemd maintenance team <systemd-maint@redhat.com> - 252-20

- udev/net: allow new link name as an altname before renaming happens (RHEL-5988)

- sd-netlink: do not swap old name and alternative name (RHEL-5988)

- sd-netlink: restore altname on error in rtnl_set_link_name (RHEL-5988)

- udev: attempt device rename even if interface is up (RHEL-5988)

- sd-netlink: add a test for rtnl_set_link_name() (RHEL-5988)

- test-network: add a test for renaming device to current altname (RHEL-5988)

- udev: align table (RHEL-5988)

- sd-device: make device_set_syspath() clear sysname and sysnum (RHEL-5988)

- sd-device: do not directly access entry in sd-device object (RHEL-5988)

- udev: move device_rename() from device-private.c (RHEL-5988)

- udev: restore syspath and properties on failure (RHEL-5988)

- sd-device: introduce device_get_property_int() (RHEL-5988)

- core/device: downgrade log level for ignored errors (RHEL-5988)

- core/device: ignore failed uevents (RHEL-5988)

- test: add tests for failure in renaming network interface (RHEL-5988)

- test: modernize test-netlink.c (RHEL-5988)

- test-netlink: use dummy interface to test assigning new interface name (RHEL-5988)

- udev: use SYNTHETIC_ERRNO() at one more place (RHEL-5988)

- udev: make udev_builtin_run() take UdevEvent* (RHEL-5988)

- udev/net: verify ID_NET_XYZ before trying to assign it as an alternative name (RHEL-5988)

- udev/net: generate new network interface name only on add uevent (RHEL-5988)

- sd-netlink: make rtnl_set_link_name() optionally append alternative names (RHEL-5988)

- udev/net: assign alternative names only on add uevent (RHEL-5988)

- test: add tests for renaming network interface (RHEL-5988)

- Backport ukify from upstream (RHEL-13199)

- bootctl: make --json output normal json (RHEL-13199)

- test: replace readfp() with read_file() (RHEL-13199)

- stub/measure: document and measure .uname UKI section (RHEL-13199)

- boot: measure .sbat section (RHEL-13199)

- Revert "test_ukify: no stinky root needed for signing" (RHEL-13199)

- ukify: move to /usr/bin and mark as non non-experimental (RHEL-13199)

- kernel-install: Add uki layout (RHEL-16354)

- kernel-install: remove math slang from man page (RHEL-16354)

- kernel-install: handle uki installs automatically (RHEL-16354)

- 90-uki-copy.install: create $BOOT/EFI/Linux directory if needed (RHEL-16354)

- kernel-install: Log location that uki is installed in (RHEL-16354)

- bootctl: fix errno logging (RHEL-16354)

- bootctl: add kernel-identity command (RHEL-16354)

- bootctl: add kernel-inspect command (RHEL-16354)

- bootctl: add kernel-inspect to --help text (RHEL-16354)

- bootctl: drop full stop at end of --help texts (RHEL-16354)

- bootctl: change section title for kernel image commands (RHEL-16354)

- bootctl: remove space that should not be there (RHEL-16354)

- bootctl: kernel-inspect: print os info (RHEL-16354)

- bootctl-uki: several coding style fixlets (RHEL-16354)

- tree-wide: unify how we pick OS pretty name to display (RHEL-16354)

- bootctl-uki: several follow-ups for inspect_osrel() (RHEL-16354)

- bootctl: Add missing %m (RHEL-16354)

- bootctl: tweak DOS header magic check (RHEL-16354)

  

* Mon Nov 13 2023 systemd maintenance team <systemd-maint@redhat.com> - 252-19

- ci: Extend source-git-automation (RHEL-1086)

- netif-naming-scheme: let's also include rhel8 schemes (RHEL-7026)

- systemd-analyze: Add table and JSON output implementation to plot (RHEL-5070)

- systemd-analyze: Update man/systemd-analyze.xml with Plot JSON and table (RHEL-5070)

- systemd-analyze: Add tab complete logic for plot (RHEL-5070)

- systemd-analyze: Add --json=, --table and -no-legend tests for plot (RHEL-5070)

- ci: enable source-git automation to validate reviews and ci results (RHEL-1086)

- ci: remove Mergify config - replaced by Pull Request Validator (RHEL-1086)

- ci: enable auto-merge GH Action (RHEL-1086)

- ci: add missing permissions (RHEL-1086)

- ci: `permissions: write-all` (RHEL-1086)

- ci(lint): exclude `.in` files from ShellCheck lint (RHEL-1086)

- udev: raise RLIMIT_NOFILE as high as we can (RHEL-11040)

  

* Tue Aug 22 2023 systemd maintenance team <systemd-maint@redhat.com> - 252-18

- doc: add downstream CONTRIBUTING document (#2170883)

- doc: improve CONTRIBUTING document (#2170883)

- doc: use link with prefilled Jira issue (#2170883)

- docs: link downstream CONTRIBUTING in README (#2170883)

- bpf: fix restrict_fs on s390x (#2230364)

- udev/net_id: use naming scheme for RHEL-9.3 (#2231845)

- core/timer: Always use inactive_exit_timestamp if it is set (#2211065)

- timer: Use dual_timestamp_is_set() in one more place (#2211065)

- loginctl: list-users: also show state (#2209912)

- loginctl: list-sessions: minor modernization (#2209912)

- loginctl: list-sessions: also show state (#2209912)

- test: add test for state in loginctl list-{users,sessions} (#2209912)

- test: add a missing session activation (#2209912)

- test: extend test for loginctl list-* (#2209912)

- loginctl: shorten variable name (#2209912)

- loginctl: use bus_map_all_properties (#2209912)

- loginctl: show session idle status in list-sessions (#2209912)

- loginctl: some modernizations (#2209912)

- loginctl: list-sessions: fix timestamp for idle hint (#2209912)

- loginctl: list-users: use bus_map_all_properties (#2209912)

- loginctl: also show idle hint in session-status (#2209912)

- memory-util: make ArrayCleanup passed to array_cleanup() const (#2190226)

- static-destruct: several cleanups (#2190226)

- static-destruct: introduce STATIC_ARRAY_DESTRUCTOR_REGISTER() (#2190226)

- macro: support the case that the number of elements has const qualifier (#2190226)

- shared/generator: apply similar config reordering of generated units (#2190226)

- nulstr-util: make ret_size in strv_make_nulstr() optional (#2190226)

- generator: teach generator_add_symlink() to instantiate specified unit (#2190226)

- units: rework growfs units to be just a regular unit that is instantiated (#2190226)

- fstab-generator: use correct targets when /sysroot is specificied in fstab only (#2190226)

- fstab-generator: add SYSTEMD_SYSFS_CHECK env var (#2190226)

- test: add fstab file support for fstab-generator tests (#2190226)

- test-fstab-generator: also check file contents (#2190226)

- test-fstab-generator: add tests for mount options (#2190226)

- fstab-generator: split out several functions from parse_fstab() (#2190226)

- fstab-generator: call add_swap() earlier (#2190226)

- fstab-generator: refuse to add swap earlier if disabled (#2190226)

- fstab-generator: refuse invalid mount point path in fstab earlier (#2190226)

- fstab-generator: fix error code propagation in run_generator() (#2190226)

- fstab-generator: support defining mount units through kernel command line (#2190226)

- test: add test cases for defining mount and swap units from kernel cmdline (#2190226)

- generators: change TimeoutSec=0 to TimeoutSec=infinity (#2190226)

- units: change TimeoutSec=0 to TimeoutSec=infinity (#2190226)

- fstab-generator: use correct swap name var (#2190226)

- fstab-generator: add more parameter name comments (#2190226)

- fstab-generator: unify initrd-root-device.target dependency handling code (#2190226)

- fstab-util: add fstab_is_bind (#2190226)

- fstab-generator: resolve bind mount source when in initrd (#2190226)

- fstab-generator: rename 'initrd' flag to 'prefix_sysroot' (#2190226)

- fstab-generator: fix target of /sysroot/usr (#2190226)

- fstab-generator: add rd.systemd.mount-extra= and friends (#2190226)

- fstab-generator: add a flag to accept entry for "/" in initrd (#2190226)

- test-fstab-generator: extract core part as a function (#2190226)

- test-fstab-generator: also test with SYSTEMD_IN_INITRD=no (#2190226)

- test-fstab-generator: add more tests for systemd.mount-extra= and friends (#2190226)

- fstab-generator: enable fsck for block device mounts specified in systemd.mount-extra= (#2190226)

- core: use correct scope of looking up units (#2226980)

- test: merge unit file related tests into TEST-23-UNIT-FILE (#2213521)

- test: rename TEST-07-ISSUE-1981 to TEST-07-PID1 (#2213521)

- test: merge TEST-08-ISSUE-2730 into TEST-07-PID1 (#2213521)

- test: merge TEST-09-ISSUE-2691 into TEST-07-PID1 (#2213521)

- test: merge TEST-10-ISSUE-2467 with TEST-07-PID1 (#2213521)

- test: merge TEST-11-ISSUE-3166 into TEST-07-PID1 (#2213521)

- test: merge TEST-12-ISSUE-3171 into TEST-07-PID1 (#2213521)

- test: move TEST-23's units into a dedicated subfolder (#2213521)

- test: merge TEST-47-ISSUE-14566 into TEST-07-PID1 (#2213521)

- test: merge TEST-51-ISSUE-16115 into TEST-07-PID1 (#2213521)

- test: merge TEST-20-MAINPIDGAMES into TEST-07-PID1 (#2213521)

- test: abstract the common test parts into a utility script (#2213521)

- test: add tests for JoinsNamespaceOf= (#2213521)

- core/unit: drop doubled empty line (#2213521)

- core/unit: make JoinsNamespaceOf= implies the inverse dependency (#2213521)

- core/unit: search shared namespace in transitive relation of JoinsNamespaceOf= (#2213521)

- core/unit: update bidirectional dependency simultaneously (#2213521)

- resolvectl: fix type of ifindex D-Bus field, and make sure to initialize to zero in all code paths (#2161260)

- resolved: add some line-breaks/comments (#2161260)

- resolvectl: don't filter loopback DNS server from global DNS server list (#2161260)

- blockdev-util: add simple wrapper around BLKSSZGET (#2170883)

- loop-util: insist on setting the sector size correctly (#2170883)

- dissect-image: add probe_sector_size() helper for detecting sector size of a GPT disk image (#2170883)

- loop-util: always tell kernel explicitly about loopback sector size (#2170883)

- Revert "Treat EPERM as "not available" too" (#2178222)

- Revert "test: accept EPERM for unavailable idmapped mounts as well" (#2178222)

  

* Fri Aug 04 2023 systemd maintenance team <systemd-maint@redhat.com> - 252-17

- Revert "core/service: when resetting PID also reset known flag" (#2225667

- ci: explicitly install python3-lldb-$COMPILER_VERSION (#2225667)

  

* Mon Jul 17 2023 systemd maintenance team <systemd-maint@redhat.com> - 252-16

- ci: update permissions for source-git automation workflows (#2170883)

- pstore: fixes for dmesg.txt reconstruction (#2170883)

- pstore: explicitly set the base when converting record ID (#2170883)

- pstore: avoid opening the dmesg.txt file if not requested (#2170883)

- test: add a couple of tests for systemd-pstore (#2170883)

- test: match all messages with the FILE field (#2170883)

- test: build the SELinux test module on the host (#2170883)

- test: make the stress test slightly less stressful on slower machines (#2170883)

- coredump: use unaligned_read_ne{32,64}() to parse auxv (#2170883)

- core/transaction: make merge_unit_ids() always return NUL-terminated string (#2170883)

- core/transaction: make merge_unit_ids() return non-NULL on success (#2170883)

- core/transaction: do not log "(null)" (#2170883)

- ci: allow `RHEL-only` labels to mark downstream-only commits (#2170883)

- elf-util: discard PT_LOAD segment early based on the start address. (#2215412)

- elf-util: check for overflow when computing end of core's PT_LOAD segments (#2215412)

- sulogin: use DEFINE_MAIN_FUNCTION() (#2169959)

- sulogin: fix control lost of the current terminal when default.target is rescue.target (#2169959)

- journal-vacuum: count size of all journal files (#2182632)

- memory-util: add a concept for gcc cleanup attribute based array destruction (#2182632)

- macro: introduce FOREACH_ARRAY() macro (#2182632)

- journal-vacuum: rename function to match struct name (#2182632)

- journal-vacuum: use CLEANUP_ARRAY (#2182632)

- pam: add call to pam_umask (#2210145)

- udev-builtin-net_id: align VF representor names with VF names (#2218886)

- pam: add a call to pam_namespace (#2218184)

- rules: online CPU automatically on IBM s390x platforms when configured (#2212612)

- core/mount: escape invalid UTF8 char in dbus reply (#2208240)

- Revert "user: delegate cpu controller, assign weights to user slices" (#2176899)

- udev-rules: fix nvme symlink creation on namespace changes (#2172509)

- rules: add whitespace after comma before the line continuation (#2172509)

- udev: restore compat symlink for nvme devices (#2172509)

- rules: drop doubled space (#2172509)

- manager: don't taint the host if cgroups v1 is used (#2193456)

- core/service: when resetting PID also reset known flag (#2210237)

- ci: drop systemd-stable from advanced-commit-linter config (#2170883)

  

* Thu May 18 2023 systemd maintenance team <systemd-maint@redhat.com> - 252-15

- ci: trigger `differential-shellcheck` workflow on push (#2100440)

- ci: workflow for gathering metadata for source-git automation (#2100440)

- ci: first part of the source-git automation - commit linter (#2100440)

- ci(Mergify): check CodeQL and build workflows based on changed files (#2100440)

- ci: add NOTICE to also update regexp in `.mergify.yml` when updating `paths` property (#2100440)

- Support /etc/system-update for OSTree systems (#2203133)

- journal-def: fix type of signature to match the actual field in the Header structure (#2183546)

- journal: use compound initialization for journal file Header structure (#2183546)

- journald: fix log message (#2183546)

- sd-journal: cache results of parsing environment variables (#2183546)

- compress: introduce compression_supported() helper function (#2183546)

- sd-journal: always use the compression algorithm specified in the header (#2183546)

- sd-journal: allow to specify compression algorithm through env (#2183546)

- test: add test case that journal file is created with the requested compression algorithm (#2183546)

- rules: do not online CPU automatically on IBM platforms (#2143107)

  

* Tue Mar 21 2023 systemd maintenance team <systemd-maint@redhat.com> - 252-14

- systemd: Support OOMPolicy in scope units (#2176918)

- systemd: Default to OOMPolicy=continue for login session scopes (#2176918)

- man: rework description of OOMPolicy= a bit (#2176918)

- core,man: add missing integration of OOMPolicy= in scopes (#2176918)

- meson: Store fuzz tests in structured way (#2176918)

- meson: Generate fuzzer inputs with directives (#2176918)

- oss-fuzz: include generated corpora in the final zip file (#2176918)

- unit: In cgroupv1, gracefully terminate delegated scopes again (#2180120)

  

* Mon Feb 27 2023 systemd maintenance team <systemd-maint@redhat.com> - 252-8

- journal-file: Fix return value in bump_entry_array() (#2173682)

  

* Mon Feb 27 2023 systemd maintenance team <systemd-maint@redhat.com> - 252-7

- test: add coverage for #24177 (#1985288)

- logind-session: make stopping of idle session visible to admins (#2172401)

  

* Wed Feb 22 2023 systemd maintenance team <systemd-maint@redhat.com> - 252-6

- journalctl: actually run the static destructors (#2122500)

- efi: drop executable-stack bit from .elf file (#2140646)

- install: fail early if specifier expansion failed (#2138081)

- test: add coverage for #26467 (#2138081)

  

* Fri Feb 17 2023 systemd maintenance team <systemd-maint@redhat.com> - 252-5

- nss-myhostname: fix inverted condition in (#2167468)

- nss-myhostname: do not return empty result with NSS_STATUS_SUCCESS (#2167468)

- sleep: rename hibernate_delay_sec -> _usec (#2151612)

- sleep: fetch_batteries_capacity_by_name() does not return -ENOENT (#2151612)

- sleep: drop unnecessary temporal vaiable and initialization (#2151612)

- sleep: introduce SuspendEstimationSec= (#2151612)

- sleep: coding style fixlets (#2151612)

- sleep: simplify code a bit (#2151612)

- sleep: fix indentation (#2151612)

- sleep: enumerate only existing and non-device batteries (#2151612)

- core: when isolating to a unit, also keep units running that are triggered by units we keep running (#1952378)

- udev/net_id: introduce naming scheme for RHEL-9.2 (#2170500)

  

* Mon Feb 06 2023 systemd maintenance team <systemd-maint@redhat.com> - 252-4

- udev: make get_virtfn_info() provide physical PCI device (#2159448)

- test: make helper_check_device_units() log unit name (#2138081)

- test: add a testcase for lvextend (#2138081)

- pid1: fix segv triggered by status query (#26279) (#2138081)

- test: create config under /run (#2138081)

- test: add tests for mDNS and LLMNR settings (#2138081)

- resolved: introduce the _localdnsstub and _localdnsproxy special hostnames for 127.0.0.54 + 127.0.0.53 (#2138081)

- test: wait for the monitoring service to become active (#2138081)

- test: suppress echo in monitor_check_rr() (#2138081)

- Revert "test: wait for the monitoring service to become active" (#2138081)

- test: show and check almost all journal entries since the relevant command being invoked (#2138081)

- test: cover IPv6 in the resolved test suite (#2138081)

- test: add a couple of SRV records to check service resolution (#2138081)

- test: add a test for the OPENPGPKEY RR (#2138081)

- test: don't hang indefinitely on no match (#2138081)

- test-ndisc: fix memleak and fd leak (#2138081)

- test-unit-name: fix fd leak (#2138081)

- test: bump D-Bus service start timeout if we run without accel (#2138081)

- test: bump the client-side timeout in sd-bus as well (#2138081)

- test: bump the container spawn timeout to 60s (#2138081)

- network: fix memleak (#2138081)

- busctl: fix introspecting DBus properties (#2138081)

- busctl: simplify peeking the type (#2138081)

- resolve: drop redundant call of socket_ipv6_is_supported() (#2138081)

- resolve: introduce link_get_llmnr_support() and link_get_mdns_support() (#2138081)

- resolve: provide effective supporting levels of mDNS and LLMNR (#2138081)

- resolvectl: warn if the global mDNS or LLMNR support level is lower than the requested one (#2138081)

- resolve: enable per-link mDNS setting by default (#2138081)

  

* Mon Jan 16 2023 systemd maintenance team <systemd-maint@redhat.com> - 252-3

- swap: tell swapon to reinitialize swap if needed (#2151993)

- coredump: adjust whitespace (#2155517)

- coredump: do not allow user to access coredumps with changed uid/gid/capabilities (#2155517)

- Revert "basic: add fallback in chase_symlinks_and_opendir() for cases when /proc is not mounted" (#2138081)

- glyph-util: add warning sign special glyph (#2138081)

- chase-symlink: when converting directory O_PATH fd to real fd, don't bother with /proc/ (#2138081)

- systemctl: print a clear warning if people invoke systemctl without /proc/ (#2138081)

- TEST-65: check cat-config operation in chroot (#2138081)

- TEST-65: use [[ -v ]] more (#2138081)

- systemctl: warn if trying to disable a unit with no install info (#2141979)

- systemctl: allow suppress the warning of no install info using --no-warn (#2141979)

- rpm/systemd-update-helper: use --no-warn when disabling units (#2141979)

- systemctl: suppress warning about missing /proc/ when --no-warn (#2141979)

- shell-completion: systemctl: add --no-warn (#2141979)

- core/unit: drop doubled empty line (#2160477)

- core/unit: drop dependency to the unit being merged (#2160477)

- core/unit: fix logic of dropping self-referencing dependencies (#2160477)

- core/unit: merge two loops into one (#2160477)

- test: add test case for sysv-generator and invalid dependency (#2160477)

- core/unit: merge unit names after merging deps (#2160477)

- core/unit: fix log message (#2160477)

- test: explicitly create the /etc/init.d directory (#2160477)

- test: support a non-default SysV directory (#2160477)

  

* Fri Dec 09 2022 systemd maintenance team <systemd-maint@redhat.com> - 252-2

- test: check if we can use SHA1 MD for signing before using it (#2141979)

- boot: cleanups for efivar_get() and friends (#2141979)

- boot: fix false maybe-uninitialized warning (#2141979)

- tree-wide: modernizations with RET_NERRNO() (#2137584)

- sd-bus: handle -EINTR return from bus_poll() (#2137584)

- stdio-bridge: don't be bothered with EINTR (#2137584)

- varlink: also handle EINTR gracefully when waiting for EIO via ppoll() (#2137584)

- sd-netlink: handle EINTR from poll() gracefully, as success (#2137584)

- resolved: handle -EINTR returned from fd_wait_for_event() better (#2137584)

- homed: handle EINTR gracefully when waiting for device node (#2137584)

- utmp-wtmp: fix error in case isatty() fails (#2137584)

- utmp-wtmp: handle EINTR gracefully when waiting to write to tty (#2137584)

- io-util: document EINTR situation a bit (#2137584)

- terminal-util: Set OPOST when setting ONLCR (#2138081)

- cgtop: Do not rewrite -P or -k options (#2138081)

- test: Add tests for systemd-cgtop args parsing (#2138081)

- resolved: remove inappropriate assert() (#2138081)

- boot: Add xstrn8_to_16 (#2138081)

- boot: Use xstr8_to_16 (#2138081)

- boot: Use xstr8_to_16 for path conversion (#2138081)

-    stub: Fix cmdline handling (#2138081)

- stub: Detect empty LoadOptions when run from EFI shell (#2138081)

- boot: Use EFI_BOOT_MANAGER_POLICY_PROTOCOL to connect console devices (#2138081)

- boot: Make sure all partitions drivers are connected (#2138081)

- boot: improve support for qemu (#2138081)

- systemd-boot man page: add section for virtual machines (#2138081)

- boot: Only do full driver initialization in VMs (#2138081)

- dissect: rework DISSECT_IMAGE_ADD_PARTITION_DEVICES + DISSECT_IMAGE_OPEN_PARTITION_DEVICES (#2138081)

- ci(Mergify): v252 configuration update (#2138081)

- ci: Run GitHub workflows on rhel branches (#2138081)

- ci: Drop scorecards workflow, not relevant (#2138081)

  

* Fri Dec 02 2022 systemd maintenance team <systemd-maint@redhat.com> - 252-1

- Rebase to systemd v252 + systemd-stable v252.2 (#2138081)

  

* Fri Dec 02 2022 systemd maintenance team <systemd-maint@redhat.com> - 250-13

- build systemd-boot EFI tools (#2140646)

  

[root@rocky14 ~]# dnf update systemd

Last metadata expiration check: 2:08:11 ago on Thu May 22 08:27:07 2025.

Dependencies resolved.

==============================================================================================================================================================================================================

Package                                                                                                  Architecture                                                                Version                                                                                                Repository                                                                      Size

==============================================================================================================================================================================================================

Upgrading:

systemd                                                                                                x86_64                                                                            252-46.el9_5.3                                                                                  baseos                                                                            4.0 M

systemd-libs                                                                                      x86_64                                                                            252-46.el9_5.3                                                                                  baseos                                                                            671 k

systemd-pam                                                                                        x86_64                                                                            252-46.el9_5.3                                                                                  baseos                                                                            278 k

systemd-rpm-macros                                                                          noarch                                                                            252-46.el9_5.3                                                                                  baseos                                                                              66 k

systemd-udev                                                                                      x86_64                                                                            252-46.el9_5.3                                                                                  baseos                                                                            1.9 M

  

Transaction Summary

==============================================================================================================================================================================================================

Upgrade    5 Packages

  

Total download size: 6.9 M

Is this ok [y/N]: y

Downloading Packages:

(1/5): systemd-rpm-macros-252-46.el9_5.3.noarch.rpm                                                                                                                                                                                                                                                      195 kB/s |    66 kB          00:00

(2/5): systemd-pam-252-46.el9_5.3.x86_64.rpm                                                                                                                                                                                                                                                                    566 kB/s | 278 kB          00:00

(3/5): systemd-libs-252-46.el9_5.3.x86_64.rpm                                                                                                                                                                                                                                                                  2.0 MB/s | 671 kB          00:00

(4/5): systemd-udev-252-46.el9_5.3.x86_64.rpm                                                                                                                                                                                                                                                                  2.6 MB/s | 1.9 MB          00:00

(5/5): systemd-252-46.el9_5.3.x86_64.rpm                                                                                                                                                                                                                                                                              11 MB/s | 4.0 MB          00:00

--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

Total                                                                                                                                                                                                                                                                                                                                                  6.9 MB/s | 6.9 MB          00:01

Running transaction check

Transaction check succeeded.

Running transaction test

Transaction test succeeded.

Running transaction

    Preparing                :                                                                                                                                                                                                                                                                                                                                                                            1/1

    Upgrading                : systemd-libs-252-46.el9_5.3.x86_64                                                                                                                                                                                                                                                                                                    1/10

    Running scriptlet: systemd-libs-252-46.el9_5.3.x86_64                                                                                                                                                                                                                                                                                                    1/10

    Upgrading                : systemd-rpm-macros-252-46.el9_5.3.noarch                                                                                                                                                                                                                                                                                        2/10

    Upgrading                : systemd-pam-252-46.el9_5.3.x86_64                                                                                                                                                                                                                                                                                                      3/10

    Running scriptlet: systemd-252-46.el9_5.3.x86_64                                                                                                                                                                                                                                                                                                              4/10

    Upgrading                : systemd-252-46.el9_5.3.x86_64                                                                                                                                                                                                                                                                                                              4/10

    Running scriptlet: systemd-252-46.el9_5.3.x86_64                                                                                                                                                                                                                                                                                                              4/10

    Upgrading                : systemd-udev-252-46.el9_5.3.x86_64                                                                                                                                                                                                                                                                                                    5/10

    Running scriptlet: systemd-udev-252-46.el9_5.3.x86_64                                                                                                                                                                                                                                                                                                    5/10

    Running scriptlet: systemd-udev-252-46.el9_5.2.0.1.x86_64                                                                                                                                                                                                                                                                                            6/10

    Cleanup                    : systemd-udev-252-46.el9_5.2.0.1.x86_64                                                                                                                                                                                                                                                                                            6/10

    Running scriptlet: systemd-udev-252-46.el9_5.2.0.1.x86_64                                                                                                                                                                                                                                                                                            6/10

    Cleanup                    : systemd-pam-252-46.el9_5.2.0.1.x86_64                                                                                                                                                                                                                                                                                              7/10

    Cleanup                    : systemd-252-46.el9_5.2.0.1.x86_64                                                                                                                                                                                                                                                                                                      8/10

    Running scriptlet: systemd-252-46.el9_5.2.0.1.x86_64                                                                                                                                                                                                                                                                                                      8/10

    Cleanup                    : systemd-rpm-macros-252-46.el9_5.2.0.1.noarch                                                                                                                                                                                                                                                                                9/10

    Cleanup                    : systemd-libs-252-46.el9_5.2.0.1.x86_64                                                                                                                                                                                                                                                                                          10/10

    Running scriptlet: systemd-252-46.el9_5.3.x86_64                                                                                                                                                                                                                                                                                                            10/10

    Running scriptlet: systemd-libs-252-46.el9_5.2.0.1.x86_64                                                                                                                                                                                                                                                                                          10/10

    Verifying                : systemd-udev-252-46.el9_5.3.x86_64                                                                                                                                                                                                                                                                                                    1/10

    Verifying                : systemd-udev-252-46.el9_5.2.0.1.x86_64                                                                                                                                                                                                                                                                                            2/10

    Verifying                : systemd-rpm-macros-252-46.el9_5.3.noarch                                                                                                                                                                                                                                                                                        3/10

    Verifying                : systemd-rpm-macros-252-46.el9_5.2.0.1.noarch                                                                                                                                                                                                                                                                                4/10

    Verifying                : systemd-pam-252-46.el9_5.3.x86_64                                                                                                                                                                                                                                                                                                      5/10

    Verifying                : systemd-pam-252-46.el9_5.2.0.1.x86_64                                                                                                                                                                                                                                                                                              6/10

    Verifying                : systemd-libs-252-46.el9_5.3.x86_64                                                                                                                                                                                                                                                                                                    7/10

    Verifying                : systemd-libs-252-46.el9_5.2.0.1.x86_64                                                                                                                                                                                                                                                                                            8/10

    Verifying                : systemd-252-46.el9_5.3.x86_64                                                                                                                                                                                                                                                                                                              9/10

    Verifying                : systemd-252-46.el9_5.2.0.1.x86_64                                                                                                                                                                                                                                                                                                    10/10

  

Upgraded:

    systemd-252-46.el9_5.3.x86_64              systemd-libs-252-46.el9_5.3.x86_64              systemd-pam-252-46.el9_5.3.x86_64              systemd-rpm-macros-252-46.el9_5.3.noarch              systemd-udev-252-46.el9_5.3.x86_64

  

Complete!
```
```bash
[root@rocky14 ~]# rpm -qi crony

package crony is not installed

[root@rocky14 ~]# cat /etc/dnf/dnf.conf

[main]

gpgcheck=1

installonly_limit=3

clean_requirements_on_remove=True

best=True

skip_if_unavailable=False

[root@rocky14 ~]# dnf repolist

repo id                                                                                                                                                repo name

appstream                                                                                                                                            Rocky Linux 9 - AppStream

baseos                                                                                                                                                  Rocky Linux 9 - BaseOS

epel                                                                                                                                                      Extra Packages for Enterprise Linux 9 - x86_64

epel-cisco-openh264                                                                                                                        Extra Packages for Enterprise Linux 9 openh264 (From Cisco) - x86_64

extras                                                                                                                                                  Rocky Linux 9 - Extras

[root@rocky14 ~]# dnf history

ID          | Command line                                                                                                                                                                                                                                                                                        | Date and time        | Action(s)            | Altered

--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

        31 | update systemd                                                                                                                                                                                                                                                                                    | 2025-05-22 10:35 | Upgrade                |        5

        30 | install cronie                                                                                                                                                                                                                                                                                    | 2025-04-30 08:18 | Install                |        3 EE

        29 | update                                                                                                                                                                                                                                                                                                    | 2025-02-10 18:35 | I, U                      |    212 EE

        28 | install iperf3                                                                                                                                                                                                                                                                                    | 2024-11-29 11:45 | Install                |        2

        27 | install podman                                                                                                                                                                                                                                                                                    | 2024-11-07 19:33 | Install                |      18    <

        26 | update                                                                                                                                                                                                                                                                                                    | 2024-11-03 11:39 | I, U                      |      54 >#

        25 | install firewalld                                                                                                                                                                                                                                                                              | 2024-10-19 11:13 | Install                |      17 EE

        24 | install -y nmap                                                                                                                                                                                                                                                                                  | 2024-10-11 16:57 | Install                |        5

        23 | install unzip                                                                                                                                                                                                                                                                                      | 2024-10-08 18:08 | Install                |        1

        22 | install sysstat                                                                                                                                                                                                                                                                                  | 2024-10-07 19:23 | Install                |        5 EE

        21 | install lsof                                                                                                                                                                                                                                                                                        | 2024-09-28 11:26 | Install                |        1

        20 | install selinux-policy-devel                                                                                                                                                                                                                                                        | 2024-09-20 18:12 | Install                |        7

        19 | install policycoreutils-python-utils                                                                                                                                                                                                                                        | 2024-09-20 18:08 | Install                |        7

        18 | install -y audit                                                                                                                                                                                                                                                                                | 2024-09-20 18:08 | Install                |        1 EE

        17 | install -y setools-console                                                                                                                                                                                                                                                            | 2024-09-20 18:08 | Install                |        2

        16 | install man-db                                                                                                                                                                                                                                                                                    | 2024-09-15 18:33 | Install                |        2

        15 | -y install vim                                                                                                                                                                                                                                                                                    | 2024-09-14 15:39 | Install                |        4

        14 | install epel-release                                                                                                                                                                                                                                                                        | 2024-09-14 15:39 | Upgrade                |        1

        13 | install shim grub2                                                                                                                                                                                                                                                                            | 2024-09-07 16:49 | I, U                      |      12

        12 | remove vim                                                                                                                                                                                                                                                                                            | 2024-08-17 10:37 | Removed                |        4

        11 | install vim                                                                                                                                                                                                                                                                                          | 2024-08-16 20:41 | Install                |        4

        10 | install cowsay                                                                                                                                                                                                                                                                                    | 2024-08-16 20:40 | Install                |      60

          9 | install -y ncurses                                                                                                                                                                                                                                                                            | 2024-07-27 10:07 | Install                |        1

          8 | install lvm2                                                                                                                                                                                                                                                                                        | 2024-07-06 18:51 | Install                |        6 EE

          7 | install -y ansible                                                                                                                                                                                                                                                                            | 2024-07-06 09:08 | Install                |      12    <

          6 | install -y epel-release                                                                                                                                                                                                                                                                  | 2024-07-06 09:08 | Install                |        8 >E

          5 | install bind-utils                                                                                                                                                                                                                                                                            | 2024-07-06 08:59 | Install                |        7

          4 | install warewulf-dracut-4.5.5-1.el9.noarch.rpm                                                                                                                                                                                                                    | 2024-07-05 23:05 | Install                |        4

          3 | install shim grub2                                                                                                                                                                                                                                                                            | 2024-07-05 22:16 | Install                |      52 EE

          2 | install -y --allowerasing coreutils cpio dhclient e2fsprogs ethtool findutils initscripts ipmitool iproute kernel-core kernel-modules net-tools Network | 2024-06-07 22:43 | E, I                      |      98 EE

          1 | update -y                                                                                                                                                                                                                                                                                              | 2024-06-07 22:43 | I, U                      |      73 EE

[root@rocky14 ~]# ls /etc/yum.repos.d/

epel-cisco-openh264.repo    epel-testing.repo    epel.repo    rocky-addons.repo    rocky-devel.repo    rocky-extras.repo    rocky.repo

[root@rocky14 ~]# cat /etc/yum.repos.d/rocky.repo

# rocky.repo

#

# The mirrorlist system uses the connecting IP address of the client and the

# update status of each mirror to pick current mirrors that are geographically

# close to the client.    You should use this for Rocky updates unless you are

# manually picking other mirrors.

#

# If the mirrorlist does not work for you, you can try the commented out

# baseurl line instead.

  

[baseos]

name=Rocky Linux $releasever - BaseOS

mirrorlist=https://mirrors.rockylinux.org/mirrorlist?arch=$basearch&repo=BaseOS-$releasever$rltype

#baseurl=http://dl.rockylinux.org/$contentdir/$releasever/BaseOS/$basearch/os/

gpgcheck=1

enabled=1

countme=1

metadata_expire=6h

gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-Rocky-9

  

[baseos-debuginfo]

name=Rocky Linux $releasever - BaseOS - Debug

mirrorlist=https://mirrors.rockylinux.org/mirrorlist?arch=$basearch&repo=BaseOS-$releasever-debug$rltype

#baseurl=http://dl.rockylinux.org/$contentdir/$releasever/BaseOS/$basearch/debug/tree/

gpgcheck=1

enabled=0

metadata_expire=6h

gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-Rocky-9

  

[baseos-source]

name=Rocky Linux $releasever - BaseOS - Source

mirrorlist=https://mirrors.rockylinux.org/mirrorlist?arch=source&repo=BaseOS-$releasever-source$rltype

#baseurl=http://dl.rockylinux.org/$contentdir/$releasever/BaseOS/source/tree/

gpgcheck=1

enabled=0

metadata_expire=6h

gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-Rocky-9

  

[appstream]

name=Rocky Linux $releasever - AppStream

mirrorlist=https://mirrors.rockylinux.org/mirrorlist?arch=$basearch&repo=AppStream-$releasever$rltype

#baseurl=http://dl.rockylinux.org/$contentdir/$releasever/AppStream/$basearch/os/

gpgcheck=1

enabled=1

countme=1

metadata_expire=6h

gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-Rocky-9

  

[appstream-debuginfo]

name=Rocky Linux $releasever - AppStream - Debug

mirrorlist=https://mirrors.rockylinux.org/mirrorlist?arch=$basearch&repo=AppStream-$releasever-debug$rltype

#baseurl=http://dl.rockylinux.org/$contentdir/$releasever/AppStream/$basearch/debug/tree/

gpgcheck=1

enabled=0

metadata_expire=6h

gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-Rocky-9

  

[appstream-source]

name=Rocky Linux $releasever - AppStream - Source

mirrorlist=https://mirrors.rockylinux.org/mirrorlist?arch=source&repo=AppStream-$releasever-source$rltype

#baseurl=http://dl.rockylinux.org/$contentdir/$releasever/AppStream/source/tree/

gpgcheck=1

enabled=0

metadata_expire=6h

gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-Rocky-9

  

[crb]

name=Rocky Linux $releasever - CRB

mirrorlist=https://mirrors.rockylinux.org/mirrorlist?arch=$basearch&repo=CRB-$releasever$rltype

#baseurl=http://dl.rockylinux.org/$contentdir/$releasever/CRB/$basearch/os/

gpgcheck=1

enabled=0

countme=1

metadata_expire=6h

gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-Rocky-9

  

[crb-debuginfo]

name=Rocky Linux $releasever - CRB - Debug

mirrorlist=https://mirrors.rockylinux.org/mirrorlist?arch=$basearch&repo=CRB-$releasever-debug$rltype

#baseurl=http://dl.rockylinux.org/$contentdir/$releasever/CRB/$basearch/debug/tree/

gpgcheck=1

enabled=0

metadata_expire=6h

gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-Rocky-9

  

[crb-source]

name=Rocky Linux $releasever - CRB - Source

mirrorlist=https://mirrors.rockylinux.org/mirrorlist?arch=source&repo=CRB-$releasever-source$rltype

#baseurl=http://dl.rockylinux.org/$contentdir/$releasever/CRB/source/tree/

gpgcheck=1

enabled=0

metadata_expire=6h

gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-Rocky-9

[root@rocky14 ~]# dnf config-manager --disable baseos

[root@rocky14 ~]# cat /etc/yum.repos.d/rocky.repo

# rocky.repo

#

# The mirrorlist system uses the connecting IP address of the client and the

# update status of each mirror to pick current mirrors that are geographically

# close to the client.    You should use this for Rocky updates unless you are

# manually picking other mirrors.

#

# If the mirrorlist does not work for you, you can try the commented out

# baseurl line instead.

  

[baseos]

name=Rocky Linux $releasever - BaseOS

mirrorlist=https://mirrors.rockylinux.org/mirrorlist?arch=$basearch&repo=BaseOS-$releasever$rltype

#baseurl=http://dl.rockylinux.org/$contentdir/$releasever/BaseOS/$basearch/os/

gpgcheck=1

enabled=0

countme=1

metadata_expire=6h

gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-Rocky-9

  

[baseos-debuginfo]

name=Rocky Linux $releasever - BaseOS - Debug

mirrorlist=https://mirrors.rockylinux.org/mirrorlist?arch=$basearch&repo=BaseOS-$releasever-debug$rltype

#baseurl=http://dl.rockylinux.org/$contentdir/$releasever/BaseOS/$basearch/debug/tree/

gpgcheck=1

enabled=0

metadata_expire=6h

gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-Rocky-9

  

[baseos-source]

name=Rocky Linux $releasever - BaseOS - Source

mirrorlist=https://mirrors.rockylinux.org/mirrorlist?arch=source&repo=BaseOS-$releasever-source$rltype

#baseurl=http://dl.rockylinux.org/$contentdir/$releasever/BaseOS/source/tree/

gpgcheck=1

enabled=0

metadata_expire=6h

gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-Rocky-9

  

[appstream]

name=Rocky Linux $releasever - AppStream

mirrorlist=https://mirrors.rockylinux.org/mirrorlist?arch=$basearch&repo=AppStream-$releasever$rltype

#baseurl=http://dl.rockylinux.org/$contentdir/$releasever/AppStream/$basearch/os/

gpgcheck=1

enabled=1

countme=1

metadata_expire=6h

gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-Rocky-9

  

[appstream-debuginfo]

name=Rocky Linux $releasever - AppStream - Debug

mirrorlist=https://mirrors.rockylinux.org/mirrorlist?arch=$basearch&repo=AppStream-$releasever-debug$rltype

#baseurl=http://dl.rockylinux.org/$contentdir/$releasever/AppStream/$basearch/debug/tree/

gpgcheck=1

enabled=0

metadata_expire=6h

gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-Rocky-9

  

[appstream-source]

name=Rocky Linux $releasever - AppStream - Source

mirrorlist=https://mirrors.rockylinux.org/mirrorlist?arch=source&repo=AppStream-$releasever-source$rltype

#baseurl=http://dl.rockylinux.org/$contentdir/$releasever/AppStream/source/tree/

gpgcheck=1

enabled=0

metadata_expire=6h

gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-Rocky-9

  

[crb]

name=Rocky Linux $releasever - CRB

mirrorlist=https://mirrors.rockylinux.org/mirrorlist?arch=$basearch&repo=CRB-$releasever$rltype

#baseurl=http://dl.rockylinux.org/$contentdir/$releasever/CRB/$basearch/os/

gpgcheck=1

enabled=0

countme=1

metadata_expire=6h

gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-Rocky-9

  

[crb-debuginfo]

name=Rocky Linux $releasever - CRB - Debug

mirrorlist=https://mirrors.rockylinux.org/mirrorlist?arch=$basearch&repo=CRB-$releasever-debug$rltype

#baseurl=http://dl.rockylinux.org/$contentdir/$releasever/CRB/$basearch/debug/tree/

gpgcheck=1

enabled=0

metadata_expire=6h

gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-Rocky-9

  

[crb-source]

name=Rocky Linux $releasever - CRB - Source

mirrorlist=https://mirrors.rockylinux.org/mirrorlist?arch=source&repo=CRB-$releasever-source$rltype

#baseurl=http://dl.rockylinux.org/$contentdir/$releasever/CRB/source/tree/

gpgcheck=1

enabled=0

metadata_expire=6h

gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-Rocky-9

[root@rocky14 ~]# dnf config-manager --enable baseos

[root@rocky14 ~]# cat /etc/yum.repos.d/rocky.repo

# rocky.repo

#

# The mirrorlist system uses the connecting IP address of the client and the

# update status of each mirror to pick current mirrors that are geographically

# close to the client.    You should use this for Rocky updates unless you are

# manually picking other mirrors.

#

# If the mirrorlist does not work for you, you can try the commented out

# baseurl line instead.

  

[baseos]

name=Rocky Linux $releasever - BaseOS

mirrorlist=https://mirrors.rockylinux.org/mirrorlist?arch=$basearch&repo=BaseOS-$releasever$rltype

#baseurl=http://dl.rockylinux.org/$contentdir/$releasever/BaseOS/$basearch/os/

gpgcheck=1

enabled=1

countme=1

metadata_expire=6h

gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-Rocky-9

  

[baseos-debuginfo]

name=Rocky Linux $releasever - BaseOS - Debug

mirrorlist=https://mirrors.rockylinux.org/mirrorlist?arch=$basearch&repo=BaseOS-$releasever-debug$rltype

#baseurl=http://dl.rockylinux.org/$contentdir/$releasever/BaseOS/$basearch/debug/tree/

gpgcheck=1

enabled=0

metadata_expire=6h

gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-Rocky-9

  

[baseos-source]

name=Rocky Linux $releasever - BaseOS - Source

mirrorlist=https://mirrors.rockylinux.org/mirrorlist?arch=source&repo=BaseOS-$releasever-source$rltype

#baseurl=http://dl.rockylinux.org/$contentdir/$releasever/BaseOS/source/tree/

gpgcheck=1

enabled=0

metadata_expire=6h

gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-Rocky-9

  

[appstream]

name=Rocky Linux $releasever - AppStream

mirrorlist=https://mirrors.rockylinux.org/mirrorlist?arch=$basearch&repo=AppStream-$releasever$rltype

#baseurl=http://dl.rockylinux.org/$contentdir/$releasever/AppStream/$basearch/os/

gpgcheck=1

enabled=1

countme=1

metadata_expire=6h

gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-Rocky-9

  

[appstream-debuginfo]

name=Rocky Linux $releasever - AppStream - Debug

mirrorlist=https://mirrors.rockylinux.org/mirrorlist?arch=$basearch&repo=AppStream-$releasever-debug$rltype

#baseurl=http://dl.rockylinux.org/$contentdir/$releasever/AppStream/$basearch/debug/tree/

gpgcheck=1

enabled=0

metadata_expire=6h

gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-Rocky-9

  

[appstream-source]

name=Rocky Linux $releasever - AppStream - Source

mirrorlist=https://mirrors.rockylinux.org/mirrorlist?arch=source&repo=AppStream-$releasever-source$rltype

#baseurl=http://dl.rockylinux.org/$contentdir/$releasever/AppStream/source/tree/

gpgcheck=1

enabled=0

metadata_expire=6h

gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-Rocky-9

  

[crb]

name=Rocky Linux $releasever - CRB

mirrorlist=https://mirrors.rockylinux.org/mirrorlist?arch=$basearch&repo=CRB-$releasever$rltype

#baseurl=http://dl.rockylinux.org/$contentdir/$releasever/CRB/$basearch/os/

gpgcheck=1

enabled=0

countme=1

metadata_expire=6h

gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-Rocky-9

  

[crb-debuginfo]

name=Rocky Linux $releasever - CRB - Debug

mirrorlist=https://mirrors.rockylinux.org/mirrorlist?arch=$basearch&repo=CRB-$releasever-debug$rltype

#baseurl=http://dl.rockylinux.org/$contentdir/$releasever/CRB/$basearch/debug/tree/

gpgcheck=1

enabled=0

metadata_expire=6h

gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-Rocky-9

  

[crb-source]

name=Rocky Linux $releasever - CRB - Source

mirrorlist=https://mirrors.rockylinux.org/mirrorlist?arch=source&repo=CRB-$releasever-source$rltype

#baseurl=http://dl.rockylinux.org/$contentdir/$releasever/CRB/source/tree/

gpgcheck=1

enabled=0

metadata_expire=6h

gpgkey=file:///etc/pki/rpm-gpg/RPM-GPG-KEY-Rocky-9
```
```bash
[root@rocky14 ~]# rpm -qa mariadb

[root@rocky14 ~]# dnf search mariadb

Last metadata expiration check: 2:30:38 ago on Thu May 22 08:27:07 2025.

======================================================================================= Name Exactly Matched: mariadb ========================================================================================

mariadb.x86_64 : A very fast and robust SQL database server

====================================================================================== Name & Summary Matched: mariadb =======================================================================================

mariadb-connector-c.x86_64 : The MariaDB Native Client library (C driver)

mariadb-connector-c.i686 : The MariaDB Native Client library (C driver)

mariadb-connector-c-devel.x86_64 : Development files for mariadb-connector-c

mariadb-connector-c-devel.i686 : Development files for mariadb-connector-c

mariadb-connector-odbc.x86_64 : The MariaDB Native Client library (ODBC driver)

mariadb-embedded.x86_64 : MariaDB as an embeddable library

mariadb-java-client.noarch : Connects applications developed in Java to MariaDB and MySQL databases

mariadb-oqgraph-engine.x86_64 : The Open Query GRAPH engine for MariaDB

mariadb-pam.x86_64 : PAM authentication plugin for the MariaDB server

mariadb-server.x86_64 : The MariaDB server and related files

mariadb-server-utils.x86_64 : Non-essential server utilities for MariaDB/MySQL applications

perl-DBD-MariaDB.x86_64 : MariaDB and MySQL driver for the Perl5 Database Interface (DBI)

=========================================================================================== Name Matched: mariadb ============================================================================================

mariadb-backup.x86_64 : The mariabackup tool for physical online backups

mariadb-common.x86_64 : The shared files required by server and client

mariadb-connector-c-config.noarch : Configuration files for packages that use /etc/my.cnf as a configuration file

mariadb-errmsg.x86_64 : The error messages files required by server and embedded

mariadb-gssapi-server.x86_64 : GSSAPI authentication plugin for server

mariadb-server-galera.x86_64 : The configuration files and scripts for galera replication

========================================================================================== Summary Matched: mariadb ==========================================================================================

anope-mysql.x86_64 : MariaDB/MySQL modules for Anope IRC services

mysql-selinux.noarch : SELinux policy modules for MySQL and MariaDB packages

phpMyAdmin.noarch : A web interface for MySQL and MariaDB

python3-asyncmy.x86_64 : A fast asyncio MySQL/MariaDB driver

python3-mysqlclient.x86_64 : MySQL/mariaDB database connector for Python

[root@rocky14 ~]# dnf search all mariadb

Last metadata expiration check: 2:30:50 ago on Thu May 22 08:27:07 2025.

================================================================================= Name & Description & URL Matched: mariadb ==================================================================================

mariadb.x86_64 : A very fast and robust SQL database server

============================================================================ Name & Summary & Description & URL Matched: mariadb =============================================================================

mariadb-connector-c.x86_64 : The MariaDB Native Client library (C driver)

mariadb-connector-c.i686 : The MariaDB Native Client library (C driver)

mariadb-connector-c-devel.x86_64 : Development files for mariadb-connector-c

mariadb-connector-c-devel.i686 : Development files for mariadb-connector-c

mariadb-connector-odbc.x86_64 : The MariaDB Native Client library (ODBC driver)

mariadb-embedded.x86_64 : MariaDB as an embeddable library

mariadb-java-client.noarch : Connects applications developed in Java to MariaDB and MySQL databases

mariadb-oqgraph-engine.x86_64 : The Open Query GRAPH engine for MariaDB

mariadb-pam.x86_64 : PAM authentication plugin for the MariaDB server

mariadb-server.x86_64 : The MariaDB server and related files

mariadb-server-utils.x86_64 : Non-essential server utilities for MariaDB/MySQL applications

perl-DBD-MariaDB.x86_64 : MariaDB and MySQL driver for the Perl5 Database Interface (DBI)

================================================================================= Name & Description & URL Matched: mariadb ==================================================================================

mariadb-backup.x86_64 : The mariabackup tool for physical online backups

mariadb-common.x86_64 : The shared files required by server and client

mariadb-errmsg.x86_64 : The error messages files required by server and embedded

mariadb-gssapi-server.x86_64 : GSSAPI authentication plugin for server

mariadb-server-galera.x86_64 : The configuration files and scripts for galera replication

======================================================================================== Name & URL Matched: mariadb =========================================================================================

mariadb-connector-c-config.noarch : Configuration files for packages that use /etc/my.cnf as a configuration file

=================================================================================== Summary & Description Matched: mariadb ===================================================================================

anope-mysql.x86_64 : MariaDB/MySQL modules for Anope IRC services

mysql-selinux.noarch : SELinux policy modules for MySQL and MariaDB packages

python3-asyncmy.x86_64 : A fast asyncio MySQL/MariaDB driver

========================================================================================== Summary Matched: mariadb ==========================================================================================

phpMyAdmin.noarch : A web interface for MySQL and MariaDB

python3-mysqlclient.x86_64 : MySQL/mariaDB database connector for Python

======================================================================================== Description Matched: mariadb ========================================================================================

holland-mariabackup.noarch : Holland plugin for Mariabackup

libdbi-dbd-mysql.x86_64 : MySQL plugin for libdbi

nextcloud-mysql.noarch : MySQL database support for NextCloud

proxysql.x86_64 : A high-performance MySQL proxy

unixODBC.x86_64 : A complete ODBC driver manager for Linux

unixODBC.i686 : A complete ODBC driver manager for Linux

[root@rocky14 ~]# dnf install mariadb

Rocky Linux 9 - BaseOS                                                                                                                                                                                                                                                                                                                  15 kB/s | 4.1 kB          00:00

Rocky Linux 9 - AppStream                                                                                                                                                                                                                                                                                                            11 kB/s | 4.5 kB          00:00

Dependencies resolved.

==============================================================================================================================================================================================================

Package                                                                                                          Architecture                                                        Version                                                                                                  Repository                                                                    Size

==============================================================================================================================================================================================================

Installing:

mariadb                                                                                                        x86_64                                                                    3:10.5.27-1.el9_5.0.1                                                                      appstream                                                                    1.6 M

Installing dependencies:

mariadb-common                                                                                          x86_64                                                                    3:10.5.27-1.el9_5.0.1                                                                      appstream                                                                      27 k

mariadb-connector-c                                                                                x86_64                                                                    3.2.6-1.el9_0                                                                                      appstream                                                                    195 k

mariadb-connector-c-config                                                                  noarch                                                                    3.2.6-1.el9_0                                                                                      appstream                                                                    9.8 k

perl-Sys-Hostname                                                                                    x86_64                                                                    1.23-481.el9                                                                                        appstream                                                                      16 k

  

Transaction Summary

==============================================================================================================================================================================================================

Install    5 Packages

  

Total download size: 1.8 M

Installed size: 19 M

Is this ok [y/N]: n

Operation aborted.

[root@rocky14 ~]# dnf -y install mariadb

Last metadata expiration check: 0:02:06 ago on Thu May 22 11:03:19 2025.

Dependencies resolved.

==============================================================================================================================================================================================================

Package                                                                                                          Architecture                                                        Version                                                                                                  Repository                                                                    Size

==============================================================================================================================================================================================================

Installing:

mariadb                                                                                                        x86_64                                                                    3:10.5.27-1.el9_5.0.1                                                                      appstream                                                                    1.6 M

Installing dependencies:

mariadb-common                                                                                          x86_64                                                                    3:10.5.27-1.el9_5.0.1                                                                      appstream                                                                      27 k

mariadb-connector-c                                                                                x86_64                                                                    3.2.6-1.el9_0                                                                                      appstream                                                                    195 k

mariadb-connector-c-config                                                                  noarch                                                                    3.2.6-1.el9_0                                                                                      appstream                                                                    9.8 k

perl-Sys-Hostname                                                                                    x86_64                                                                    1.23-481.el9                                                                                        appstream                                                                      16 k

  

Transaction Summary

==============================================================================================================================================================================================================

Install    5 Packages

  

Total download size: 1.8 M

Installed size: 19 M

Downloading Packages:

(1/5): mariadb-connector-c-config-3.2.6-1.el9_0.noarch.rpm                                                                                                                                                                                                                                          29 kB/s | 9.8 kB          00:00

(2/5): perl-Sys-Hostname-1.23-481.el9.x86_64.rpm                                                                                                                                                                                                                                                              38 kB/s |    16 kB          00:00

(3/5): mariadb-connector-c-3.2.6-1.el9_0.x86_64.rpm                                                                                                                                                                                                                                                      309 kB/s | 195 kB          00:00

(4/5): mariadb-common-10.5.27-1.el9_5.0.1.x86_64.rpm                                                                                                                                                                                                                                                      88 kB/s |    27 kB          00:00

(5/5): mariadb-10.5.27-1.el9_5.0.1.x86_64.rpm                                                                                                                                                                                                                                                                  3.2 MB/s | 1.6 MB          00:00

--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

Total                                                                                                                                                                                                                                                                                                                                                  1.7 MB/s | 1.8 MB          00:01

Running transaction check

Transaction check succeeded.

Running transaction test

Transaction test succeeded.

Running transaction

    Preparing                :                                                                                                                                                                                                                                                                                                                                                                            1/1

    Installing              : mariadb-connector-c-config-3.2.6-1.el9_0.noarch                                                                                                                                                                                                                                                                            1/5

    Installing              : mariadb-connector-c-3.2.6-1.el9_0.x86_64                                                                                                                                                                                                                                                                                          2/5

    Installing              : mariadb-common-3:10.5.27-1.el9_5.0.1.x86_64                                                                                                                                                                                                                                                                                    3/5

    Installing              : perl-Sys-Hostname-1.23-481.el9.x86_64                                                                                                                                                                                                                                                                                                4/5

    Installing              : mariadb-3:10.5.27-1.el9_5.0.1.x86_64                                                                                                                                                                                                                                                                                                  5/5

    Running scriptlet: mariadb-3:10.5.27-1.el9_5.0.1.x86_64                                                                                                                                                                                                                                                                                                  5/5

    Verifying                : mariadb-connector-c-3.2.6-1.el9_0.x86_64                                                                                                                                                                                                                                                                                          1/5

    Verifying                : mariadb-connector-c-config-3.2.6-1.el9_0.noarch                                                                                                                                                                                                                                                                            2/5

    Verifying                : perl-Sys-Hostname-1.23-481.el9.x86_64                                                                                                                                                                                                                                                                                                3/5

    Verifying                : mariadb-common-3:10.5.27-1.el9_5.0.1.x86_64                                                                                                                                                                                                                                                                                    4/5

    Verifying                : mariadb-3:10.5.27-1.el9_5.0.1.x86_64                                                                                                                                                                                                                                                                                                  5/5

  

Installed:

    mariadb-3:10.5.27-1.el9_5.0.1.x86_64                    mariadb-common-3:10.5.27-1.el9_5.0.1.x86_64                  mariadb-connector-c-3.2.6-1.el9_0.x86_64                  mariadb-connector-c-config-3.2.6-1.el9_0.noarch

    perl-Sys-Hostname-1.23-481.el9.x86_64

  

Complete!

[root@rocky14 ~]# dnf remove mariadb

Dependencies resolved.

==============================================================================================================================================================================================================

Package                                                                                                          Architecture                                                        Version                                                                                                Repository                                                                      Size

==============================================================================================================================================================================================================

Removing:

mariadb                                                                                                        x86_64                                                                    3:10.5.27-1.el9_5.0.1                                                                    @appstream                                                                      18 M

Removing unused dependencies:

mariadb-common                                                                                          x86_64                                                                    3:10.5.27-1.el9_5.0.1                                                                    @appstream                                                                    179 k

mariadb-connector-c                                                                                x86_64                                                                    3.2.6-1.el9_0                                                                                    @appstream                                                                    540 k

mariadb-connector-c-config                                                                  noarch                                                                    3.2.6-1.el9_0                                                                                    @appstream                                                                    497

perl-Sys-Hostname                                                                                    x86_64                                                                    1.23-481.el9                                                                                      @appstream                                                                      21 k

  

Transaction Summary

==============================================================================================================================================================================================================

Remove    5 Packages

  

Freed space: 19 M

Is this ok [y/N]:

Operation aborted.

[root@rocky14 ~]# dnf -y remove mariadb

Dependencies resolved.

==============================================================================================================================================================================================================

Package                                                                                                          Architecture                                                        Version                                                                                                Repository                                                                      Size

==============================================================================================================================================================================================================

Removing:

mariadb                                                                                                        x86_64                                                                    3:10.5.27-1.el9_5.0.1                                                                    @appstream                                                                      18 M

Removing unused dependencies:

mariadb-common                                                                                          x86_64                                                                    3:10.5.27-1.el9_5.0.1                                                                    @appstream                                                                    179 k

mariadb-connector-c                                                                                x86_64                                                                    3.2.6-1.el9_0                                                                                    @appstream                                                                    540 k

mariadb-connector-c-config                                                                  noarch                                                                    3.2.6-1.el9_0                                                                                    @appstream                                                                    497

perl-Sys-Hostname                                                                                    x86_64                                                                    1.23-481.el9                                                                                      @appstream                                                                      21 k

  

Transaction Summary

==============================================================================================================================================================================================================

Remove    5 Packages

  

Freed space: 19 M

Running transaction check

Transaction check succeeded.

Running transaction test

Transaction test succeeded.

Running transaction

    Preparing                :                                                                                                                                                                                                                                                                                                                                                                            1/1

    Erasing                    : mariadb-3:10.5.27-1.el9_5.0.1.x86_64                                                                                                                                                                                                                                                                                                  1/5

    Erasing                    : mariadb-common-3:10.5.27-1.el9_5.0.1.x86_64                                                                                                                                                                                                                                                                                    2/5

    Erasing                    : mariadb-connector-c-3.2.6-1.el9_0.x86_64                                                                                                                                                                                                                                                                                          3/5

    Erasing                    : mariadb-connector-c-config-3.2.6-1.el9_0.noarch                                                                                                                                                                                                                                                                            4/5

    Erasing                    : perl-Sys-Hostname-1.23-481.el9.x86_64                                                                                                                                                                                                                                                                                                5/5

    Running scriptlet: perl-Sys-Hostname-1.23-481.el9.x86_64                                                                                                                                                                                                                                                                                                5/5

    Verifying                : mariadb-3:10.5.27-1.el9_5.0.1.x86_64                                                                                                                                                                                                                                                                                                  1/5

    Verifying                : mariadb-common-3:10.5.27-1.el9_5.0.1.x86_64                                                                                                                                                                                                                                                                                    2/5

    Verifying                : mariadb-connector-c-3.2.6-1.el9_0.x86_64                                                                                                                                                                                                                                                                                          3/5

    Verifying                : mariadb-connector-c-config-3.2.6-1.el9_0.noarch                                                                                                                                                                                                                                                                            4/5

    Verifying                : perl-Sys-Hostname-1.23-481.el9.x86_64                                                                                                                                                                                                                                                                                                5/5

  

Removed:

    mariadb-3:10.5.27-1.el9_5.0.1.x86_64                    mariadb-common-3:10.5.27-1.el9_5.0.1.x86_64                  mariadb-connector-c-3.2.6-1.el9_0.x86_64                  mariadb-connector-c-config-3.2.6-1.el9_0.noarch

    perl-Sys-Hostname-1.23-481.el9.x86_64

  

Complete!

[root@rocky14 ~]# rpm -q    mariadb-common

package mariadb-common is not installed

[root@rocky14 ~]# rpm -qi    mariadb-common

package mariadb-common is not installed

[root@rocky14 ~]# dnf whatprovides iostat

Last metadata expiration check: 0:03:54 ago on Thu May 22 11:03:19 2025.

sysstat-12.5.4-9.el9.x86_64 : Collection of performance monitoring tools for Linux

Repo                : @System

Matched from:

Filename        : /usr/bin/iostat

  

sysstat-12.5.4-9.el9.x86_64 : Collection of performance monitoring tools for Linux

Repo                : appstream

Matched from:

Filename        : /usr/bin/iostat

  

[root@rocky14 ~]# dnf whatprovides sar

Last metadata expiration check: 0:04:14 ago on Thu May 22 11:03:19 2025.

sysstat-12.5.4-9.el9.x86_64 : Collection of performance monitoring tools for Linux

Repo                : @System

Matched from:

Filename        : /usr/bin/sar

  

sysstat-12.5.4-9.el9.x86_64 : Collection of performance monitoring tools for Linux

Repo                : appstream

Matched from:

Filename        : /usr/bin/sar

  

[root@rocky14 ~]# dnf whatprovides systemd

  

Last metadata expiration check: 0:04:30 ago on Thu May 22 11:03:19 2025.

systemd-252-46.el9_5.3.i686 : System and Service Manager

Repo                : baseos

Matched from:

Provide        : systemd = 252-46.el9_5.3

  

systemd-252-46.el9_5.3.x86_64 : System and Service Manager

Repo                : @System

Matched from:

Provide        : systemd = 252-46.el9_5.3

  

systemd-252-46.el9_5.3.x86_64 : System and Service Manager

Repo                : baseos

Matched from:

Provide        : systemd = 252-46.el9_5.3

  

[root@rocky14 ~]#

[root@rocky14 ~]# dnf whatprovides ls

Last metadata expiration check: 0:04:41 ago on Thu May 22 11:03:19 2025.

coreutils-8.32-36.el9.x86_64 : A set of basic GNU tools commonly used in shell scripts

Repo                : @System

Matched from:

Filename        : /usr/bin/ls

  

coreutils-8.32-36.el9.x86_64 : A set of basic GNU tools commonly used in shell scripts

Repo                : baseos

Matched from:

Filename        : /usr/bin/ls

  

coreutils-single-8.32-36.el9.x86_64 : coreutils multicall binary

Repo                : baseos

Matched from:

Filename        : /usr/bin/ls

  

[root@rocky14 ~]# dnf whatprovides python

Last metadata expiration check: 0:04:53 ago on Thu May 22 11:03:19 2025.

python-unversioned-command-3.9.21-1.el9_5.noarch : The "python" command that runs Python 3

Repo                : appstream

Matched from:

Provide        : python = 3.9.21-1.el9_5

  

[root@rocky14 ~]# dnf update

Last metadata expiration check: 0:05:49 ago on Thu May 22 11:03:19 2025.

Dependencies resolved.

==============================================================================================================================================================================================================

Package                                                                                                Architecture                                                      Version                                                                                                                Repository                                                                  Size

==============================================================================================================================================================================================================

Installing:

kernel-core                                                                                      x86_64                                                                  5.14.0-503.40.1.el9_5                                                                                    baseos                                                                          18 M

kernel-modules                                                                                x86_64                                                                  5.14.0-503.40.1.el9_5                                                                                    baseos                                                                          36 M

Upgrading:

NetworkManager                                                                                x86_64                                                                  1:1.48.10-8.el9_5                                                                                            baseos                                                                        2.3 M

NetworkManager-libnm                                                                    x86_64                                                                  1:1.48.10-8.el9_5                                                                                            baseos                                                                        1.8 M

bind-libs                                                                                          x86_64                                                                  32:9.16.23-24.el9_5.3                                                                                    appstream                                                                  1.2 M

bind-license                                                                                    noarch                                                                  32:9.16.23-24.el9_5.3                                                                                    appstream                                                                    12 k

bind-utils                                                                                        x86_64                                                                  32:9.16.23-24.el9_5.3                                                                                    appstream                                                                  201 k

dracut                                                                                                x86_64                                                                  057-80.git20250411.el9_5                                                                              baseos                                                                        376 k

dracut-network                                                                                x86_64                                                                  057-80.git20250411.el9_5                                                                              baseos                                                                          68 k

e2fsprogs                                                                                          x86_64                                                                  1.46.5-6.el9_5                                                                                                  baseos                                                                        1.0 M

e2fsprogs-libs                                                                                x86_64                                                                  1.46.5-6.el9_5                                                                                                  baseos                                                                        221 k

epel-release                                                                                    noarch                                                                  9-10.el9                                                                                                              epel                                                                              19 k

expat                                                                                                  x86_64                                                                  2.5.0-3.el9_5.3                                                                                                baseos                                                                        115 k

freetype                                                                                            x86_64                                                                  2.10.4-10.el9_5                                                                                                baseos                                                                        386 k

glibc                                                                                                  x86_64                                                                  2.34-125.el9_5.8                                                                                              baseos                                                                        1.9 M

glibc-common                                                                                    x86_64                                                                  2.34-125.el9_5.8                                                                                              baseos                                                                        290 k

glibc-minimal-langpack                                                                x86_64                                                                  2.34-125.el9_5.8                                                                                              baseos                                                                          16 k

grub2-common                                                                                    noarch                                                                  1:2.06-94.el9_5                                                                                                baseos                                                                        903 k

grub2-pc                                                                                            x86_64                                                                  1:2.06-94.el9_5                                                                                                baseos                                                                          12 k

grub2-pc-modules                                                                            noarch                                                                  1:2.06-94.el9_5                                                                                                baseos                                                                        909 k

grub2-tools                                                                                      x86_64                                                                  1:2.06-94.el9_5                                                                                                baseos                                                                        1.8 M

grub2-tools-efi                                                                              x86_64                                                                  1:2.06-94.el9_5                                                                                                baseos                                                                        539 k

grub2-tools-extra                                                                          x86_64                                                                  1:2.06-94.el9_5                                                                                                baseos                                                                        840 k

grub2-tools-minimal                                                                      x86_64                                                                  1:2.06-94.el9_5                                                                                                baseos                                                                        603 k

libcom_err                                                                                        x86_64                                                                  1.46.5-6.el9_5                                                                                                  baseos                                                                          25 k

libgcc                                                                                                x86_64                                                                  11.5.0-5.el9_5                                                                                                  baseos                                                                          84 k

libgomp                                                                                              x86_64                                                                  11.5.0-5.el9_5                                                                                                  baseos                                                                        260 k

libnfsidmap                                                                                      x86_64                                                                  1:2.5.4-27.el9_5.1                                                                                          baseos                                                                          59 k

libss                                                                                                  x86_64                                                                  1.46.5-6.el9_5                                                                                                  baseos                                                                          31 k

libstdc++                                                                                          x86_64                                                                  11.5.0-5.el9_5                                                                                                  baseos                                                                        731 k

libxml2                                                                                              x86_64                                                                  2.9.13-6.el9_5.2                                                                                              baseos                                                                        746 k

linux-firmware                                                                                noarch                                                                  20250415-146.5.el9_5                                                                                      baseos                                                                        475 M

linux-firmware-whence                                                                  noarch                                                                  20250415-146.5.el9_5                                                                                      baseos                                                                        112 k

mdadm                                                                                                  x86_64                                                                  4.3-4.el9_5                                                                                                        baseos                                                                        435 k

nfs-utils                                                                                          x86_64                                                                  1:2.5.4-27.el9_5.1                                                                                          baseos                                                                        430 k

openssl                                                                                              x86_64                                                                  1:3.2.2-6.el9_5.1                                                                                            baseos                                                                        1.3 M

openssl-libs                                                                                    x86_64                                                                  1:3.2.2-6.el9_5.1                                                                                            baseos                                                                        2.4 M

passt                                                                                                  x86_64                                                                  0^20240806.gee36266-7.el9_5                                                                        appstream                                                                  193 k

passt-selinux                                                                                  noarch                                                                  0^20240806.gee36266-7.el9_5                                                                        appstream                                                                    27 k

pciutils                                                                                            x86_64                                                                  3.7.0-5.el9_5.1                                                                                                baseos                                                                          91 k

pciutils-libs                                                                                  x86_64                                                                  3.7.0-5.el9_5.1                                                                                                baseos                                                                          40 k

podman                                                                                                x86_64                                                                  4:5.2.2-16.el9_5                                                                                              appstream                                                                    16 M

rocky-gpg-keys                                                                                noarch                                                                  9.5-1.3.el9                                                                                                        baseos                                                                          12 k

rocky-release                                                                                  noarch                                                                  9.5-1.3.el9                                                                                                        baseos                                                                          22 k

rocky-repos                                                                                      noarch                                                                  9.5-1.3.el9                                                                                                        baseos                                                                          12 k

tzdata                                                                                                noarch                                                                  2025b-1.el9                                                                                                        baseos                                                                        430 k

unzip                                                                                                  x86_64                                                                  6.0-58.el9_5                                                                                                      baseos                                                                        180 k

Installing dependencies:

kernel-modules-core                                                                      x86_64                                                                  5.14.0-503.40.1.el9_5                                                                                    baseos                                                                          30 M

Removing:

kernel-core                                                                                      x86_64                                                                  5.14.0-427.18.1.el9_4                                                                                    @baseos                                                                        64 M

kernel-modules                                                                                x86_64                                                                  5.14.0-427.18.1.el9_4                                                                                    @baseos                                                                        33 M

kernel-modules-core                                                                      x86_64                                                                  5.14.0-427.18.1.el9_4                                                                                    @baseos                                                                        27 M

  

Transaction Summary

==============================================================================================================================================================================================================

Install      3 Packages

Upgrade    45 Packages

Remove        3 Packages

  

Total download size: 599 M

Is this ok [y/N]:

Operation aborted.

[root@rocky14 ~]# df -h /var/cache/dnf

Filesystem            Size    Used Avail Use% Mounted on

tmpfs                      8.0G    2.0G    6.1G    25% /

[root@rocky14 ~]# dnf update --exclude=kernel

Last metadata expiration check: 0:06:35 ago on Thu May 22 11:03:19 2025.

Dependencies resolved.

==============================================================================================================================================================================================================

Package                                                                                                Architecture                                                      Version                                                                                                                Repository                                                                  Size

==============================================================================================================================================================================================================

Installing:

kernel-core                                                                                      x86_64                                                                  5.14.0-503.40.1.el9_5                                                                                    baseos                                                                          18 M

kernel-modules                                                                                x86_64                                                                  5.14.0-503.40.1.el9_5                                                                                    baseos                                                                          36 M

Upgrading:

NetworkManager                                                                                x86_64                                                                  1:1.48.10-8.el9_5                                                                                            baseos                                                                        2.3 M

NetworkManager-libnm                                                                    x86_64                                                                  1:1.48.10-8.el9_5                                                                                            baseos                                                                        1.8 M

bind-libs                                                                                          x86_64                                                                  32:9.16.23-24.el9_5.3                                                                                    appstream                                                                  1.2 M

bind-license                                                                                    noarch                                                                  32:9.16.23-24.el9_5.3                                                                                    appstream                                                                    12 k

bind-utils                                                                                        x86_64                                                                  32:9.16.23-24.el9_5.3                                                                                    appstream                                                                  201 k

dracut                                                                                                x86_64                                                                  057-80.git20250411.el9_5                                                                              baseos                                                                        376 k

dracut-network                                                                                x86_64                                                                  057-80.git20250411.el9_5                                                                              baseos                                                                          68 k

e2fsprogs                                                                                          x86_64                                                                  1.46.5-6.el9_5                                                                                                  baseos                                                                        1.0 M

e2fsprogs-libs                                                                                x86_64                                                                  1.46.5-6.el9_5                                                                                                  baseos                                                                        221 k

epel-release                                                                                    noarch                                                                  9-10.el9                                                                                                              epel                                                                              19 k

expat                                                                                                  x86_64                                                                  2.5.0-3.el9_5.3                                                                                                baseos                                                                        115 k

freetype                                                                                            x86_64                                                                  2.10.4-10.el9_5                                                                                                baseos                                                                        386 k

glibc                                                                                                  x86_64                                                                  2.34-125.el9_5.8                                                                                              baseos                                                                        1.9 M

glibc-common                                                                                    x86_64                                                                  2.34-125.el9_5.8                                                                                              baseos                                                                        290 k

glibc-minimal-langpack                                                                x86_64                                                                  2.34-125.el9_5.8                                                                                              baseos                                                                          16 k

grub2-common                                                                                    noarch                                                                  1:2.06-94.el9_5                                                                                                baseos                                                                        903 k

grub2-pc                                                                                            x86_64                                                                  1:2.06-94.el9_5                                                                                                baseos                                                                          12 k

grub2-pc-modules                                                                            noarch                                                                  1:2.06-94.el9_5                                                                                                baseos                                                                        909 k

grub2-tools                                                                                      x86_64                                                                  1:2.06-94.el9_5                                                                                                baseos                                                                        1.8 M

grub2-tools-efi                                                                              x86_64                                                                  1:2.06-94.el9_5                                                                                                baseos                                                                        539 k

grub2-tools-extra                                                                          x86_64                                                                  1:2.06-94.el9_5                                                                                                baseos                                                                        840 k

grub2-tools-minimal                                                                      x86_64                                                                  1:2.06-94.el9_5                                                                                                baseos                                                                        603 k

libcom_err                                                                                        x86_64                                                                  1.46.5-6.el9_5                                                                                                  baseos                                                                          25 k

libgcc                                                                                                x86_64                                                                  11.5.0-5.el9_5                                                                                                  baseos                                                                          84 k

libgomp                                                                                              x86_64                                                                  11.5.0-5.el9_5                                                                                                  baseos                                                                        260 k

libnfsidmap                                                                                      x86_64                                                                  1:2.5.4-27.el9_5.1                                                                                          baseos                                                                          59 k

libss                                                                                                  x86_64                                                                  1.46.5-6.el9_5                                                                                                  baseos                                                                          31 k

libstdc++                                                                                          x86_64                                                                  11.5.0-5.el9_5                                                                                                  baseos                                                                        731 k

libxml2                                                                                              x86_64                                                                  2.9.13-6.el9_5.2                                                                                              baseos                                                                        746 k

linux-firmware                                                                                noarch                                                                  20250415-146.5.el9_5                                                                                      baseos                                                                        475 M

linux-firmware-whence                                                                  noarch                                                                  20250415-146.5.el9_5                                                                                      baseos                                                                        112 k

mdadm                                                                                                  x86_64                                                                  4.3-4.el9_5                                                                                                        baseos                                                                        435 k

nfs-utils                                                                                          x86_64                                                                  1:2.5.4-27.el9_5.1                                                                                          baseos                                                                        430 k

openssl                                                                                              x86_64                                                                  1:3.2.2-6.el9_5.1                                                                                            baseos                                                                        1.3 M

openssl-libs                                                                                    x86_64                                                                  1:3.2.2-6.el9_5.1                                                                                            baseos                                                                        2.4 M

passt                                                                                                  x86_64                                                                  0^20240806.gee36266-7.el9_5                                                                        appstream                                                                  193 k

passt-selinux                                                                                  noarch                                                                  0^20240806.gee36266-7.el9_5                                                                        appstream                                                                    27 k

pciutils                                                                                            x86_64                                                                  3.7.0-5.el9_5.1                                                                                                baseos                                                                          91 k

pciutils-libs                                                                                  x86_64                                                                  3.7.0-5.el9_5.1                                                                                                baseos                                                                          40 k

podman                                                                                                x86_64                                                                  4:5.2.2-16.el9_5                                                                                              appstream                                                                    16 M

rocky-gpg-keys                                                                                noarch                                                                  9.5-1.3.el9                                                                                                        baseos                                                                          12 k

rocky-release                                                                                  noarch                                                                  9.5-1.3.el9                                                                                                        baseos                                                                          22 k

rocky-repos                                                                                      noarch                                                                  9.5-1.3.el9                                                                                                        baseos                                                                          12 k

tzdata                                                                                                noarch                                                                  2025b-1.el9                                                                                                        baseos                                                                        430 k

unzip                                                                                                  x86_64                                                                  6.0-58.el9_5                                                                                                      baseos                                                                        180 k

Installing dependencies:

kernel-modules-core                                                                      x86_64                                                                  5.14.0-503.40.1.el9_5                                                                                    baseos                                                                          30 M

Removing:

kernel-core                                                                                      x86_64                                                                  5.14.0-427.18.1.el9_4                                                                                    @baseos                                                                        64 M

kernel-modules                                                                                x86_64                                                                  5.14.0-427.18.1.el9_4                                                                                    @baseos                                                                        33 M

kernel-modules-core                                                                      x86_64                                                                  5.14.0-427.18.1.el9_4                                                                                    @baseos                                                                        27 M

  

Transaction Summary

==============================================================================================================================================================================================================

Install      3 Packages

Upgrade    45 Packages

Remove        3 Packages

  

Total download size: 599 M

Is this ok [y/N]:

Operation aborted.

[root@rocky14 ~]# dnf grouplist

Last metadata expiration check: 0:08:24 ago on Thu May 22 11:03:19 2025.

Available Environment Groups:

      Server with GUI

      Server

      Minimal Install

      Workstation

      KDE Plasma Workspaces

      Custom Operating System

      Virtualization Host

Available Groups:

      Fedora Packager

      VideoLAN Client

      Xfce

      Legacy UNIX Compatibility

      Console Internet Tools

      Container Management

      Development Tools

      .NET Development

      Graphical Administration Tools

      Headless Management

      Network Servers

      RPM Development Tools

      Scientific Support

      Security Tools

      Smart Card Support

      System Tools

[root@rocky14 ~]# dnf group install development

Last metadata expiration check: 0:08:38 ago on Thu May 22 11:03:19 2025.

Dependencies resolved.

==============================================================================================================================================================================================================

Package                                                                                                                        Architecture                                            Version                                                                                                            Repository                                                        Size

==============================================================================================================================================================================================================

Upgrading:

glibc                                                                                                                          x86_64                                                        2.34-125.el9_5.8                                                                                          baseos                                                              1.9 M

glibc-common                                                                                                            x86_64                                                        2.34-125.el9_5.8                                                                                          baseos                                                              290 k

glibc-minimal-langpack                                                                                        x86_64                                                        2.34-125.el9_5.8                                                                                          baseos                                                                16 k

libgcc                                                                                                                        x86_64                                                        11.5.0-5.el9_5                                                                                              baseos                                                                84 k

libgomp                                                                                                                      x86_64                                                        11.5.0-5.el9_5                                                                                              baseos                                                              260 k

libstdc++                                                                                                                  x86_64                                                        11.5.0-5.el9_5                                                                                              baseos                                                              731 k

Installing group/module packages:

asciidoc                                                                                                                    noarch                                                        9.1.0-3.el9                                                                                                    appstream                                                        238 k

autoconf                                                                                                                    noarch                                                        2.69-39.el9                                                                                                    appstream                                                        665 k

automake                                                                                                                    noarch                                                        1.16.2-8.el9                                                                                                  appstream                                                        662 k

bison                                                                                                                          x86_64                                                        3.7.4-5.el9                                                                                                    appstream                                                        921 k

byacc                                                                                                                          x86_64                                                        2.0.20210109-4.el9                                                                                      appstream                                                          88 k

diffstat                                                                                                                    x86_64                                                        1.64-6.el9                                                                                                      appstream                                                          43 k

flex                                                                                                                            x86_64                                                        2.6.4-9.el9                                                                                                    appstream                                                        308 k

gcc                                                                                                                              x86_64                                                        11.5.0-5.el9_5                                                                                              appstream                                                          32 M

gcc-c++                                                                                                                      x86_64                                                        11.5.0-5.el9_5                                                                                              appstream                                                          13 M

gdb                                                                                                                              x86_64                                                        14.2-3.el9                                                                                                      appstream                                                        146 k

git                                                                                                                              x86_64                                                        2.43.5-2.el9_5                                                                                              appstream                                                          50 k

glibc-devel                                                                                                              x86_64                                                        2.34-125.el9_5.8                                                                                          appstream                                                          25 k

intltool                                                                                                                    noarch                                                        0.51.0-20.el9                                                                                                appstream                                                          55 k

jna                                                                                                                              x86_64                                                        5.6.0-8.el9                                                                                                    appstream                                                        268 k

libtool                                                                                                                      x86_64                                                        2.4.6-46.el9                                                                                                  appstream                                                        577 k

ltrace                                                                                                                        x86_64                                                        0.7.91-43.el9                                                                                                appstream                                                        137 k

patchutils                                                                                                                x86_64                                                        0.4.2-7.el9                                                                                                    appstream                                                          99 k

perl-Fedora-VSP                                                                                                      noarch                                                        0.001-23.el9                                                                                                  appstream                                                          23 k

perl-generators                                                                                                      noarch                                                        1.11-12.el9                                                                                                    appstream                                                          16 k

pesign                                                                                                                        x86_64                                                        115-6.el9_1.rocky.2                                                                                    appstream                                                        171 k

pkgconf                                                                                                                      x86_64                                                        1.7.3-10.el9                                                                                                  baseos                                                                40 k

pkgconf-m4                                                                                                                noarch                                                        1.7.3-10.el9                                                                                                  baseos                                                                14 k

pkgconf-pkg-config                                                                                                x86_64                                                        1.7.3-10.el9                                                                                                  baseos                                                                10 k

redhat-rpm-config                                                                                                  noarch                                                        208-1.el9                                                                                                        appstream                                                          66 k

rpm-build                                                                                                                  x86_64                                                        4.16.1.3-34.el9.0.1                                                                                    appstream                                                          59 k

rpm-sign                                                                                                                    x86_64                                                        4.16.1.3-34.el9.0.1                                                                                    baseos                                                                17 k

source-highlight                                                                                                    x86_64                                                        3.1.9-12.el9                                                                                                  appstream                                                        608 k

systemtap                                                                                                                  x86_64                                                        5.1-4.el9_5                                                                                                    appstream                                                        8.3 k

valgrind                                                                                                                    x86_64                                                        1:3.23.0-4.el9                                                                                              appstream                                                        4.7 M

valgrind-devel                                                                                                        x86_64                                                        1:3.23.0-4.el9                                                                                              appstream                                                          46 k

Installing dependencies:

ModemManager-glib                                                                                                  x86_64                                                        1.20.2-1.el9                                                                                                  baseos                                                              334 k

adobe-mappings-cmap                                                                                              noarch                                                        20171205-12.el9                                                                                            appstream                                                        1.9 M

adobe-mappings-cmap-deprecated                                                                        noarch                                                        20171205-12.el9                                                                                            appstream                                                        113 k

adobe-mappings-pdf                                                                                                noarch                                                        20180407-10.el9                                                                                            appstream                                                        627 k

adobe-source-code-pro-fonts                                                                              noarch                                                        2.030.1.050-12.el9.1                                                                                  baseos                                                              831 k

adwaita-cursor-theme                                                                                            noarch                                                        40.1.1-3.el9                                                                                                  appstream                                                        623 k

adwaita-icon-theme                                                                                                noarch                                                        40.1.1-3.el9                                                                                                  appstream                                                          11 M

alsa-lib                                                                                                                    x86_64                                                        1.2.12-1.el9                                                                                                  appstream                                                        504 k

annobin                                                                                                                      x86_64                                                        12.65-1.el9                                                                                                    appstream                                                        1.0 M

at-spi2-atk                                                                                                              x86_64                                                        2.38.0-4.el9                                                                                                  appstream                                                          86 k

at-spi2-core                                                                                                            x86_64                                                        2.40.3-1.el9                                                                                                  appstream                                                        176 k

atk                                                                                                                              x86_64                                                        2.36.0-5.el9                                                                                                  appstream                                                        270 k

avahi-glib                                                                                                                x86_64                                                        0.8-21.el9                                                                                                      appstream                                                          14 k

bluez-libs                                                                                                                x86_64                                                        5.72-2.el9                                                                                                      baseos                                                                81 k

boost-filesystem                                                                                                    x86_64                                                        1.75.0-8.el9                                                                                                  appstream                                                          57 k

boost-regex                                                                                                              x86_64                                                        1.75.0-8.el9                                                                                                  appstream                                                        277 k

boost-system                                                                                                            x86_64                                                        1.75.0-8.el9                                                                                                  appstream                                                          13 k

boost-thread                                                                                                            x86_64                                                        1.75.0-8.el9                                                                                                  appstream                                                          55 k

bubblewrap                                                                                                                x86_64                                                        0.4.1-8.el9_5                                                                                                baseos                                                                49 k

bzip2                                                                                                                          x86_64                                                        1.0.8-10.el9_5                                                                                              baseos                                                                51 k

cairo                                                                                                                          x86_64                                                        1.17.4-7.el9                                                                                                  appstream                                                        659 k

cairo-gobject                                                                                                          x86_64                                                        1.17.4-7.el9                                                                                                  appstream                                                          18 k

colord-libs                                                                                                              x86_64                                                        1.4.5-4.el9                                                                                                    appstream                                                        230 k

composefs-libs                                                                                                        x86_64                                                        1.0.5-1.el9                                                                                                    appstream                                                          60 k

copy-jdk-configs                                                                                                    noarch                                                        4.0-3.el9                                                                                                        appstream                                                          27 k

cpp                                                                                                                              x86_64                                                        11.5.0-5.el9_5                                                                                              appstream                                                          11 M

cups-libs                                                                                                                  x86_64                                                        1:2.3.3op2-31.el9_5                                                                                    baseos                                                              262 k

debugedit                                                                                                                  x86_64                                                        5.0-5.el9                                                                                                        appstream                                                          76 k

dejavu-sans-fonts                                                                                                  noarch                                                        2.37-18.el9                                                                                                    baseos                                                              1.3 M

docbook-dtds                                                                                                            noarch                                                        1.0-79.el9                                                                                                      appstream                                                        282 k

docbook-style-xsl                                                                                                  noarch                                                        1.79.2-16.el9                                                                                                appstream                                                        1.2 M

dwz                                                                                                                              x86_64                                                        0.14-3.el9                                                                                                      appstream                                                        127 k

dyninst                                                                                                                      x86_64                                                        12.1.0-1.el9                                                                                                  appstream                                                        3.8 M

ed                                                                                                                                x86_64                                                        1.14.2-12.el9                                                                                                baseos                                                                74 k

efi-srpm-macros                                                                                                      noarch                                                        6-2.el9_0                                                                                                        appstream                                                          22 k

elfutils                                                                                                                    x86_64                                                        0.191-4.el9                                                                                                    baseos                                                              550 k

elfutils-devel                                                                                                        x86_64                                                        0.191-4.el9                                                                                                    appstream                                                          48 k

elfutils-libelf-devel                                                                                          x86_64                                                        0.191-4.el9                                                                                                    appstream                                                          21 k

emacs-filesystem                                                                                                    noarch                                                        1:27.2-11.el9_5.2                                                                                        appstream                                                        7.7 k

exempi                                                                                                                        x86_64                                                        2.6.0-0.2.20211007gite23c213.el9                                                          appstream                                                        523 k

exiv2-libs                                                                                                                x86_64                                                        0.27.5-2.el9                                                                                                  appstream                                                        779 k

fdk-aac-free                                                                                                            x86_64                                                        2.0.0-8.el9                                                                                                    appstream                                                        324 k

flac-libs                                                                                                                  x86_64                                                        1.3.3-10.el9_2.1                                                                                          appstream                                                        217 k

flatpak-selinux                                                                                                      noarch                                                        1.12.9-3.el9_5                                                                                              appstream                                                          21 k

flatpak-session-helper                                                                                        x86_64                                                        1.12.9-3.el9_5                                                                                              appstream                                                          72 k

fontconfig                                                                                                                x86_64                                                        2.14.0-2.el9_1                                                                                              appstream                                                        274 k

fonts-filesystem                                                                                                    noarch                                                        1:2.0.5-7.el9.1                                                                                            baseos                                                              9.0 k

fonts-srpm-macros                                                                                                  noarch                                                        1:2.0.5-7.el9.1                                                                                            appstream                                                          27 k

fribidi                                                                                                                      x86_64                                                        1.0.10-6.el9.2                                                                                              appstream                                                          84 k

fuse                                                                                                                            x86_64                                                        2.9.9-16.el9                                                                                                  baseos                                                                78 k

gcc-plugin-annobin                                                                                                x86_64                                                        11.5.0-5.el9_5                                                                                              appstream                                                          39 k

gd                                                                                                                                x86_64                                                        2.3.2-3.el9                                                                                                    appstream                                                        131 k

gdb-headless                                                                                                            x86_64                                                        14.2-3.el9                                                                                                      appstream                                                        4.8 M

gdk-pixbuf2                                                                                                              x86_64                                                        2.42.6-4.el9_4                                                                                              appstream                                                        466 k

gdk-pixbuf2-modules                                                                                              x86_64                                                        2.42.6-4.el9_4                                                                                              appstream                                                          85 k

geoclue2                                                                                                                    x86_64                                                        2.6.0-7.el9                                                                                                    appstream                                                        122 k

gettext-common-devel                                                                                            noarch                                                        0.21-8.el9                                                                                                      appstream                                                        405 k

gettext-devel                                                                                                          x86_64                                                        0.21-8.el9                                                                                                      appstream                                                        199 k

ghc-srpm-macros                                                                                                      noarch                                                        1.5.0-6.el9                                                                                                    appstream                                                        7.8 k

giflib                                                                                                                        x86_64                                                        5.2.1-9.el9                                                                                                    appstream                                                          48 k

git-core-doc                                                                                                            noarch                                                        2.43.5-2.el9_5                                                                                              appstream                                                        2.7 M

glib-networking                                                                                                      x86_64                                                        2.68.3-3.el9                                                                                                  baseos                                                              169 k

glibc-gconv-extra                                                                                                  x86_64                                                        2.34-125.el9_5.8                                                                                          baseos                                                              1.6 M

glibc-headers                                                                                                          x86_64                                                        2.34-125.el9_5.8                                                                                          appstream                                                        429 k

go-srpm-macros                                                                                                        noarch                                                        3.6.0-3.el9                                                                                                    appstream                                                          26 k

google-droid-sans-fonts                                                                                      noarch                                                        20200215-11.el9.2                                                                                        appstream                                                        2.7 M

graphene                                                                                                                    x86_64                                                        1.10.6-2.el9                                                                                                  appstream                                                          64 k

graphviz                                                                                                                    x86_64                                                        2.44.0-26.el9                                                                                                appstream                                                        3.3 M

gsettings-desktop-schemas                                                                                  x86_64                                                        40.0-6.el9                                                                                                      baseos                                                              667 k

gsm                                                                                                                              x86_64                                                        1.0.19-6.el9                                                                                                  appstream                                                          33 k

gstreamer1                                                                                                                x86_64                                                        1.22.1-2.el9                                                                                                  appstream                                                        1.4 M

gstreamer1-plugins-base                                                                                      x86_64                                                        1.22.1-3.el9_5                                                                                              appstream                                                        2.2 M

gtk-update-icon-cache                                                                                          x86_64                                                        3.24.31-5.el9                                                                                                appstream                                                          32 k

gtk2                                                                                                                            x86_64                                                        2.24.33-8.el9                                                                                                appstream                                                        3.5 M

gtk3                                                                                                                            x86_64                                                        3.24.31-5.el9                                                                                                appstream                                                        4.8 M

hicolor-icon-theme                                                                                                noarch                                                        0.17-13.el9                                                                                                    appstream                                                          66 k

info                                                                                                                            x86_64                                                        6.7-15.el9                                                                                                      baseos                                                              224 k

iso-codes                                                                                                                  noarch                                                        4.6.0-3.el9                                                                                                    appstream                                                        3.3 M

java-1.8.0-openjdk-headless                                                                              x86_64                                                        1:1.8.0.452.b09-2.el9                                                                                appstream                                                          33 M

javapackages-filesystem                                                                                      noarch                                                        6.0.0-7.el9_5                                                                                                appstream                                                        9.9 k

jbig2dec-libs                                                                                                          x86_64                                                        0.19-7.el9                                                                                                      appstream                                                          72 k

jbigkit-libs                                                                                                            x86_64                                                        2.1-23.el9                                                                                                      appstream                                                          52 k

kernel-headers                                                                                                        x86_64                                                        5.14.0-503.40.1.el9_5                                                                                appstream                                                        3.5 M

kernel-srpm-macros                                                                                                noarch                                                        1.0-13.el9                                                                                                      appstream                                                          15 k

langpacks-core-font-en                                                                                        noarch                                                        3.0-16.el9                                                                                                      appstream                                                        9.5 k

lcms2                                                                                                                          x86_64                                                        2.12-3.el9                                                                                                      appstream                                                        166 k

libICE                                                                                                                        x86_64                                                        1.0.10-8.el9                                                                                                  appstream                                                          70 k

libSM                                                                                                                          x86_64                                                        1.2.3-10.el9                                                                                                  appstream                                                          41 k

libX11                                                                                                                        x86_64                                                        1.7.0-9.el9                                                                                                    appstream                                                        650 k

libX11-common                                                                                                          noarch                                                        1.7.0-9.el9                                                                                                    appstream                                                        151 k

libX11-xcb                                                                                                                x86_64                                                        1.7.0-9.el9                                                                                                    appstream                                                          10 k

libXau                                                                                                                        x86_64                                                        1.0.9-8.el9                                                                                                    appstream                                                          30 k

libXaw                                                                                                                        x86_64                                                        1.0.13-19.el9                                                                                                appstream                                                        197 k

libXcomposite                                                                                                          x86_64                                                        0.4.5-7.el9                                                                                                    appstream                                                          23 k

libXcursor                                                                                                                x86_64                                                        1.2.0-7.el9                                                                                                    appstream                                                          30 k

libXdamage                                                                                                                x86_64                                                        1.1.5-7.el9                                                                                                    appstream                                                          22 k

libXext                                                                                                                      x86_64                                                        1.3.4-8.el9                                                                                                    appstream                                                          39 k

libXfixes                                                                                                                  x86_64                                                        5.0.3-16.el9                                                                                                  appstream                                                          19 k

libXft                                                                                                                        x86_64                                                        2.3.3-8.el9                                                                                                    appstream                                                          61 k

libXi                                                                                                                          x86_64                                                        1.7.10-8.el9                                                                                                  appstream                                                          39 k

libXinerama                                                                                                              x86_64                                                        1.1.4-10.el9                                                                                                  appstream                                                          14 k

libXmu                                                                                                                        x86_64                                                        1.1.3-8.el9                                                                                                    appstream                                                          74 k

libXpm                                                                                                                        x86_64                                                        3.5.13-10.el9                                                                                                appstream                                                          58 k

libXrandr                                                                                                                  x86_64                                                        1.5.2-8.el9                                                                                                    appstream                                                          27 k

libXrender                                                                                                                x86_64                                                        0.9.10-16.el9                                                                                                appstream                                                          27 k

libXt                                                                                                                          x86_64                                                        1.2.0-6.el9                                                                                                    appstream                                                        180 k

libXtst                                                                                                                      x86_64                                                        1.2.3-16.el9                                                                                                  appstream                                                          20 k

libXv                                                                                                                          x86_64                                                        1.0.11-16.el9                                                                                                appstream                                                          18 k

libXxf86vm                                                                                                                x86_64                                                        1.1.4-18.el9                                                                                                  appstream                                                          18 k

libappstream-glib                                                                                                  x86_64                                                        0.7.18-5.el9_4                                                                                              appstream                                                        386 k

libasyncns                                                                                                                x86_64                                                        0.8-22.el9                                                                                                      appstream                                                          29 k

libatomic                                                                                                                  x86_64                                                        11.5.0-5.el9_5                                                                                              baseos                                                                25 k

libbabeltrace                                                                                                          x86_64                                                        1.5.8-10.el9                                                                                                  appstream                                                        186 k

libcanberra                                                                                                              x86_64                                                        0.30-27.el9                                                                                                    appstream                                                          85 k

libcanberra-gtk3                                                                                                    x86_64                                                        0.30-27.el9                                                                                                    appstream                                                          31 k

libdatrie                                                                                                                  x86_64                                                        0.2.13-4.el9                                                                                                  appstream                                                          32 k

libdrm                                                                                                                        x86_64                                                        2.4.121-1.el9                                                                                                appstream                                                        158 k

libepoxy                                                                                                                    x86_64                                                        1.5.5-4.el9                                                                                                    appstream                                                        244 k

libexif                                                                                                                      x86_64                                                        0.6.22-6.el9                                                                                                  appstream                                                        423 k

libfontenc                                                                                                                x86_64                                                        1.1.3-17.el9                                                                                                  appstream                                                          30 k

libgexiv2                                                                                                                  x86_64                                                        0.12.3-1.el9                                                                                                  appstream                                                          81 k

libglvnd                                                                                                                    x86_64                                                        1:1.3.4-1.el9                                                                                                appstream                                                        133 k

libglvnd-egl                                                                                                            x86_64                                                        1:1.3.4-1.el9                                                                                                appstream                                                          36 k

libglvnd-glx                                                                                                            x86_64                                                        1:1.3.4-1.el9                                                                                                appstream                                                        140 k

libgs                                                                                                                          x86_64                                                        9.54.0-17.el9_4                                                                                            appstream                                                        3.1 M

libgsf                                                                                                                        x86_64                                                        1.14.47-5.el9                                                                                                appstream                                                        245 k

libgxps                                                                                                                      x86_64                                                        0.3.2-3.el9                                                                                                    appstream                                                          78 k

libicu                                                                                                                        x86_64                                                        67.1-9.el9                                                                                                      baseos                                                              9.6 M

libijs                                                                                                                        x86_64                                                        0.35-15.el9                                                                                                    appstream                                                          29 k

libipt                                                                                                                        x86_64                                                        2.0.4-5.el9                                                                                                    appstream                                                          55 k

libiptcdata                                                                                                              x86_64                                                        1.0.5-10.el9                                                                                                  appstream                                                          60 k

libjpeg-turbo                                                                                                          x86_64                                                        2.0.90-7.el9                                                                                                  appstream                                                        174 k

libldac                                                                                                                      x86_64                                                        2.0.2.3-10.el9                                                                                              appstream                                                          40 k

libmpc                                                                                                                        x86_64                                                        1.2.1-4.el9                                                                                                    appstream                                                          61 k

libnotify                                                                                                                  x86_64                                                        0.7.9-8.el9                                                                                                    appstream                                                          43 k

libogg                                                                                                                        x86_64                                                        2:1.3.4-6.el9                                                                                                appstream                                                          32 k

libosinfo                                                                                                                  x86_64                                                        1.10.0-1.el9                                                                                                  appstream                                                        312 k

libpaper                                                                                                                    x86_64                                                        1.1.28-4.el9                                                                                                  appstream                                                          41 k

libpciaccess                                                                                                            x86_64                                                        0.16-7.el9                                                                                                      baseos                                                                26 k

libpkgconf                                                                                                                x86_64                                                        1.7.3-10.el9                                                                                                  baseos                                                                35 k

libproxy                                                                                                                    x86_64                                                        0.4.15-35.el9                                                                                                baseos                                                                73 k

librsvg2                                                                                                                    x86_64                                                        2.50.7-3.el9                                                                                                  appstream                                                        2.8 M

libsbc                                                                                                                        x86_64                                                        1.4-9.el9                                                                                                        appstream                                                          44 k

libsndfile                                                                                                                x86_64                                                        1.0.31-8.el9_5.2                                                                                          appstream                                                        206 k

libsoup                                                                                                                      x86_64                                                        2.72.0-8.el9_5.3                                                                                          appstream                                                        388 k

libstdc++-devel                                                                                                      x86_64                                                        11.5.0-5.el9_5                                                                                              appstream                                                        2.2 M

libstemmer                                                                                                                x86_64                                                        0-18.585svn.el9                                                                                            appstream                                                          83 k

libtdb                                                                                                                        x86_64                                                        1.4.10-1.el9                                                                                                  baseos                                                                50 k

libthai                                                                                                                      x86_64                                                        0.1.28-8.el9                                                                                                  appstream                                                        208 k

libtheora                                                                                                                  x86_64                                                        1:1.1.1-31.el9                                                                                              appstream                                                        163 k

libtiff                                                                                                                      x86_64                                                        4.4.0-13.el9                                                                                                  appstream                                                        197 k

libtool-ltdl                                                                                                            x86_64                                                        2.4.6-46.el9                                                                                                  appstream                                                          35 k

libtracker-sparql                                                                                                  x86_64                                                        3.1.2-3.el9_1                                                                                                appstream                                                        316 k

libvisual                                                                                                                  x86_64                                                        1:0.4.0-34.el9                                                                                              appstream                                                        143 k

libvorbis                                                                                                                  x86_64                                                        1:1.3.7-5.el9                                                                                                appstream                                                        192 k

libwayland-client                                                                                                  x86_64                                                        1.21.0-1.el9                                                                                                  appstream                                                          33 k

libwayland-cursor                                                                                                  x86_64                                                        1.21.0-1.el9                                                                                                  appstream                                                          18 k

libwayland-egl                                                                                                        x86_64                                                        1.21.0-1.el9                                                                                                  appstream                                                          12 k

libwayland-server                                                                                                  x86_64                                                        1.21.0-1.el9                                                                                                  appstream                                                          41 k

libwebp                                                                                                                      x86_64                                                        1.2.0-8.el9                                                                                                    appstream                                                        276 k

libxcb                                                                                                                        x86_64                                                        1.13.1-9.el9                                                                                                  appstream                                                        224 k

libxcrypt-devel                                                                                                      x86_64                                                        4.4.18-3.el9                                                                                                  appstream                                                          28 k

libxkbcommon                                                                                                            x86_64                                                        1.0.3-4.el9                                                                                                    appstream                                                        132 k

libxshmfence                                                                                                            x86_64                                                        1.3-10.el9                                                                                                      appstream                                                          12 k

libxslt                                                                                                                      x86_64                                                        1.1.34-9.el9_5.3                                                                                          appstream                                                        239 k

libzstd-devel                                                                                                          x86_64                                                        1.5.1-2.el9                                                                                                    appstream                                                          46 k

llvm-libs                                                                                                                  x86_64                                                        18.1.8-3.el9                                                                                                  appstream                                                          26 M

low-memory-monitor                                                                                                x86_64                                                        2.1-4.el9                                                                                                        appstream                                                          35 k

lua                                                                                                                              x86_64                                                        5.4.4-4.el9                                                                                                    appstream                                                        187 k

lua-posix                                                                                                                  x86_64                                                        35.0-8.el9                                                                                                      appstream                                                        131 k

lua-srpm-macros                                                                                                      noarch                                                        1-6.el9                                                                                                            appstream                                                        8.5 k

mesa-filesystem                                                                                                      x86_64                                                        24.1.2-3.el9                                                                                                  appstream                                                          10 k

mesa-libEGL                                                                                                              x86_64                                                        24.1.2-3.el9                                                                                                  appstream                                                        138 k

mesa-libGL                                                                                                                x86_64                                                        24.1.2-3.el9                                                                                                  appstream                                                        169 k

mesa-libgbm                                                                                                              x86_64                                                        24.1.2-3.el9                                                                                                  appstream                                                          35 k

mesa-libglapi                                                                                                          x86_64                                                        24.1.2-3.el9                                                                                                  appstream                                                          44 k

mkfontscale                                                                                                              x86_64                                                        1.2.1-3.el9                                                                                                    appstream                                                          31 k

nss-tools                                                                                                                  x86_64                                                        3.101.0-10.el9_5                                                                                          appstream                                                        435 k

ocaml-srpm-macros                                                                                                  noarch                                                        6-6.el9                                                                                                            appstream                                                        7.8 k

openblas-srpm-macros                                                                                            noarch                                                        2-11.el9                                                                                                          appstream                                                        7.3 k

openjpeg2                                                                                                                  x86_64                                                        2.4.0-7.el9                                                                                                    appstream                                                        162 k

opus                                                                                                                            x86_64                                                        1.3.1-10.el9                                                                                                  appstream                                                        199 k

orc                                                                                                                              x86_64                                                        0.4.31-8.el9                                                                                                  appstream                                                        182 k

osinfo-db                                                                                                                  noarch                                                        20240701-2.el9                                                                                              appstream                                                        289 k

osinfo-db-tools                                                                                                      x86_64                                                        1.10.0-1.el9                                                                                                  appstream                                                          68 k

ostree-libs                                                                                                              x86_64                                                        2024.9-1.el9_5                                                                                              appstream                                                        467 k

pango                                                                                                                          x86_64                                                        1.48.7-3.el9                                                                                                  appstream                                                        297 k

patch                                                                                                                          x86_64                                                        2.7.6-16.el9                                                                                                  appstream                                                        127 k

perl-DynaLoader                                                                                                      x86_64                                                        1.47-481.el9                                                                                                  appstream                                                          24 k

perl-Error                                                                                                                noarch                                                        1:0.17029-7.el9                                                                                            appstream                                                          41 k

perl-File-Compare                                                                                                  noarch                                                        1.100.600-481.el9                                                                                        appstream                                                          12 k

perl-File-Copy                                                                                                        noarch                                                        2.34-481.el9                                                                                                  appstream                                                          19 k

perl-Git                                                                                                                    noarch                                                        2.43.5-2.el9_5                                                                                              appstream                                                          37 k

perl-TermReadKey                                                                                                    x86_64                                                        2.38-11.el9                                                                                                    appstream                                                          36 k

perl-Thread-Queue                                                                                                  noarch                                                        3.14-460.el9                                                                                                  appstream                                                          21 k

perl-XML-Parser                                                                                                      x86_64                                                        2.46-9.el9                                                                                                      appstream                                                        230 k

perl-lib                                                                                                                    x86_64                                                        0.65-481.el9                                                                                                  appstream                                                          13 k

perl-locale                                                                                                              noarch                                                        1.09-481.el9                                                                                                  appstream                                                          12 k

perl-macros                                                                                                              noarch                                                        4:5.32.1-481.el9                                                                                          appstream                                                        9.3 k

perl-srpm-macros                                                                                                    noarch                                                        1-41.el9                                                                                                          appstream                                                        8.2 k

perl-threads                                                                                                            x86_64                                                        1:2.25-460.el9                                                                                              appstream                                                          57 k

perl-threads-shared                                                                                              x86_64                                                        1.61-460.el9.0.1                                                                                          appstream                                                          44 k

pipewire-jack-audio-connection-kit-libs                                                      x86_64                                                        1.0.1-1.el9                                                                                                    appstream                                                        134 k

pipewire-libs                                                                                                          x86_64                                                        1.0.1-1.el9                                                                                                    appstream                                                        1.9 M

pixman                                                                                                                        x86_64                                                        0.40.0-6.el9_3                                                                                              appstream                                                        269 k

poppler                                                                                                                      x86_64                                                        21.01.0-21.el9                                                                                              appstream                                                        1.1 M

poppler-data                                                                                                            noarch                                                        0.4.9-9.el9.0.1                                                                                            appstream                                                        1.8 M

poppler-glib                                                                                                            x86_64                                                        21.01.0-21.el9                                                                                              appstream                                                        151 k

pulseaudio-libs                                                                                                      x86_64                                                        15.0-2.el9                                                                                                      appstream                                                        666 k

pyproject-srpm-macros                                                                                          noarch                                                        1.12.0-1.el9                                                                                                  appstream                                                          13 k

python-srpm-macros                                                                                                noarch                                                        3.9-54.el9                                                                                                      appstream                                                          17 k

qt5-srpm-macros                                                                                                      noarch                                                        5.15.9-1.el9                                                                                                  appstream                                                        7.9 k

rtkit                                                                                                                          x86_64                                                        0.11-29.el9                                                                                                    appstream                                                          55 k

rust-srpm-macros                                                                                                    noarch                                                        17-4.el9                                                                                                          appstream                                                        9.3 k

sgml-common                                                                                                              noarch                                                        0.6.3-58.el9                                                                                                  appstream                                                          54 k

sound-theme-freedesktop                                                                                      noarch                                                        0.8-17.el9                                                                                                      appstream                                                        377 k

systemtap-client                                                                                                    x86_64                                                        5.1-4.el9_5                                                                                                    appstream                                                        3.6 M

systemtap-devel                                                                                                      x86_64                                                        5.1-4.el9_5                                                                                                    appstream                                                        2.2 M

systemtap-runtime                                                                                                  x86_64                                                        5.1-4.el9_5                                                                                                    appstream                                                        441 k

tbb                                                                                                                              x86_64                                                        2020.3-8.el9_5.1                                                                                          appstream                                                        168 k

totem-pl-parser                                                                                                      x86_64                                                        3.26.6-2.el9                                                                                                  appstream                                                        130 k

tracker                                                                                                                      x86_64                                                        3.1.2-3.el9_1                                                                                                appstream                                                        538 k

tzdata-java                                                                                                              noarch                                                        2025b-1.el9                                                                                                    appstream                                                        145 k

upower                                                                                                                        x86_64                                                        0.99.13-2.el9                                                                                                appstream                                                        165 k

urw-base35-bookman-fonts                                                                                    noarch                                                        20200910-6.el9                                                                                              appstream                                                        847 k

urw-base35-c059-fonts                                                                                          noarch                                                        20200910-6.el9                                                                                              appstream                                                        874 k

urw-base35-d050000l-fonts                                                                                  noarch                                                        20200910-6.el9                                                                                              appstream                                                          76 k

urw-base35-fonts                                                                                                    noarch                                                        20200910-6.el9                                                                                              appstream                                                        9.9 k

urw-base35-fonts-common                                                                                      noarch                                                        20200910-6.el9                                                                                              appstream                                                          21 k

urw-base35-gothic-fonts                                                                                      noarch                                                        20200910-6.el9                                                                                              appstream                                                        643 k

urw-base35-nimbus-mono-ps-fonts                                                                      noarch                                                        20200910-6.el9                                                                                              appstream                                                        795 k

urw-base35-nimbus-roman-fonts                                                                          noarch                                                        20200910-6.el9                                                                                              appstream                                                        856 k

urw-base35-nimbus-sans-fonts                                                                            noarch                                                        20200910-6.el9                                                                                              appstream                                                        1.3 M

urw-base35-p052-fonts                                                                                          noarch                                                        20200910-6.el9                                                                                              appstream                                                        973 k

urw-base35-standard-symbols-ps-fonts                                                            noarch                                                        20200910-6.el9                                                                                              appstream                                                          41 k

urw-base35-z003-fonts                                                                                          noarch                                                        20200910-6.el9                                                                                              appstream                                                        275 k

webkit2gtk3-jsc                                                                                                      x86_64                                                        2.48.1-1.el9_5                                                                                              appstream                                                        4.7 M

webrtc-audio-processing                                                                                      x86_64                                                        0.3.1-8.el9.0.1                                                                                            appstream                                                        303 k

wireplumber                                                                                                              x86_64                                                        0.4.14-1.el9.0.1                                                                                          appstream                                                          83 k

wireplumber-libs                                                                                                    x86_64                                                        0.4.14-1.el9.0.1                                                                                          appstream                                                        338 k

xdg-dbus-proxy                                                                                                        x86_64                                                        0.1.3-1.el9                                                                                                    appstream                                                          41 k

xdg-desktop-portal                                                                                                x86_64                                                        1.12.6-1.el9                                                                                                  appstream                                                        367 k

xkeyboard-config                                                                                                    noarch                                                        2.33-2.el9                                                                                                      appstream                                                        779 k

xml-common                                                                                                                noarch                                                        0.6.3-58.el9                                                                                                  appstream                                                          31 k

xorg-x11-fonts-ISO8859-1-100dpi                                                                      noarch                                                        7.5-33.el9                                                                                                      appstream                                                        1.0 M

xz-devel                                                                                                                    x86_64                                                        5.2.5-8.el9_0                                                                                                appstream                                                          52 k

zip                                                                                                                              x86_64                                                        3.0-35.el9                                                                                                      baseos                                                              263 k

zlib-devel                                                                                                                x86_64                                                        1.2.11-40.el9                                                                                                appstream                                                          44 k

zstd                                                                                                                            x86_64                                                        1.5.1-2.el9                                                                                                    baseos                                                              546 k

Installing weak dependencies:

abattis-cantarell-fonts                                                                                      noarch                                                        0.301-4.el9                                                                                                    appstream                                                        364 k

dconf                                                                                                                          x86_64                                                        0.40.0-6.el9                                                                                                  appstream                                                        109 k

exiv2                                                                                                                          x86_64                                                        0.27.5-2.el9                                                                                                  appstream                                                        975 k

flatpak                                                                                                                      x86_64                                                        1.12.9-3.el9_5                                                                                              appstream                                                        1.7 M

libcanberra-gtk2                                                                                                    x86_64                                                        0.30-27.el9                                                                                                    appstream                                                          25 k

libproxy-webkitgtk4                                                                                              x86_64                                                        0.4.15-35.el9                                                                                                appstream                                                          21 k

mesa-dri-drivers                                                                                                    x86_64                                                        24.1.2-3.el9                                                                                                  appstream                                                        8.8 M

p11-kit-server                                                                                                        x86_64                                                        0.25.3-3.el9_5                                                                                              appstream                                                        244 k

perl-version                                                                                                            x86_64                                                        7:0.99.28-4.el9                                                                                            appstream                                                          62 k

pipewire                                                                                                                    x86_64                                                        1.0.1-1.el9                                                                                                    appstream                                                        101 k

pipewire-alsa                                                                                                          x86_64                                                        1.0.1-1.el9                                                                                                    appstream                                                          56 k

pipewire-jack-audio-connection-kit                                                                x86_64                                                        1.0.1-1.el9                                                                                                    appstream                                                        8.1 k

pipewire-pulseaudio                                                                                              x86_64                                                        1.0.1-1.el9                                                                                                    appstream                                                        185 k

tracker-miners                                                                                                        x86_64                                                        3.1.2-4.el9_3                                                                                                appstream                                                        888 k

xdg-desktop-portal-gtk                                                                                        x86_64                                                        1.12.0-3.el9                                                                                                  appstream                                                        130 k

Installing Groups:

Development Tools

  

Transaction Summary

==============================================================================================================================================================================================================

Install    294 Packages

Upgrade        6 Packages

  

Total download size: 265 M

Is this ok [y/N]:

Operation aborted.
```