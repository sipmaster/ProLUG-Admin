Using VictoriaLogs as a replacement for loki

Install Grafana
```bash
sudo wget -q -O /usr/share/keyrings/grafana.key https://apt.grafana.com/gpg.key
echo "deb [signed-by=/usr/share/keyrings/grafana.key] https://apt.grafana.com stable main" | sudo tee -a /etc/apt/sources.list.d/grafana.list
apt update
apt install -y grafana-enterprise
systemctl daemon-reload
systemctl start grafana-server
systemctl status grafana-server --no-pager
ss -ntulp | grep grafana
ss -ntulp | grep 3000
```

Install VictoriaLogs
```bash
wget https://github.com/VictoriaMetrics/VictoriaLogs/releases/download/v1.28.0/victoria-logs-linux-amd64-v1.28.0.tar.gz
tar xf victoria-logs-linux-amd64-v1.28.0.tar.gz
nohup ./victoria-logs-prod &
```

Install victorialogs's Grafana plugin
```bash
grafana-cli plugins install victoriametrics-logs-datasource
systemctl restart grafana-server
```

Install promtail
```bash
apt install promtail
#on debian/ubuntu the log file is syslog, not message
sed -i 's/messages/syslog/' /etc/promtail/config.yml
cd /var/
setfacl -R -m u:promtail:rX log 
setfacl -R -m d:u:promtail:rX log
systemctl start promtail
```

Change the endpoint in promtail
```bash
vi /etc/promtail/config.yml
# change the client url to show http://127.0.0.1:9428/insert/loki/api/v1/push
systemctl restart promtail
```

Create datasource Victorialogs in grafana with http://127.0.0.1:9428 in url
Import dashboard 22759 in grafana choosing VictoriaLogs datasource

![[Pasted image 20250816113430.png]]


