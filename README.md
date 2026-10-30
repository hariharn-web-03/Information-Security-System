# Information Security System & SIEM Monitoring 🛡️📈

A comprehensive enterprise defense and vulnerability management project centered around SIEM monitoring, centralized log collection, host firewall hardening, and automated vulnerability scanning.

---

## 📋 Table of Contents
- [Project Scope](#-project-scope)
- [SIEM Integration & Wazuh Deployment](#-siem-integration--wazuh-deployment)
- [Custom Threat Detection Rules](#-custom-threat-detection-rules)
- [Vulnerability Scanning & Hardening](#-vulnerability-scanning--hardening)

---

## 🎯 Project Scope
Focuses on establishing robust defensive visibility, detecting brute-force attacks in real time, hardening operating system firewalls, and managing asset vulnerability lifecycles.

---

## 👁️ SIEM Integration & Wazuh Deployment
* **Multi-Platform Agents**: Deployed and configured Wazuh security agents across Linux (`Ubuntu`, `RHEL`) and Windows endpoints (`Windows Server 2019`, `Windows 10`)[cite: 82, 176, 191].
* **Audit Policy Integration**: Enabled advanced audit logging (`auditpol` / Windows Security Event logs) to feed authentication success/failure metrics directly into the SIEM dashboard[cite: 32, 188].

---

## 🚨 Custom Threat Detection Rules
* **Custom Alerting**: Developed specialized XML rules (`local_rules.xml`) within Wazuh to trigger high-priority alerts upon detecting repeated authentication failures, suspicious script execution, or unauthorized service attempts[cite: 196].

---

## 🔍 Vulnerability Scanning & Hardening
* **Nessus Scanning**: Conducted scheduled vulnerability assessments against lab subnets to locate unpatched software, missing security patches, and legacy operating systems[cite: 206].
* **Firewall Hardening**: Configured Windows Defender Firewall with Advanced Security rules (`netsh` / Inbound Rule Wizard) to block high-risk ports such as SMB (`445`) and RDP against lateral traversal[cite: 219].
