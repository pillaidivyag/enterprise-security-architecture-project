# PostgreSQL Configuration

## Purpose

This document records the installation and initial configuration of PostgreSQL as the backend database for the Nextcloud environment.

---

## Installation

PostgreSQL was installed using the Ubuntu package manager.

Key command:

```bash
sudo apt install postgresql postgresql-contrib
```

---

## Configuration

The following tasks were completed:

- Verified the PostgreSQL service was running.
- Enabled automatic service startup.
- Created a dedicated database for Nextcloud.
- Created a dedicated database user.
- Granted the required permissions to the application user.

Using a dedicated database account instead of the default PostgreSQL administrator follows the Principle of Least Privilege.

---

## Planned Hardening

Additional security configuration will be completed later in the project, including:

- Restricting remote database access.
- Reviewing authentication settings.
- Enabling database logging.
- Verifying file permissions.

---

## Outcome

PostgreSQL has been successfully installed and configured as the backend database for the Nextcloud deployment.