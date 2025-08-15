```bash
ls -l fruits.txt
-rw-r--r-- 1 root root 0 Aug 14 19:36 fruits.txt
```
```bash
rm -rf fruits.txt
```
```bash
ls -l fruits.txt
ls: cannot access 'fruits.txt': No such file or directory
```

```bash
echo “grapes 5” > fruits.txt
cat fruits.txt
echo “apples 3” > fruits.txt
cat fruits.txt

echo “ “ > fruits.txt

echo “grapes 5” >> fruits.txt
cat fruits.txt
echo “apples 3” >> fruits.txt
cat fruits.txt
```
```bash
“grapes 5”
“apples 3”
“ “
“grapes 5”
“ “
“grapes 5”
“apples 3”
```
```bash
ls
backupfile.txt  fruits.txt  somefile.txt  warewulf-dracut-4.6.2-1.el9.noarch.rpm
```
```bash
cat backupfile.txt
grapes 5
apples 7
oranges 3
bananas 2
pears 6
pineapples 9
```
```bash
mv somefile.txt fruits.txt
mv: overwrite 'fruits.txt'? y
ls
backupfile.txt  fruits.txt  warewulf-dracut-4.6.2-1.el9.noarch.rpm
cat fruits.txt
grapes 5
apples 7
oranges 3
bananas 2
pears 6
pineapples 9
```
```bash
cat fruits.txt | grep apple
apples 7
pineapples 9
```
```bash
cat fruits.txt | grep APPLE
```
```bash
cat fruits.txt | grep -i "^apple"
apples 7
```
```bash
sort fruits.txt
apples 7
bananas 2
grapes 5
oranges 3
pears 6
pineapples 9
```
```bash
cat fruits.txt
grapes 5
apples 7
oranges 3
bananas 2
pears 6
pineapples 9
```
```bash
sort -k 2 fruits.txt
bananas 2
oranges 3
grapes 5
pears 6
apples 7
pineapples 9
```
```bash
sort fruits.txt > sort_by_alphabetical.txt
sort -k 2 fruits.txt > sort_by_price.txt
```
```bash
cat sort_by_alphabetical.txt
apples 7
bananas 2
grapes 5
oranges 3
pears 6
pineapples 9
```
```bash
cat sort_by_price.txt
bananas 2
oranges 3
grapes 5
pears 6
apples 7
pineapples 9
```
```bash
ps -aux | head
USER         PID %CPU %MEM    VSZ   RSS TTY      STAT START   TIME COMMAND
root           1  0.0  0.1 106172 14464 ?        Ss   Aug13   0:04 /sbin/init
root           2  0.0  0.0      0     0 ?        S    Aug13   0:00 [kthreadd]
root           3  0.0  0.0      0     0 ?        S    Aug13   0:00 [pool_workqueue_]
root           4  0.0  0.0      0     0 ?        I<   Aug13   0:00 [kworker/R-rcu_g]
root           5  0.0  0.0      0     0 ?        I<   Aug13   0:00 [kworker/R-sync_]
root           6  0.0  0.0      0     0 ?        I<   Aug13   0:00 [kworker/R-slub_]
root           7  0.0  0.0      0     0 ?        I<   Aug13   0:00 [kworker/R-netns]
root          10  0.0  0.0      0     0 ?        I    Aug13   0:00 [kworker/u256:0-events_unbound]
root          11  0.0  0.0      0     0 ?        I<   Aug13   0:00 [kworker/R-mm_pe]
```
```bash
ps -aux | sort -k 4 -n -r | head -10
polkitd      760  0.0  0.3 2512648 25396 ?       Ssl  Aug13   0:00 /usr/lib/polkit-1/polkitd --no-debug
root         806  0.0  0.2 172920 18304 ?        Ssl  Aug13   0:14 /usr/sbin/rsyslogd -n
root         752  0.0  0.2 253472 18688 ?        Ssl  Aug13   0:41 /usr/sbin/NetworkManager --no-daemon
root      803367  0.0  0.1  18288  8576 pts/0    S    19:45   0:00 sudo -i
root      728318  0.0  0.1  19968 11648 ?        Ss   15:57   0:00 sshd: root [priv]
root         866  0.0  0.1  21664 11520 ?        Ss   Aug13   0:00 /usr/lib/systemd/systemd --user
root         861  0.0  0.1  19940 11648 ?        Ss   Aug13   0:25 sshd: root [priv]
root         778  0.0  0.1 1231272 13052 ?       Ssl  Aug13   0:08 /warewulf/wwclient
root         777  0.0  0.1  16612  9600 ?        Ss   Aug13   0:00 sshd: /usr/sbin/sshd -D [listener] 0 of 10-100 startups
root         756  0.0  0.1 395156 15528 ?        Ssl  Aug13   0:01 /usr/libexec/udisks2/udisksd
```
```bash
cat fruits.txt | grep apple
apples 7
pineapples 9
```
```bash
time dd if=/dev/urandom bs=1024k count=20 | bzip2 -9 >> /dev/null
20+0 records in
20+0 records out
20971520 bytes (21 MB, 20 MiB) copied, 4.98923 s, 4.2 MB/s

real    0m5.043s
user    0m4.823s
sys     0m0.161s
```

