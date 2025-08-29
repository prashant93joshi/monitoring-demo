# Monitoring Demo Project

This repository contains a monitoring setup using Prometheus, Node Exporter, Alertmanager, and Grafana.

## Setup

1. Clone the repo:
```bash
git clone https://github.com/prashant93joshi/monitoring-demo.git
cd monitoring-demo

2. Copy systemd service files:
sudo cp systemd/*.service /etc/systemd/system/
sudo systemctl daemon-reload

3. Enable and start services:
sudo systemctl enable prometheus nodeexporter alertmanager grafana-server
sudo systemctl start prometheus nodeexporter alertmanager grafana-server

Access

Prometheus → http://<vm-ip>:9090

Node Exporter → http://<vm-ip>:9100/metrics

Alertmanager → http://<vm-ip>:9093

Grafana → http://<vm-ip>:3000

*********END*********
