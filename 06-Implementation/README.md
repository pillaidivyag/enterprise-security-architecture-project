# Implementation

## Overview

This phase documents the practical implementation of the enterprise security architecture designed during the previous phases.

The implementation focuses on deploying and securing a self-hosted Nextcloud environment using open-source technologies on Ubuntu Linux. Each component is installed, configured, hardened, and validated according to security best practices.

The objective is not only to deploy a functional file-sharing platform, but also to demonstrate the practical application of security architecture principles.

---

## Implementation Scope

The implementation includes:

- Ubuntu Server preparation
- Operating system hardening
- PostgreSQL database configuration
- PHP installation and configuration
- Nginx web server configuration
- Nextcloud deployment
- HTTPS/TLS configuration
- Firewall implementation
- Fail2Ban configuration
- Nextcloud security hardening
- Backup and recovery configuration

---

## Technologies

| Technology | Purpose |
|------------|----------|
| Ubuntu Server LTS | Operating System |
| PostgreSQL | Database |
| PHP-FPM | Application Runtime |
| Nginx | Reverse Proxy / Web Server |
| Nextcloud | File Collaboration Platform |
| UFW | Host Firewall |
| Fail2Ban | Intrusion Prevention |
| OpenSSL / Let's Encrypt | TLS Certificates |

---

## Security Principles Applied

Throughout the implementation the following principles are applied:

- Defence in Depth
- Least Privilege
- Secure by Default
- Principle of Separation
- Secure Configuration
- Continuous Validation

---

## Related Documents

- Environment Preparation
- Ubuntu Hardening
- PostgreSQL Configuration
- Nginx Configuration
- Nextcloud Installation
- Validation Phase