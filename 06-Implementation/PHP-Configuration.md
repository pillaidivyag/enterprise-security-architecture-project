# PHP Configuration

## Purpose

This document records the installation and initial configuration of PHP for the Nextcloud deployment.

PHP provides the runtime environment required for the Nextcloud application.

---

## Installation

The required PHP packages and extensions were installed to support Nextcloud and PostgreSQL.

The PHP FastCGI Process Manager (PHP-FPM) was configured as the application runtime.

---

## Configuration

The following activities were completed:

- Installed PHP and required extensions.
- Verified the PHP installation.
- Verified the PHP-FPM service was running.
- Enabled the PHP-FPM service to start automatically after system boot.

---

## Planned Configuration

Additional PHP configuration will be completed during the Nextcloud deployment, including:

- Memory limit optimisation
- Maximum upload file size
- Maximum execution time
- Performance tuning

---

## Outcome

PHP has been successfully installed and configured. The environment is ready for Nginx integration and Nextcloud deployment.