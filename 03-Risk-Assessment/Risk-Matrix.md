## Overview

This document defines the risk scoring methodology used during the security assessment of the Nextcloud Enterprise deployment.

Each identified risk has been evaluated based on:

- Likelihood of occurrence
- Business impact
- Overall risk rating

The purpose of the matrix is to prioritise remediation activities and support risk-based security decisions before production deployment.

---

# Risk Assessment Method

Overall Risk Score = Likelihood × Impact

Likelihood is scored from 1 (Rare) to 5 (Almost Certain).

Impact is scored from 1 (Negligible) to 5 (Critical).

The resulting score determines the overall risk level.

---

# Likelihood Scale

| Score | Rating | Description |
|------|---------|-------------|
| 1 | Rare | Highly unlikely to occur. Requires exceptional circumstances. |
| 2 | Unlikely | Could occur but has not been observed in similar environments. |
| 3 | Possible | Could reasonably occur during normal operations. |
| 4 | Likely | Expected to occur without appropriate security controls. |
| 5 | Almost Certain | Expected to occur frequently or is highly probable. |

---

# Impact Scale

| Score | Rating | Description |
|------|---------|-------------|
| 1 | Negligible | Minimal operational impact with no significant business consequences. |
| 2 | Minor | Limited disruption affecting a small number of users or services. |
| 3 | Moderate | Noticeable business disruption or limited exposure of sensitive information. |
| 4 | Major | Significant operational impact, financial loss, or regulatory implications. |
| 5 | Critical | Severe business disruption, large-scale data compromise, or prolonged service outage. |

---

# Risk Rating

| Score | Risk Level | Required Action |
|------|------------|----------------|
| 1–5 | Low | Accept or monitor. |
| 6–10 | Medium | Plan and implement mitigation. |
| 11–15 | High | Mitigate before production deployment. |
| 16–25 | Critical | Immediate action required. Deployment should not proceed until risk is reduced. |

---

# Risk Matrix

| Likelihood \\ Impact | 1 | 2 | 3 | 4 | 5 |
|----------------------|---|---|---|---|---|
| **5 – Almost Certain** | Low | Medium | High | Critical | Critical |
| **4 – Likely** | Low | Medium | High | High | Critical |
| **3 – Possible** | Low | Medium | Medium | High | High |
| **2 – Unlikely** | Low | Low | Medium | Medium | High |
| **1 – Rare** | Low | Low | Low | Medium | Medium |

---

# Risk Distribution

The identified risks are distributed as follows:

| Risk Level | Number of Risks |
|------------|----------------|
| Critical | 2 |
| High | 6 |
| Medium | 3 |
| Low | 1 |

---

# Risks Mapped to the Matrix

| Risk ID | Description | Likelihood | Impact | Score | Risk Level |
|---------|-------------|------------|---------|-------|------------|
| R-001 | Compromised user credentials | 4 | 5 | 20 | Critical |
| R-002 | Authentication token manipulation | 3 | 5 | 15 | High |
| R-003 | Application vulnerability exploitation | 3 | 5 | 15 | High |
| R-004 | Unauthorised access to business documents | 4 | 5 | 20 | Critical |
| R-005 | Unauthorised modification of documents | 3 | 4 | 12 | High |
| R-006 | Database compromise | 2 | 5 | 10 | Medium |
| R-007 | Excessive database privileges | 3 | 5 | 15 | High |
| R-008 | Web application attack | 3 | 4 | 12 | High |
| R-009 | Log manipulation | 3 | 4 | 12 | High |
| R-010 | Monitoring failure | 3 | 3 | 9 | Medium |
| R-011 | Backup data exposure | 2 | 5 | 10 | Medium |
| R-012 | Service disruption | 2 | 4 | 8 | Medium |

---

# Risk Acceptance Criteria

The organisation's risk appetite is defined as follows:

- Low risks may be accepted and reviewed periodically.
- Medium risks require planned mitigation and monitoring.
- High risks must be mitigated before production deployment.
- Critical risks require immediate remediation and management approval before deployment.

---

# Summary

The assessment identified identity compromise and unauthorised access to business documents as the highest priority risks.

These risks will be addressed through security controls including Multi-Factor Authentication (MFA), Role-Based Access Control (RBAC), secure authentication protocols, network segmentation, centralised logging, and continuous monitoring.

The Risk Register and Risk Treatment Plan provide detailed mitigation activities for each identified risk.