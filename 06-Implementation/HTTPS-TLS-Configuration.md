# HTTPS TLS Configuration

## Purpose

This document describes the implementation of HTTPS encryption for the Nextcloud deployment.

TLS was enabled to protect communication between users and the Nextcloud application by encrypting data transmitted over the network.

---

## Certificate Implementation

A self-signed TLS certificate was generated for the internal lab environment.

The certificate approach was selected because:

- The environment is private and not publicly accessible.
- No production domain name is configured.
- The implementation demonstrates TLS configuration and encrypted communication.

In a production environment, the certificate would be replaced with a certificate issued by a trusted Certificate Authority.

---

## Nginx Configuration

The following TLS configurations were implemented:

- Enabled HTTPS listener on port 443.
- Configured TLS certificate and private key.
- Enabled TLS 1.2 and TLS 1.3 protocols.
- Redirected HTTP traffic from port 80 to HTTPS.
- Maintained secure access through Nginx reverse proxy.

---

## Firewall Configuration

Firewall rules were updated to allow required services:

- SSH (22/tcp)
- HTTP redirect (80/tcp)
- HTTPS encrypted traffic (443/tcp)

---

## Validation

The following checks were performed:

- Confirmed Nginx was listening on HTTPS port 443.
- Confirmed HTTPS access from client browser.
- Verified encrypted access to the Nextcloud application.
- Confirmed HTTP requests redirect to HTTPS.

---

## Outcome

HTTPS was successfully implemented for the Nextcloud deployment.

Client communication is now encrypted using TLS, providing confidentiality and protection against network interception.