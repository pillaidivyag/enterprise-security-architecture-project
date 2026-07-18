# Identity and Access Management

## Purpose

Identity and Access Management (IAM) ensures that only authorised users can access enterprise resources while preventing excessive privileges and unauthorised access.

Identity security is considered one of the highest priorities because credential compromise represents one of the highest risks identified during the assessment.

---

# Objectives

The IAM design aims to:

- Verify user identities before granting access
- Apply least privilege access
- Protect privileged accounts
- Support secure remote access
- Reduce the risk of credential compromise

---

# Recommended Controls

## Single Sign-On (SSO)

Nextcloud should integrate with the enterprise Identity Provider using OpenID Connect (OIDC) or SAML.

Benefits include:

- Centralised authentication
- Reduced password fatigue
- Consistent access policies
- Simplified user management

---

## Multi-Factor Authentication (MFA)

MFA should be mandatory for:

- All administrators
- Remote users
- External partners
- Privileged accounts

Accepted factors may include:

- Authenticator application
- Hardware security key
- Push notification

SMS should not be used unless no stronger option is available.

---

## Role-Based Access Control (RBAC)

Users should receive permissions based on their business role rather than individual assignment.

Example roles include:

| Role | Permissions |
|------|-------------|
| Employee | Standard file access |
| Project Manager | Team collaboration and file sharing |
| External Partner | Restricted project folder access |
| Administrator | Platform administration |
| Security Administrator | Audit and security management |

---

## Least Privilege

Users should only receive access required to perform their job responsibilities.

Permissions should be reviewed regularly to identify unnecessary access.

---

## Privileged Access Management

Administrative accounts should be separated from normal user accounts.

Recommendations include:

- Dedicated administrator accounts
- No shared administrator credentials
- Administrative actions logged
- Privileged access reviewed regularly

---

## Password Policy

The Identity Provider should enforce password requirements including:

- Minimum length
- Password history
- Protection against compromised passwords
- Account lockout after repeated failures

Users should not reuse passwords across systems.

---

## Session Management

Authentication sessions should be protected through:

- Secure session cookies
- Automatic session timeout
- Re-authentication for sensitive actions
- Session invalidation after logout

---

## Joiner, Mover and Leaver Process

User access should follow the organisation's identity lifecycle.

### Joiner

- Create account
- Assign appropriate role
- Enable MFA

### Mover

- Update permissions
- Remove unnecessary access
- Review privileged roles

### Leaver

- Disable account immediately
- Remove group memberships
- Revoke active sessions

---

## Access Reviews

Periodic access reviews should verify:

- User permissions remain appropriate
- Dormant accounts are removed
- Privileged access remains justified

Recommended frequency:

- Quarterly for privileged accounts
- Annually for standard users

---

## Risks Addressed

The controls within this document reduce the following risks:

- Credential compromise
- Privilege escalation
- Unauthorised access
- Excessive permissions
- Insider threats

---

## Summary

A strong identity and access management solution forms the foundation of the proposed security architecture by ensuring users receive only the access required while protecting authentication processes through centralised identity management and multi-factor authentication.