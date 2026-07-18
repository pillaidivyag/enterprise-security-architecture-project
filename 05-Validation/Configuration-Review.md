# Configuration Review

## Purpose

This document defines the configuration review process for the proposed Nextcloud Enterprise deployment.

The objective is to verify that systems are configured according to the approved security architecture and secure baseline.

---

# Objectives

Configuration reviews aim to:

- Confirm secure configuration
- Detect configuration drift
- Verify compliance with security requirements
- Reduce the likelihood of misconfiguration-related incidents

---

# Review Scope

Configuration reviews include:

- Operating systems
- Nextcloud application
- PostgreSQL database
- Reverse Proxy
- Web Application Firewall (WAF)
- Firewall configuration
- Logging configuration
- Backup configuration

---

# Configuration Checklist

## Operating System

Verify:

- Latest security updates installed
- Unnecessary services disabled
- Secure SSH configuration
- Host firewall enabled
- Time synchronisation configured

---

## Nextcloud

Verify:

- Secure configuration applied
- HTTPS enforced
- Administrative accounts reviewed
- File sharing restrictions configured
- Audit logging enabled

---

## Database

Verify:

- Strong authentication enabled
- Least privilege applied
- TLS enabled
- Default accounts removed
- Backups configured

---

## Network

Verify:

- Firewall rules match approved architecture
- Network segmentation implemented
- Administrative interfaces restricted
- Reverse Proxy correctly configured

---

## Logging

Verify:

- Audit logging enabled
- Logs forwarded to SIEM
- Log retention configured
- Time synchronisation functioning

---

## Backup

Verify:

- Scheduled backups configured
- Encryption enabled
- Backup restoration tested
- Off-site storage configured where applicable

---

# Review Evidence

Evidence may include:

- Configuration screenshots
- Configuration files
- System commands
- Firewall rules
- Application settings
- Backup reports

---

# Findings

Configuration review findings should be classified as:

| Rating | Description |
|---------|-------------|
| Compliant | Meets approved configuration baseline |
| Observation | Minor improvement recommended |
| Non-Compliant | Requires corrective action |

---

# Summary

Regular configuration reviews help ensure the deployed environment remains aligned with the approved security architecture and reduces the likelihood of security issues caused by configuration errors.