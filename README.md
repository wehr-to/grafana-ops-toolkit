# 📊 grafana-ops

A hands-on toolkit for managing, provisioning, and securing Grafana environments — including dashboards, alerts, data sources, and automation scripts.

## 🔧 Dashboards

- `linux-hosts.json`: System health and performance
- `cloudwatch-lambda.json`: Function monitoring via AWS CloudWatch
- `prometheus-node-exporter.json`: Infra stats from exporters

📂 Easily import into Grafana UI or use provisioning.

## 🌐 Datasources

- `prometheus.yaml`: Connects to Prometheus server
- `loki.yaml`: Central log aggregation (Loki)
- `cloudwatch.yaml`: Ties AWS metrics into Grafana

## ⚙️ Provisioning

Grafana’s built-in provisioning is supported for:
- Dashboards (`provisioning/dashboards/dashboards.yaml`)
- Datasources (`provisioning/datasources/datasources.yaml`)

This allows for code-based, version-controlled Grafana setup.

## 🚨 Alerts

- `cpu-usage-alert.json`: Example Grafana alert rule
- `disk-space-alert.json`: Basic threshold rule for disk utilization

🔐 Alerting integrations with Slack, Teams, and Webhooks can be added later.

## 🛠️ Tools

- `import-dashboards.sh`: Import dashboards via Grafana API
- `backup-dashboards.sh`: Export all current dashboards to JSON
- `grafana-api.md`: Basic usage of Grafana’s REST API

## 🔐 Security

Best practices for:
- LDAP and OAuth authentication
- Role-based folder permissions
- API token use and Grafana secrets

## 🧠 Ideal Use Cases

- Build and version-control your observability stack
- Integrate Prometheus and CloudWatch monitoring
- Automate dashboards for dev, staging, and prod
- Create a demo lab for platform observability interviews

## 🚀 Roadmap

- [ ] Add Loki + Promtail logging pipeline
- [ ] Create Terraform module for Grafana + Prometheus setup
- [ ] Add scripted dashboard generation (jsonnet or grafonnet)
- [ ] Secure with Vault-based secrets for cloud datasources
