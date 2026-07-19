# Nextcloud Installation

## Purpose

This document records the installation of the Nextcloud application within the Ubuntu environment.

Nextcloud provides the secure file storage and collaboration platform used throughout this project.

---

## Installation

The latest stable Nextcloud release was downloaded from the official project repository and deployed to the web server directory.

Application ownership and file permissions were configured to allow secure operation by the Nginx web server.

---

## Configuration

The following activities were completed:

- Downloaded the latest stable Nextcloud release.
- Extracted the application files.
- Deployed the application to the web server directory.
- Assigned ownership to the web server account.
- Applied secure file and directory permissions.

---

## Security Considerations

The application was deployed using the Principle of Least Privilege.

Only the web server service account was granted ownership of the application files, reducing the risk of unauthorised local access.

Additional application configuration will be completed during the Nginx and HTTPS configuration stages.

---

## Outcome

The Nextcloud application has been successfully deployed and is ready for web server configuration.