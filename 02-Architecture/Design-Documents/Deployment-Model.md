# Deployment Model

## Overview

The solution is deployed using a three-tier architecture consisting of presentation, application, and database layers. This separation improves security, scalability, and maintainability.

---

## Components

### Client Layer

Users access the application through a web browser over HTTPS.

Examples:

- Employee laptops
- Corporate desktops
- Mobile devices

---

### Application Layer

Ubuntu Server hosts the following services:

- Nginx
- PHP-FPM
- Nextcloud
- Fail2Ban
- UFW Firewall

Responsibilities include:

- User authentication
- File management
- Application processing
- Logging

---

### Database Layer

PostgreSQL stores:

- User accounts
- File metadata
- Application settings
- Audit information

The database accepts connections only from the application server.

---

## Network Design

Communication flow:

Client

↓

HTTPS (443)

↓

Nginx Reverse Proxy

↓

PHP-FPM

↓

Nextcloud

↓

PostgreSQL

---

## Security Design Principles

The deployment follows several security principles:

- Defence in depth
- Least privilege
- Secure by default
- Network segmentation
- Encryption in transit
- Secure administration

---

## Future Scalability

The architecture supports future enhancements including:

- Load balancing
- Multiple application servers
- External object storage
- Centralised logging
- High availability database clusters