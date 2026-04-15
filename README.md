# Distributed CI/CD & Monitoring Stack (Tomcat + Jenkins + Prometheus + Grafana)

This project demonstrates a professional DevOps architecture involving automated deployment and real-time observability across a multi-instance AWS environment.

## 🚀 Architecture Overview
* **Instance 1 (App Server):** Apache Tomcat 9, Java Application (nazeef-app), JMX Exporter.
* **Instance 2 (DevOps Server):** Jenkins, Prometheus, Grafana.

## 🛠 Tech Stack
* **Infrastructure:** AWS EC2 (Ubuntu 24.04 LTS)
* **CI/CD:** Jenkins, Maven, GitHub
* **Monitoring:** Prometheus & Grafana
* **Metrics:** JMX Prometheus Java Agent

## 📋 Implementation Details
1. **Automated CI/CD:** Code pushed from Instance 1 is built by Jenkins on Instance 2 and redeployed to Instance 1.
2. **Real-Time Monitoring:** Prometheus scrapes JMX metrics from Instance 1. Grafana visualizes active sessions via the **"Green Line"** graph.
3. **Issue Resolution:** Successfully resolved 100% disk utilization on Instance 2 by optimizing storage and removing unnecessary swap files.

---
*Developed by Muhammed Nazeef | April 2026*
