# 🛡️ Wazuh SIEM Installation, Configuration & SOC Monitoring

## 📌 Project Overview
This project demonstrates the **complete installation, configuration, and basic usage of Wazuh**, an open-source **SIEM and XDR platform**. It showcases how a **Security Operations Center (SOC)** monitors systems, detects security threats, and analyzes logs in real-time.

This project was created as part of a **cybersecurity academic requirement** and focuses on **Blue Team / SOC fundamentals**.

---

## 🎯 Project Objectives
* **Understand SOC Operations:** Learn how SIEM tools function within a security team.
* **Deployment:** Install and configure the Wazuh manager and agents.
* **Log Monitoring:** Centralize system and security logs for analysis.
* **Threat Detection:** Identify suspicious activities such as Failed login attempts and File integrity changes.
* **Visualization:** Use the Wazuh dashboard to create actionable security insights.

---

## 🧠 Core Concepts

### What is SOC?
A **Security Operations Center (SOC)** is a centralized team responsible for **monitoring, detecting, analyzing, and responding to cybersecurity incidents** in real time. Analysts rely on SIEM tools to protect organizational data.

### What is Wazuh?
**Wazuh** is a powerful open-source security platform used for:
* **Log Analysis:** Collecting and parsing data from various sources.
* **HIDS:** Host-based intrusion detection.
* **FIM:** File Integrity Monitoring.
* **Vulnerability Detection:** Identifying outdated or insecure software.

---

## 🧱 Wazuh Architecture
Wazuh follows a **server–agent model**:

`Wazuh Agent` → `Wazuh Server (Manager)` → `Wazuh Dashboard`

* **Wazuh Server:** The "brain" that collects, parses, and analyzes logs.
* **Wazuh Agent:** Installed on end-points (Windows, Linux, etc.) to monitor activity.
* **Dashboard:** The web user interface used for visualization and alert management.

---

## 🛠️ Tools & Technologies Used
* **OS:** Ubuntu Linux (Virtual Machine)
* **SIEM:** Wazuh (Server & Agent)
* **Stack:** ELK Stack (Elasticsearch, Kibana - integrated)
* **Hypervisor:** VirtualBox / VMware

---

## 🚀 Installation & Setup

### 1️⃣ Install Wazuh Server
The server was installed using the official "All-in-One" installation script:

```bash
curl -sO [https://packages.wazuh.com/4.7/wazuh-install.sh](https://packages.wazuh.com/4.7/wazuh-install.sh)
sudo bash wazuh-install.sh -a
