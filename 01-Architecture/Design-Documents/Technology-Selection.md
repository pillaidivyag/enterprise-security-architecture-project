# Technology Selection

## Purpose

This document explains the technologies selected for the project and the reasons for each decision.

---

## Operating System

### Ubuntu Server LTS

Reason for selection:

- Long-term support
- Regular security updates
- Strong community support
- Widely used in enterprise environments

---

## Application

### Nextcloud

Reason for selection:

- Open-source
- Self-hosted
- Enterprise features
- Strong security capabilities
- Supports MFA and encryption

---

## Web Server

### Nginx

Reason for selection:

- High performance
- Reverse proxy support
- SSL/TLS support
- Secure default configuration
- Efficient resource usage

---

## Database

### PostgreSQL

Reason for selection:

- Enterprise-grade database
- Reliability
- ACID compliance
- Strong security model
- Excellent performance

---

## Firewall

### UFW

Reason for selection:

- Simple management
- Integrated with Ubuntu
- Suitable for host-based firewall protection

---

## Intrusion Prevention

### Fail2Ban

Reason for selection:

- Detects repeated failed logins
- Automatically blocks malicious IP addresses
- Lightweight and widely adopted

---

## Encryption

### TLS 1.2 / TLS 1.3

Reason for selection:

- Protects data in transit
- Industry standard
- Supported by modern browsers

---

## Validation Tools

| Tool | Purpose |
|-------|----------|
| Nmap | Network discovery and port scanning |
| OWASP ZAP | Web application security testing |
| Nikto | Web server vulnerability assessment |
| Lynis | Operating system security auditing |

---

## Selection Summary

The selected technologies are open source, widely adopted, well documented, and suitable for demonstrating enterprise security architecture principles while remaining practical for a lab environment.