# enterprise-security-architecture-project
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
01-Architecture
│
├── Design Documents
├── Architecture Decisions
├── Diagrams

02-Threat-Model

03-Risk-Assessment

04-Security-Controls

05-Validation

06-Documentation
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
