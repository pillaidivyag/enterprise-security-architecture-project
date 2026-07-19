## Purpose

The purpose of this risk assessment is to evaluate the security risks identified during the threat modelling phase and determine their potential impact on the proposed Nextcloud Enterprise deployment.

The assessment helps prioritise security improvements before the solution is deployed into production and supports risk-based decision making by identifying which risks require immediate mitigation and which can be accepted or monitored.

## Scope

This assessment covers the components included within the proposed enterprise architecture, including:

- External users
- Internal employees
- Identity Provider (SSO and MFA)
- Reverse Proxy / Web Application Firewall
- Nextcloud application
- PostgreSQL database
- File storage
- Logging and monitoring platform
- Backup infrastructure
- Network communications between system components

The assessment focuses on risks associated with confidentiality, integrity and availability of business information.

## Assessment Process

The assessment was completed using the following process:

1. Review the proposed enterprise architecture.
2. Analyse system components, data flows and trust boundaries.
3. Identify potential threats using the STRIDE methodology.
4. Assess the likelihood of each threat occurring.
5. Assess the potential business impact if the threat were realised.
6. Calculate an overall risk rating using the defined risk matrix.
7. Prioritise risks based on their severity.
8. Recommend appropriate security controls to reduce identified risks.
9. Record residual risks after proposed mitigations.

This structured approach ensures that risks are evaluated consistently across the entire architecture.

## Likelihood Scale

| Score | Description    |
| ----- | -------------- |
| 1     | Rare           |
| 2     | Unlikely       |
| 3     | Possible       |
| 4     | Likely         |
| 5     | Almost Certain |

## Impact Scale

| Score | Description |
| ----- | ----------- |
| 1     | Negligible  |
| 2     | Minor       |
| 3     | Moderate    |
| 4     | Major       |
| 5     | Critical    |

## Risk Calculation
   
    Likelihood × Impact

## Risk scores are classified as:

| Score | Risk Level |
|------|------------|
| 1–5 | Low |
| 6–10 | Medium |
| 11–15 | High |
| 16–25 | Critical |

## Risk Acceptance Criteria

The organisation applies a risk-based approach when determining whether a risk is acceptable.

- **Low risks** may be accepted and monitored through normal operational processes.
- **Medium risks** require planned mitigation and periodic review.
- **High risks** should be reduced through appropriate security controls before production deployment.
- **Critical risks** are considered unacceptable and must be addressed before the solution is approved for production.

Where a risk cannot be fully mitigated, it should be formally accepted by the appropriate business owner after reviewing the potential business impact and any remaining residual risk.

---

## Review Process

Risk assessments should not be treated as a one-time activity. The assessment should be reviewed whenever significant changes occur within the environment.

Examples include:

- Major application upgrades
- Changes to system architecture
- Introduction of new integrations
- Deployment of new infrastructure
- Discovery of critical vulnerabilities
- Significant security incidents
- Changes to business or regulatory requirements

In addition, a formal review should be carried out at least annually to ensure the assessment remains accurate and reflects the current security posture of the environment.

