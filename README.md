# 🚀 DevOps Monitoring API

Projeto de monitoramento desenvolvido com **Spring Boot, PostgreSQL, Docker, Prometheus e Grafana**.

O objetivo é criar uma aplicação preparada para práticas de **DevOps, observabilidade e monitoramento de APIs**.

## 🛠️ Tecnologias

- Java 21
- Spring Boot
- Spring Data JPA
- PostgreSQL 16
- Docker
- Docker Compose
- Prometheus
- Grafana
- Micrometer
- Spring Boot Actuator
- Maven
- Git/GitHub

## 🏗️ Arquitetura

```text
                 ┌─────────────────┐
                 │   Spring Boot   │
                 │      API        │
                 │     :8080       │
                 └────────┬────────┘
                          │
              /actuator/prometheus
                          │
                          ▼
                 ┌─────────────────┐
                 │   Prometheus    │
                 │      :9090      │
                 └────────┬────────┘
                          │
                          ▼
                 ┌─────────────────┐
                 │     Grafana     │
                 │      :3000      │
                 └─────────────────┘

                 ┌─────────────────┐
                 │   PostgreSQL    │
                 │      :5432      │
                 └─────────────────┘
