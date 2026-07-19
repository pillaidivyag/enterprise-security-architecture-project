# Security Objectives

## Purpose

The purpose of this document is to define the security objectives for the enterprise Nextcloud deployment. These objectives guide the architecture, security controls, and validation activities throughout the project.

---

## Confidentiality

Ensure that business data is accessible only to authorised users.

Objectives:

- Encrypt all communication using HTTPS/TLS.
- Implement role-based access control (RBAC).
- Enforce strong authentication.
- Enable multi-factor authentication (MFA) for privileged accounts.
- Restrict administrative access.

---

## Integrity

Protect information from unauthorised modification.

Objectives:

- Maintain audit logs of administrative actions.
- Apply regular operating system and application updates.
- Validate uploaded files using antivirus scanning.
- Protect application and database configurations from unauthorised changes.

---

## Availability

Ensure that business services remain available when required.

Objectives:

- Perform scheduled backups.
- Monitor system health and service availability.
- Implement firewall protection against common attacks.
- Recover services quickly after failures.

---

## Authentication

Verify the identity of every user before access is granted.

Objectives:

- Enforce strong password policies.
- Enable MFA for administrators.
- Use secure session management.

---

## Authorisation

Limit user access according to business responsibilities.

Objectives:

- Apply the principle of least privilege.
- Separate administrative and standard user roles.
- Review permissions regularly.

---

## Monitoring

Provide sufficient visibility into security events.

Objectives:

- Log authentication events.
- Monitor administrative activities.
- Record application errors.
- Retain logs for investigation and auditing.

---

## Compliance

The solution aligns with recognised security best practices including:

- NIST Cybersecurity Framework
- CIS Controls
- OWASP Top 10
- ISO/IEC 27001 security principles