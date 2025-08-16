## Using VictoriaLogs as a replacement for Loki

#### Install Grafana
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

#### Install VictoriaLogs
```bash
wget https://github.com/VictoriaMetrics/VictoriaLogs/releases/download/v1.28.0/victoria-logs-linux-amd64-v1.28.0.tar.gz
tar xf victoria-logs-linux-amd64-v1.28.0.tar.gz
nohup ./victoria-logs-prod &
```

#### Install victorialogs's Grafana plugin
```bash
grafana-cli plugins install victoriametrics-logs-datasource
systemctl restart grafana-server
```

#### Install promtail
```bash
apt install promtail
#on debian/ubuntu the log file is syslog, not message
sed -i 's/messages/syslog/' /etc/promtail/config.yml
cd /var/
#Fix access permission on files
setfacl -R -m u:promtail:rX log 
setfacl -R -m d:u:promtail:rX log
systemctl start promtail
```

#### Change the endpoint in promtail
```bash
vi /etc/promtail/config.yml
# change the client url to show http://127.0.0.1:9428/insert/loki/api/v1/push
systemctl restart promtail
```

#### Create datasource Victorialogs in grafana with http://127.0.0.1:9428 in url

#### Import dashboard 22759 in grafana choosing VictoriaLogs datasource
![[Pasted image 20250816113430.png]]

## Using VictoriaMetrics to replace Prometheus
#### Install Node exporter
```bash
apt install -y prmometheus-node-exporter prometheus-node-exporter-collectors
systemctl start prometheus-node-exporter 
systemctl status prometheus-node-exporter --no-pager
```

#### Install vmagent
```bash
wget https://github.com/VictoriaMetrics/VictoriaMetrics/releases/download/v1.123.0/vmutils-linux-amd64-v1.123.0.tar.gz
tar xf vmutil*.tar.gz
```

#### Install VictoriaMetrics
```bash
wget https://github.com/VictoriaMetrics/VictoriaMetrics/releases/download/v1.123.0/victoria-metrics-linux-amd64-v1.123.0.tar.gz
tar xf victoria-metrics*.tar.gz
nohup ./victoria-matrics-prod &
```

#### Copy prometheus.yaml
```yaml
# my global config
global:
  scrape_interval: 15s # Set the scrape interval to every 15 seconds. Default is every 1 minute.
  evaluation_interval: 15s # Evaluate rules every 15 seconds. The default is every 1 minute.
  # scrape_timeout is set to the global default (10s).

# Alertmanager configuration
alerting:
  alertmanagers:
    - static_configs:
        - targets:
          # - alertmanager:9093

# Load rules once and periodically evaluate them according to the global 'evaluation_interval'.
rule_files:
  # - "first_rules.yml"
  # - "second_rules.yml"

# A scrape configuration containing exactly one endpoint to scrape:
# Here it's Prometheus itself.
scrape_configs:
  # The job name is added as a label `job=<job_name>` to any timeseries scraped from this config.
  - job_name: "prometheus"

    # metrics_path defaults to '/metrics'
    # scheme defaults to 'http'.

    static_configs:
      #      - targets: ["localhost:9090"]
      - targets: ['localhost:9100']

  - job_name: 'Prometheus_node'
    static_configs:
    - targets: ['localhost:9100']
```

#### Start vmagent
```bash
nohup ./vmagent-prod -promscrape.config=prometheus.yaml -promscrape.config.strictParse=false -remoteWrite.url=http://127.0.0.1:8428/api/v1/write &
```

#### Install Grafana plugin
```bash
grafana-cli plugins install victoriametrics-metrics-datasource
systemctl restart grafana-server
```

##### Create 1 victoria-metrics and 1 prometheus datasource with both http://127.0.0.1:8428

##### Import dashboard 159 in Grafana

![[Pasted image 20250816150636.png]]
