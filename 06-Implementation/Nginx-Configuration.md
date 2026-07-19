# Nginx Configuration

## Purpose

This document records the installation and configuration of Nginx as the web server for the Nextcloud deployment.

---

## Installation

Nginx was installed using the Ubuntu package manager and configured to run as the front-end web server for the application.

---

## Configuration

The following activities were completed:

- Installed Nginx.
- Verified the Nginx service was running.
- Enabled automatic startup.
- Validated the default configuration.
- Confirmed the default web page was accessible.
- Created a dedicated Nginx server block for Nextcloud.
- Configured PHP-FPM integration.
- Updated the document root.
- Enabled the Nextcloud site.
- Disabled the default Nginx site.
- Validated the Nginx configuration.
- Reloaded the Nginx service.

---

## Security Considerations

The web server was configured to:

- Restrict access to hidden files.
- Process PHP requests through PHP-FPM.
- Limit client upload size to support Nextcloud.

HTTPS configuration is documented separately.

---

## Outcome

Nginx was successfully configured to serve the Nextcloud application.
