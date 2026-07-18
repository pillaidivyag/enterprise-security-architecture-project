# Data Protection

## Purpose

The purpose of this document is to define the controls required to protect business information stored and processed by the Nextcloud platform.

The recommended controls aim to preserve the confidentiality, integrity and availability of organisational data throughout its lifecycle.

---

# Objectives

The data protection strategy aims to:

- Protect sensitive business information
- Prevent unauthorised disclosure
- Maintain data integrity
- Support regulatory compliance
- Ensure secure recovery following incidents

---

# Data Classification

Information should be classified according to business sensitivity.

| Classification | Example |
|---------------|---------|
| Public | Marketing material |
| Internal | Internal procedures |
| Confidential | Business documents |
| Restricted | Financial and engineering data |

Security controls should increase according to classification.

---

# Encryption in Transit

All communications between users and the platform should use TLS 1.2 or higher.

Encryption should protect:

- User authentication
- File uploads
- File downloads
- API communications
- Administrative sessions

---

# Encryption at Rest

Business documents should be encrypted while stored.

Recommended locations include:

- File storage
- Database storage
- Backup repositories

Encryption keys should be managed separately from encrypted data.

---

# Key Management

Encryption keys should:

- Be securely generated
- Be stored separately
- Be rotated periodically
- Be accessible only by authorised administrators

---

# File Permissions

Access to files should follow least privilege.

Controls include:

- Folder ownership
- Role-based permissions
- Controlled external sharing
- Expiring sharing links

---

# Backup Protection

Backups should:

- Be encrypted
- Be stored separately
- Be protected by restricted access
- Be tested regularly

Backup integrity should be verified after creation.

---

# Data Retention

Retention periods should align with business and regulatory requirements.

Expired information should be securely removed.

---

# Secure Deletion

Deleted information should not remain recoverable beyond the defined retention period.

Storage media should follow secure sanitisation procedures before disposal.

---

# Risks Addressed

These controls reduce risks including:

- Information disclosure
- Data tampering
- Backup compromise
- Data loss
- Regulatory non-compliance

---

# Summary

The proposed controls protect business information throughout its lifecycle using encryption, access controls, secure backups and data governance practices. Together they help ensure organisational information remains confidential, accurate and available when required.