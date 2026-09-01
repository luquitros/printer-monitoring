# Printer Monitoring System

Sistema de monitoramento de impressoras desenvolvido utilizando Prometheus, Grafana, Docker e arquivos de configuração YAML.

O projeto permite monitorar a disponibilidade de impressoras na rede, acompanhar o tempo de resposta e visualizar as métricas através de dashboards.

## Tecnologias utilizadas

- Docker
- Docker Compose
- Prometheus
- Grafana
- Blackbox Exporter
- SNMP Exporter
- YAML
- HTTP
- SNMP

## Arquitetura

```text
Impressoras
     │
     │ HTTP / SNMP
     ▼
Blackbox Exporter / SNMP Exporter
     │
     ▼
Prometheus
     │
     ▼
Grafana