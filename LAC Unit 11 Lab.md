```bash
 systemctl status grafana-server --no-pager
● grafana-server.service - Grafana instance
     Loaded: loaded (/usr/lib/systemd/system/grafana-server.service; disabled; preset: enabled)
     Active: active (running) since Fri 2025-08-15 03:37:50 UTC; 25s ago
       Docs: http://docs.grafana.org
   Main PID: 29674 (grafana)
      Tasks: 6 (limit: 2614)
     Memory: 326.1M (peak: 326.3M)
        CPU: 5.206s
     CGroup: /system.slice/grafana-server.service
             └─29674 /usr/share/grafana/bin/grafana server --config=/etc/grafana/grafana.ini --pidfile=/run/grafana/grafana-server.pid --packaging=deb cfg:default.paths.logs=/var/log/gra…

Aug 15 03:38:00 controlplane grafana[29674]: logger=grafana-apiserver t=2025-08-15T03:38:00.456379248Z level=info msg="Adding GroupVersion dashboard.grafana.app v2alpha1 to…sourceManager"
Aug 15 03:38:00 controlplane grafana[29674]: logger=installer.fs t=2025-08-15T03:38:00.45910444Z level=info msg="Downloaded and extracted grafana-pyroscope-app v1.7.0 zip s…pyroscope-app"
Aug 15 03:38:00 controlplane grafana[29674]: logger=plugins.registration t=2025-08-15T03:38:00.559695626Z level=info msg="Plugin registered" pluginId=grafana-pyroscope-app
Aug 15 03:38:00 controlplane grafana[29674]: logger=plugin.backgroundinstaller t=2025-08-15T03:38:00.559938818Z level=info msg="Plugin successfully installed" pluginId=graf…n=439.771167ms
Aug 15 03:38:00 controlplane grafana[29674]: logger=plugin.backgroundinstaller t=2025-08-15T03:38:00.560061081Z level=info msg="Installing plugin" pluginId=grafana-exploret…s-app version=
Aug 15 03:38:00 controlplane grafana[29674]: logger=app-registry t=2025-08-15T03:38:00.561611059Z level=info msg="app registry initialized"
Aug 15 03:38:00 controlplane grafana[29674]: logger=plugin.installer t=2025-08-15T03:38:00.818181457Z level=info msg="Installing plugin" pluginId=grafana-exploretraces-app version=
Aug 15 03:38:00 controlplane grafana[29674]: logger=installer.fs t=2025-08-15T03:38:00.913816676Z level=info msg="Downloaded and extracted grafana-exploretraces-app v1.1.3 …oretraces-app"
Aug 15 03:38:00 controlplane grafana[29674]: logger=plugins.registration t=2025-08-15T03:38:00.9654838Z level=info msg="Plugin registered" pluginId=grafana-exploretraces-app
Aug 15 03:38:00 controlplane grafana[29674]: logger=plugin.backgroundinstaller t=2025-08-15T03:38:00.965734282Z level=info msg="Plugin successfully installed" pluginId=graf…n=405.573054ms
Hint: Some lines were ellipsized, use -l to show in full.
```
```bash
ss -ntulp | grep grafana
tcp   LISTEN 0      4096                                    *:3000             *:*    users:(("grafana",pid=29674,fd=11))                    
controlplane:~$ ss -ntulp | grep 3000
tcp   LISTEN 0      4096                                    *:3000             *:*    users:(("grafana",pid=29674,fd=11))
```
```bash
systemctl enable loki.service --now
Created symlink /etc/systemd/system/default.target.wants/loki.service → /etc/systemd/system/loki.service.
controlplane:/opt/loki$ systemctl status loki.service --no-pager
● loki.service - Loki Startup
     Loaded: loaded (/etc/systemd/system/loki.service; enabled; preset: enabled)
     Active: active (running) since Fri 2025-08-15 03:42:42 UTC; 6s ago
   Main PID: 32886 (loki-linux-amd6)
      Tasks: 6 (limit: 2614)
     Memory: 21.1M (peak: 21.4M)
        CPU: 89ms
     CGroup: /system.slice/loki.service
             └─32886 /opt/loki/loki-linux-amd64 -config.file=/opt/loki/loki-local-config.yaml

Aug 15 03:42:47 controlplane loki-linux-amd64[32886]: level=info ts=2025-08-15T03:42:47.703835879Z caller=compactor.go:474 msg="this instance has been chosen to run the comp…ng compactor"
Aug 15 03:42:47 controlplane loki-linux-amd64[32886]: level=info ts=2025-08-15T03:42:47.703883166Z caller=compactor.go:503 msg="waiting 10m0s for ring to stay stable and pre…ng compactor"
Aug 15 03:42:48 controlplane loki-linux-amd64[32886]: level=debug ts=2025-08-15T03:42:48.55640139Z caller=mock.go:186 msg="Get - deadline exceeded" key=collectors/compactor
Aug 15 03:42:48 controlplane loki-linux-amd64[32886]: level=debug ts=2025-08-15T03:42:48.556433568Z caller=mock.go:150 msg=Get key=collectors/compactor wait_index=5
Aug 15 03:42:48 controlplane loki-linux-amd64[32886]: level=debug ts=2025-08-15T03:42:48.556443247Z caller=mock.go:186 msg="Get - deadline exceeded" key=collectors/scheduler
Aug 15 03:42:48 controlplane loki-linux-amd64[32886]: level=debug ts=2025-08-15T03:42:48.556451065Z caller=mock.go:150 msg=Get key=collectors/scheduler wait_index=6
Aug 15 03:42:48 controlplane loki-linux-amd64[32886]: level=debug ts=2025-08-15T03:42:48.556456768Z caller=mock.go:186 msg="Get - deadline exceeded" key=collectors/distributor
Aug 15 03:42:48 controlplane loki-linux-amd64[32886]: level=debug ts=2025-08-15T03:42:48.556476386Z caller=mock.go:150 msg=Get key=collectors/distributor wait_index=4
Aug 15 03:42:48 controlplane loki-linux-amd64[32886]: level=debug ts=2025-08-15T03:42:48.556482479Z caller=mock.go:186 msg="Get - deadline exceeded" key=collectors/ring
Aug 15 03:42:48 controlplane loki-linux-amd64[32886]: level=debug ts=2025-08-15T03:42:48.556489514Z caller=mock.go:150 msg=Get key=collectors/ring wait_index=8
Hint: Some lines were ellipsized, use -l to show in full.
controlplane:/opt/loki$ ss -ntulp | grep 3100
tcp   LISTEN 0      4096                                    *:3100             *:*    users:(("loki-linux-amd6",pid=32886,fd=8))             
```
```bash
 systemctl status promtail.service --no-pager
● promtail.service - Promtail Service Startup
     Loaded: loaded (/etc/systemd/system/promtail.service; enabled; preset: enabled)
     Active: active (running) since Fri 2025-08-15 03:44:28 UTC; 4s ago
   Main PID: 33914 (promtail-linux-)
      Tasks: 8 (limit: 2614)
     Memory: 14.8M (peak: 15.0M)
        CPU: 47ms
     CGroup: /system.slice/promtail.service
             └─33914 /opt/promtail/promtail-linux-amd64 -config.file=/opt/promtail/promtail-local-config.yaml

Aug 15 03:44:28 controlplane systemd[1]: Started promtail.service - Promtail Service Startup.
Aug 15 03:44:29 controlplane promtail-linux-amd64[33914]: level=info ts=2025-08-15T03:44:28.926372257Z caller=promtail.go:123 msg="Reloading configuration file" md5sum=83f74…be7f5eff283fd
Aug 15 03:44:29 controlplane promtail-linux-amd64[33914]: level=info ts=2025-08-15T03:44:28.92695828Z caller=server.go:323 http=[::]:9080 grpc=[::]:37957 msg="server listeni…on addresses"
Aug 15 03:44:29 controlplane promtail-linux-amd64[33914]: level=info ts=2025-08-15T03:44:28.927101739Z caller=main.go:171 msg="Starting Promtail" version="(version=HEAD-e0af…n=e0af1cc8a)"
Aug 15 03:44:29 controlplane promtail-linux-amd64[33914]: level=warn ts=2025-08-15T03:44:28.942341747Z caller=promtail.go:220 msg="enable watchConfig"
Hint: Some lines were ellipsized, use -l to show in full.
controlplane:/opt/promtail$ ps -ef | grep [p]romtail
root       33914       1  0 03:44 ?        00:00:00 /opt/promtail/promtail-linux-amd64 -config.file=/opt/promtail/promtail-local-config.yaml
```
```bash
status prometheus.service --no-pager
● prometheus.service - Prometheus
     Loaded: loaded (/etc/systemd/system/prometheus.service; disabled; preset: enabled)
     Active: active (running) since Fri 2025-08-15 14:12:18 UTC; 3s ago
   Main PID: 156313 (prometheus)
      Tasks: 6 (limit: 2614)
     Memory: 15.2M (peak: 15.5M)
        CPU: 52ms
     CGroup: /system.slice/prometheus.service
             └─156313 /usr/bin/prometheus --config.file /etc/prometheus/prometheus.yml --storage.tsdb.path /var/lib/prometheus/ --web.console.templates=/var/lib/prometheus/consoles --web…

Aug 15 14:12:18 controlplane prometheus[156313]: ts=2025-08-15T14:12:18.424Z caller=tls_config.go:232 level=info component=web msg="Listening on" address=[::]:9090
Aug 15 14:12:18 controlplane prometheus[156313]: ts=2025-08-15T14:12:18.424Z caller=tls_config.go:235 level=info component=web msg="TLS is disabled." http2=false address=[::]:9090
Aug 15 14:12:18 controlplane prometheus[156313]: ts=2025-08-15T14:12:18.424Z caller=head.go:685 level=info component=tsdb msg="WAL segment loaded" segment=0 maxSegment=0
Aug 15 14:12:18 controlplane prometheus[156313]: ts=2025-08-15T14:12:18.425Z caller=head.go:722 level=info component=tsdb msg="WAL replay completed" checkpoint_replay_durat…ion=2.169384ms
Aug 15 14:12:18 controlplane prometheus[156313]: ts=2025-08-15T14:12:18.427Z caller=main.go:1014 level=info fs_type=EXT4_SUPER_MAGIC
Aug 15 14:12:18 controlplane prometheus[156313]: ts=2025-08-15T14:12:18.427Z caller=main.go:1017 level=info msg="TSDB started"
Aug 15 14:12:18 controlplane prometheus[156313]: ts=2025-08-15T14:12:18.427Z caller=main.go:1197 level=info msg="Loading configuration file" filename=/etc/prometheus/prometheus.yml
Aug 15 14:12:18 controlplane prometheus[156313]: ts=2025-08-15T14:12:18.428Z caller=main.go:1234 level=info msg="Completed loading of configuration file" filename=/etc/prometheus/prometh…
Aug 15 14:12:18 controlplane prometheus[156313]: ts=2025-08-15T14:12:18.428Z caller=main.go:978 level=info msg="Server is ready to receive web requests."
Aug 15 14:12:18 controlplane prometheus[156313]: ts=2025-08-15T14:12:18.428Z caller=manager.go:974 level=info component="rule manager" msg="Starting rule manager..."
Hint: Some lines were ellipsized, use -l to show in full.
controlplane:/opt/node_exporter/node_exporter-1.5.0.linux-amd64$ ps -ef | grep [p]rometheus
prometh+  156313       1  1 14:12 ?        00:00:00 /usr/bin/prometheus --config.file /etc/prometheus/prometheus.yml --storage.tsdb.path /var/lib/prometheus/ --web.console.templates=/var/lib/prometheus/consoles --web.console.libraries=/var/lib/prometheus/console_libraries
```
```bash
ss -ntulp | grep 8086
tcp   LISTEN 0      4096                                    *:8086             *:*    users:(("influxd",pid=33508,fd=9))                    
controlplane:~$ lsof -i :8086
COMMAND   PID     USER   FD   TYPE DEVICE SIZE/OFF NODE NAME
influxd 33508 influxdb    9u  IPv6 178241      0t0  TCP *:8086 (LISTEN)
```
```bash
user: me
passwd: -$UC8w#dcJ8iS@4
organization: ME
bucket: bucket
toekn: NNAbGCHA3yvnwOfSxqmGIh2yvz8Ry1T5UQ-Q7CbE97qbKYmdAyRYeU4J3zTRBFe9kCy7YNCOTINA1l1NBTrNJQ==

controlplane:~$ systemctl status telegraf --no-pager -l
● telegraf.service - Telegraf
     Loaded: loaded (/usr/lib/systemd/system/telegraf.service; enabled; preset: enabled)
     Active: active (running) since Fri 2025-08-15 15:05:01 UTC; 16ms ago
       Docs: https://github.com/influxdata/telegraf
   Main PID: 38428 (telegraf)
      Tasks: 5 (limit: 2614)
     Memory: 102.1M (peak: 102.3M)
        CPU: 85ms
     CGroup: /system.slice/telegraf.service
             ├─38428 /usr/bin/telegraf -config /etc/telegraf/telegraf.conf -config-directory /etc/telegraf/telegraf.d
             └─38443 /usr/bin/dbus-daemon --syslog --fork --print-pid 4 --print-address 6 --session

Aug 15 15:05:00 controlplane systemd[1]: Starting telegraf.service - Telegraf...
Aug 15 15:05:00 controlplane (telegraf)[38428]: telegraf.service: Referenced but unset environment variable evaluates to an empty string: TELEGRAF_OPTS
Aug 15 15:05:01 controlplane dbus-daemon[38443]: [session uid=995 pid=38441] AppArmor D-Bus mediation is enabled
Aug 15 15:05:01 controlplane systemd[1]: Started telegraf.service - Telegraf.
```
