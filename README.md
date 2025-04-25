# System Monitoring Dashboard

A real-time system monitoring dashboard built with Prometheus, Node Exporter, and Grafana on Ubuntu (WSL2). This project visualizes key system metrics like CPU, memory, disk I/O, and swap usage through a clean Grafana interfaces.
## Features
- Real-time system metrics using Node Exporter
- Fully functional Prometheus server scraping configured targets
- Grafana dashboard for visual insights
- Monitors:
  - CPU usage
  - Memory usage
  - Disk I/O
  - Swap usage
  - System load
## 🛠Requirements
- Ubuntu with WSL2 (or any Linux distro)
- Prometheus (v2.52.0+)
- Node Exporter (v1.8.0+)
- Grafana (v11+)
- Git
## Getting Started
 1. Clone the Repository
#Bash Code 
git clone https://github.com/Rochak24/system-monitoring-dashboard.git
cd system-monitoring-dashboard

#Bash Code 
cd node_exporter-1.8.0.linux-amd64
./node_exporter

#Bash Code 
cd prometheus-2.52.0.linux-amd64
./prometheus --config.file=../prometheus.yml


#Local Host 3000/ Grafana
http://localhost:3000/d/rYdddlPWk/node-exporter-full?orgId=1&from=now-5m&to=now&timezone=browser&var-datasource=default&var-job=node_exporter&var-nodename=XORG&var-node=localhost:9100&var-diskdevices=%5Ba-z%5D%2B%7Cnvme%5B0-9%5D%2Bn%5B0-9%5D%2B%7Cmmcblk%5B0-9%5D%2B&refresh=5s

#Local Host 9090 / Prometheus/ node_exporter
http://localhost:9090/targets?search=
