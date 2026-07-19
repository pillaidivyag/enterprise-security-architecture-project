# Trust Boundaries

## Purpose

Trust boundaries identify where data moves between components with different security levels. These boundaries help determine where security controls should be applied.

---

## Trust Boundary 1

### Internet ↔ Nextcloud Web Server

Risk:

Traffic originates from untrusted networks.

Security Controls:

- HTTPS/TLS
- Nginx
- UFW Firewall
- Fail2Ban
- Secure HTTP headers

---

## Trust Boundary 2

### Web Server ↔ Nextcloud Application

Risk:

Application vulnerabilities could compromise the server.

Security Controls:

- Least privilege
- Secure file permissions
- PHP hardening
- Input validation

---

## Trust Boundary 3

### Nextcloud ↔ PostgreSQL

Risk:

Unauthorised database access.

Security Controls:

- Local database communication
- Database authentication
- Restricted database permissions

---

## Trust Boundary 4

### Administrator ↔ Server

Risk:

Privileged account compromise.

Security Controls:

- SSH hardening
- MFA (where available)
- Least privilege
- Audit logging

---

## Trust Boundary 5

### Backup Storage

Risk:

Exposure of backup data.

Security Controls:

- Backup encryption
- Restricted access
- Secure storage location