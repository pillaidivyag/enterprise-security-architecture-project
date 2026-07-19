# Nextcloud Configuration

## Purpose

This document records the deployment and initial configuration of the Nextcloud application.

---

## Installation

Nextcloud was deployed on the Ubuntu environment using Nginx as the web server, PHP-FPM as the application runtime, and PostgreSQL as the backend database.

---

## Configuration

The following activities were completed:

- Installed Nextcloud application files.
- Configured PostgreSQL database connectivity.
- Created an administrative account.
- Verified successful application startup.
- Verified access through the web interface.

---

## Security Considerations

The deployment uses:

- Dedicated PostgreSQL database account.
- Web server ownership of application files.
- Separate application and database layers.

Additional security hardening will be completed in later phases.

---

## Outcome

Nextcloud was successfully deployed and is operational within the lab environment.