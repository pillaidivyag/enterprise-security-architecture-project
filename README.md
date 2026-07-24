# Enterprise Security Architecture Assessment – Nextcloud Enterprise

## About this project

This repository documents a complete security architecture assessment for an enterprise deployment of Nextcloud.

Architecture
↓

Threat Model
↓

Risk Assessment
↓

Security Controls
↓

Implementation
↓

Validation
↓

Evidence

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
ENTERPRISE-SECURITY-ARCHITECTURE-PROJECT
├── 01-Architecture
│   ├── Architecture-Decisions
│   │   └── ADR-001-Deployment-Model.md
│   ├── Design-Documents
│   │   ├── Business-Requirements.md
│   │   ├── Deployment-Model.md
│   │   ├── Security-Objectives.md
│   │   ├── Security-Requirements.md
│   │   ├── Technology-Selection.md
│   │   └── Trust-Boundaries.md
│   ├── Diagrams
│   │   ├── Data-Flow-Diagram.drawio
│   │   ├── Data-Flow-Diagram.png
│   │   ├── High-Level-Architecture.drawio
│   │   ├── High-Level-Architecture.png
│   │   ├── Trust-Boundary.drawio
│   │   └── Trust-Boundary.png
│   └── README.md
├── 02-Threat-Model
│   ├── Mitigation-Plan.md
│   ├── STRIDE-Analysis.md
│   ├── Threat-Modelling-Methodology.md
│   └── Threat-Register.md
├── 03-Risk-Assessment
│   ├── Diagrams
│   │   ├── Risk-Matrix.drawio
│   │   └── Risk-Matrix.png
│   ├── README.md
│   ├── Risk Treatment Plan.md
│   ├── Risk-Assessment-Methodology.md
│   ├── Risk-Matrix.md
│   └── Risk-Register.md
├── 04-Security-Controls
│   ├── Application-Security.md
│   ├── Architecture-Control-Summary.md
│   ├── Availability-and-Resilience.md
│   ├── Data-Protection.md
│   ├── Identity-and-Access-Management.md
│   ├── Logging-and-Monitoring.md
│   ├── Network-Security.md
│   ├── README.md
│   └── Security-Control-Matrix.md
├── 05-Validation
│   ├── Diagrams
│   │   ├── Validation-Process.drawio
│   │   └── Validation-Process.png
│   ├── Reports
│   │   ├── Lynis.md
│   │   ├── Nikto scanning.png
│   │   └── Nmap scan.png
│   ├── Configuration-Review.md
│   ├── Penetration-Testing.md
│   ├── README.md
│   ├── Security-Control-Validation.md
│   ├── Security-Test-Cases.md
│   ├── Validation-Checklist.md
│   ├── Validation-Strategy.md
│   ├── Validation-Summary.md
│   └── Vulnerability-Assessment.md
├── 06-Implementation
│   ├── Environment-Preparation.md
│   ├── Firewall-Configuration.md          ← Added
│   ├── HTTPS-TLS-Configuration.md
│   ├── Nextcloud-Configuration.md
│   ├── Nextcloud-Hardening.md
│   ├── Nextcloud-Installation.md
│   ├── Nginx-Configuration.md
│   ├── PHP-Configuration.md
│   ├── PostgreSQL-Configuration.md
│   ├── README.md
│   ├── Ubuntu-Hardening.md
│   ├── Firewall-Policy.png                ← Moved here
│   └── UFW-HTTPS-Rule.png                 ← Moved here
├── 07-Evidence
│   ├── Errors-in-the-log.png
│   ├── Least-Privilege.md
│   ├── Least-Privilege.png
│   ├── Nextcloud-Security-Overview.png
│   ├── Nextcloud-setup-page.png
│   ├── Nginx-Welcome-Page.png
│   ├── README.md
│   ├── resolved warnings.png
│   ├── Security-Warnings.drawio
│   ├── Security-Warnings.png
│   └── TLS-Certificate-Details.png
├── README.md
└── Security-Standards-Mapping.md
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
