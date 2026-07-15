# Threat Modelling Methodology

## Overview

This document describes the approach used to identify and analyse security threats against the Nextcloud Enterprise deployment.

The threat modelling activity was performed during the security architecture review phase to identify potential security weaknesses before production deployment.

The objective is to understand how an attacker could compromise the system, identify the impact of successful attacks, and recommend appropriate security controls.

---

## Threat Modelling Approach

The STRIDE methodology was selected for this assessment.

STRIDE provides a structured approach to identify threats across different categories:

| Category | Description |
|----------|-------------|
| Spoofing | Attacker impersonates a legitimate user or system |
| Tampering | Unauthorized modification of data or configuration |
| Repudiation | User or system actions cannot be proven or traced |
| Information Disclosure | Exposure of sensitive information |
| Denial of Service | Disruption of service availability |
| Elevation of Privilege | Unauthorized increase in access permissions |

---

## Scope

The threat model covers the following components:

- External users accessing the platform
- Internal employees
- External partner access
- Identity Provider and authentication services
- Reverse Proxy / Web Application Firewall
- Nextcloud application layer
- Database layer
- File storage
- Logging and monitoring components
- Backup infrastructure

---

## Assets Identified

The following assets are considered important within the system:

| Asset | Description | Criticality |
|------|-------------|-------------|
| User credentials | Authentication information used to access the platform | High |
| Business documents | Confidential company files stored within Nextcloud | Critical |
| User accounts | Identity and access permissions | High |
| Database records | Application data and metadata | High |
| Audit logs | Security monitoring and investigation records | High |
| Backup data | Recovery copies of business information | Critical |

---

## Trust Boundaries

The architecture contains multiple trust boundaries:

### External Boundary

Separates untrusted internet users from enterprise infrastructure.

Examples:
- External users
- Partner access
- Internet traffic

### Application Boundary

Separates the web application layer from internal services.

Examples:
- Reverse proxy
- Nextcloud application
- Authentication services

### Data Boundary

Separates application services from sensitive data stores.

Examples:
- Database
- File storage
- Backup systems

---

## Threat Identification Process

Threats will be identified by analysing:

1. Each system component
2. Each data flow between components
3. Each trust boundary
4. Potential attacker actions
5. Security impact

Each identified threat will be documented with:

- Threat description
- STRIDE category
- Affected component
- Potential impact
- Risk rating
- Recommended mitigation

---

## Risk Assessment Approach

Each threat will be evaluated based on:

### Likelihood

How likely the threat is to occur:

- Low
- Medium
- High

### Impact

The potential business impact:

- Low
- Medium
- High

Overall risk will be calculated using:

    **Risk = Likelihood × Impact**

High-risk items will receive priority mitigation recommendations.