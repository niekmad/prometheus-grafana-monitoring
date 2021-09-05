# Node Exporter as Linux service


1. Download Node Exporter at ~/
```
wget https://github.com/prometheus/node_exporter/releases/download/v*/node_exporter-*.*-amd64.tar.gz
tar xvfz node_exporter-*.*-amd64.tar.gz
cd node_exporter-*.*-amd64
```
2. Create linux service
```
sudo cp node_exporter.service /etc/systemd/systemd/node_exporter.service
sudo systemctl daemon-reload
sudo systemctl start node_exporter.service
sudo systemctl status node_exporter.service
sudo systemctl enable node_exporter.service
```

### Links
- https://prometheus.io/docs/guides/node-exporter/
- https://prometheus.io/download/#node_exporter
