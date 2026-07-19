# Enterprise Security Architecture Assessment – Nextcloud Enterprise

## About this project

This repository documents a complete security architecture assessment for an enterprise deployment of Nextcloud.

I created this project to demonstrate how a Security Architect approaches the design and review of an enterprise application before it is deployed into production.

Rather than focusing on a single security tool, the project follows the complete security architecture lifecycle—from understanding business requirements through to architecture design, threat modelling, risk assessment, security controls, and validation.

The aim is to produce documentation and design artefacts similar to those created during a real security architecture engagement.

---

## Project scenario

Organisation X with around 5000 employees operating across multiple locations.

The company plans to deploy Nextcloud as its enterprise file-sharing and collaboration platform. Employees need to securely store, share, and access business documents while approved external partners require limited access to specific project files.

Before deployment, the organisation requests a security architecture assessment to identify potential security risks, recommend appropriate security controls, and ensure the proposed design aligns with secure-by-design principles.

---

## What this project covers

This assessment includes:

* Business and security requirements
* High-level security architecture
* Data flow modelling
* Threat modelling using STRIDE
* Risk assessment
* Security control recommendations
* Architecture validation
* Security documentation

---

## Repository structure

```text
enterprise-security-architecture-project/
│
├── README.md
│
├── 01-Architecture
│   ├── README.md
│   ├── Design-Documents
│   │   ├── Business-Requirements.md
│   │   ├── Security-Objectives.md
│   │   ├── Deployment-Model.md
│   │   ├── Security-Requirements.md
│   │   ├── Trust-Boundaries.md
│   │   └── Technology-Selection.md
│   │
│   ├── Architecture-Decisions
│   │   └── ADR-001-Deployment-Model.md
│   │
│   └── Diagrams
│       ├── High-Level-Architecture.drawio
│       ├── High-Level-Architecture.png
│       ├── Data-Flow-Diagram.drawio
│       ├── Data-Flow-Diagram.png
│       ├── Trust-Boundary.drawio
│       └── Trust-Boundary.png
│
├── 02-Threat-Model
│   ├── README.md
│   ├── STRIDE-Analysis.md
│   ├── Threat-Modelling-Methodology.md
│   └── Threat-Register.md
│
├── 03-Risk-Assessment
│   ├── README.md
│   ├── Risk-Assessment-Methodology.md
│   ├── Risk-Register.md
│   ├── Risk Treatment Plan.md
│   ├── Risk-Matrix.md
│   └── Diagrams
│       ├── Risk-Matrix.drawio
│       └── Risk-Matrix.png
│
├── 04-Security-Controls
│   ├── README.md
│   ├── Identity-and-Access-Management.md
│   ├── Data-Protection.md
│   ├── Network-Security.md
│   ├── Application-Security.md
│   ├── Logging-and-Monitoring.md
│   ├── Availability-and-Resilience.md
│   ├── Security-Control-Matrix.md
│   └── Architecture-Control-Summary.md
│
├── 05-Validation
│   ├── README.md
│   ├── Validation-Strategy.md
│   ├── Security-Test-Cases.md
│   ├── Validation-Checklist.md
│   ├── Security-Control-Validation.md
│   ├── Vulnerability-Assessment.md
│   ├── Penetration-Testing.md
│   ├── Configuration-Review.md
│   ├── Validation-Summary.md
│   ├── Diagrams
│   │   └── Validation-Workflow.drawio
│   └── Reports
│       ├── Nmap-Scan.md
│       ├── OWASP-ZAP.md
│       ├── Nikto.md
│       └── Lynis.md
│
├── 06-Implementation
│   ├── README.md
│   ├── Environment-Preparation.md
│   ├── Ubuntu-Hardening.md
│   ├── PostgreSQL-Configuration.md
│   ├── Nginx-Configuration.md
│   ├── PHP-Configuration.md
│   ├── Nextcloud-Installation.md
│   ├── SSL-TLS-Configuration.md
│   ├── Firewall-Configuration.md
│   ├── Fail2Ban-Configuration.md
│   ├── Nextcloud-Hardening.md
│   ├── Backup-and-Recovery.md
│   ├── Scripts
│   │   ├── backup.sh
│   │   ├── restore.sh
│   │   └── install-notes.md
│   └── Configuration
│       ├── nginx.conf
│       ├── php.ini
│       ├── nextcloud-config.php
│       ├── ufw-rules.txt
│       └── fail2ban-jail.local
|
└── 06-Implementation
│   ├── README.md
│   ├── Environment-Preparation.md
│   ├── Ubuntu-Hardening.md
│   ├── PostgreSQL-Configuration.md
│   ├── Nginx-Configuration.md
│   ├── PHP-Configuration.md
│   ├── Nextcloud-Installation.md
│   ├── SSL-TLS-Configuration.md
│   ├── Firewall-Configuration.md
│   ├── Fail2Ban-Configuration.md
│   ├── Nextcloud-Hardening.md
│   ├── Backup-and-Recovery.md
│   ├── Scripts
│   │   ├── backup.sh
│   │   ├── restore.sh
│   │   └── install-notes.md
│   └── Configuration
│       ├── nginx.conf
│       ├── php.ini
│       ├── nextcloud-config.php
│       ├── ufw-rules.txt
│       └── fail2ban-jail.local
```

---

## Technologies and concepts

The project uses Nextcloud as the application being assessed and applies common enterprise security concepts including:

* Identity and Access Management (SSO, MFA and RBAC)
* Data protection
* Network segmentation
* Secure application design
* Logging and monitoring
* Backup and recovery
* Defence in depth
* Least privilege
* Zero Trust principles

The assessment is based on widely recognised security practices including STRIDE threat modelling, the NIST Cybersecurity Framework, NIST SP 800-53 and ISO/IEC 27001.

---

## Why I built this project

I wanted to create a realistic security architecture project that demonstrates practical design and risk assessment skills rather than focusing only on security tools or certifications.

The objective is to build a portfolio that reflects how a Security Architect approaches an enterprise application review, documents design decisions, identifies security risks, and recommends appropriate controls.

As the project progresses, additional artefacts such as threat models, risk registers, security control mappings and validation reports will be added.

---
