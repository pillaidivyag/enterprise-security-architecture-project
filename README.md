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
├── 01-Business-Requirements/
│   ├── Business-Requirements.md
│   ├── Stakeholders.md
│   ├── Assumptions-and-Constraints.md
│   └── Security-Objectives.md
│
├── 02-Architecture/
│   ├── README.md
│   ├── Design-Documents/
│   │   ├── Deployment-Model.md
│   │   ├── Security-Requirements.md
│   │   ├── Trust-Boundaries.md
│   │   ├── Data-Flow.md
│   │   └── Technology-Selection.md
│   │
│   ├── Architecture-Decisions/
│   │   ├── ADR-001-Deployment-Model.md
│   │   ├── ADR-002-Database-Selection.md
│   │   ├── ADR-003-Reverse-Proxy.md
│   │   └── ADR-004-Authentication.md
│   │
│   └── Diagrams/
│       ├── High-Level-Architecture.drawio
│       ├── High-Level-Architecture.png
│       ├── Data-Flow-Diagram.drawio
│       ├── Data-Flow-Diagram.png
│       └── Trust-Boundary-Diagram.drawio
│
├── 03-Threat-Model/
│   ├── README.md
│   ├── STRIDE-Analysis.md
│   ├── Attack-Surface.md
│   ├── Threat-Scenarios.md
│   ├── Mitigation-Plan.md
│   └── Diagrams/
│       ├── Threat-Model.drawio
│       └── Threat-Model.png
│
├── 04-Risk-Assessment/
│   ├── README.md
│   ├── Risk-Assessment-Methodology.md
│   ├── Risk-Register.md
│   ├── Risk-Matrix.md
│   └── Diagrams/
│       ├── Risk-Matrix.drawio
│       └── Risk-Matrix.png
│
├── 05-Security-Controls/
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
├── 06-Implementation/
│   ├── README.md
│   ├── Environment-Setup.md
│   ├── Ubuntu-Hardening.md
│   ├── PostgreSQL-Setup.md
│   ├── Nginx-Configuration.md
│   ├── PHP-Configuration.md
│   ├── Nextcloud-Installation.md
│   ├── SSL-TLS-Configuration.md
│   ├── UFW-Firewall.md
│   ├── Fail2Ban.md
│   ├── MFA-Configuration.md
│   ├── Backup-and-Recovery.md
│   └── Scripts/
│       ├── install-nextcloud.sh
│       ├── backup.sh
│       └── restore.sh
│
├── 07-Validation/
│   ├── README.md
│   ├── Security-Testing-Plan.md
│   ├── Validation-Checklist.md
│   ├── Vulnerability-Assessment.md
│   ├── Penetration-Testing.md
│   ├── Security-Compliance.md
│   ├── Lessons-Learned.md
│   └── Reports/
│       ├── Nmap-Scan.md
│       ├── OWASP-ZAP.md
│       ├── Nikto.md
│       └── Lynis.md
│
├── 08-Evidence/
│   ├── Screenshots/
│   │   ├── Ubuntu-Desktop.png
│   │   ├── PostgreSQL-Service.png
│   │   ├── Nginx-Running.png
│   │   ├── Nextcloud-Login.png
│   │   ├── HTTPS-Certificate.png
│   │   ├── MFA.png
│   │   ├── Firewall-Rules.png
│   │   ├── Fail2Ban.png
│   │   ├── Audit-Logs.png
│   │   └── Backup-Success.png
│   │
│   ├── Vulnerability-Scans/
│   │   ├── nmap.xml
│   │   ├── zap-report.html
│   │   ├── nikto.txt
│   │   └── lynis-report.dat
│   │
│   └── Logs/
│       ├── nginx.log
│       ├── auth.log
│       └── nextcloud.log
│
├── 09-Documentation/
│   ├── Project-Summary.md
│   ├── Security-Architecture-Report.md
│   ├── Operations-Guide.md
│   ├── Incident-Response-Guide.md
│   └── Future-Improvements.md
│
└── .gitignore
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
