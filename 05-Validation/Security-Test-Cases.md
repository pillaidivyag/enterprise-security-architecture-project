# Security Test Cases

## Purpose

This document defines the security test cases used to verify that the recommended security controls operate as intended.

The test cases cover authentication, authorisation, data protection, network security, application security, logging and resilience.

---

# Test Execution

Each test should include:

- Test ID
- Objective
- Test procedure
- Expected result
- Actual result
- Status
- Tester
- Test date

---

# Security Test Cases

| Test ID | Control Area | Test Description | Expected Result |
|----------|--------------|------------------|-----------------|
| TC-001 | Authentication | Attempt login using valid credentials | Login successful |
| TC-002 | MFA | Attempt login without completing MFA | Access denied |
| TC-003 | RBAC | User attempts to access restricted folder | Access denied |
| TC-004 | Session Management | Leave session idle beyond timeout | Session automatically expires |
| TC-005 | Password Policy | Attempt weak password | Password rejected |
| TC-006 | HTTPS | Access application using HTTP | Redirected to HTTPS |
| TC-007 | TLS | Verify TLS configuration | TLS 1.2 or higher in use |
| TC-008 | File Upload | Upload unsupported executable file | Upload rejected |
| TC-009 | Malware Protection | Upload EICAR test file | File detected or quarantined |
| TC-010 | WAF | Submit SQL injection payload | Request blocked |
| TC-011 | WAF | Submit Cross-Site Scripting (XSS) payload | Request blocked |
| TC-012 | Logging | Delete a file | Audit log generated |
| TC-013 | Logging | Administrator changes permissions | Event recorded |
| TC-014 | SIEM | Generate failed login attempts | Alert visible in SIEM |
| TC-015 | Backup | Restore selected file | File successfully restored |
| TC-016 | Disaster Recovery | Verify recovery documentation | Documentation complete and accessible |

---

# Test Status

Each test should be assigned one of the following statuses:

| Status | Meaning |
|---------|---------|
| Passed | Expected behaviour observed |
| Failed | Expected behaviour not observed |
| Blocked | Test could not be completed |
| Not Executed | Test not yet performed |

---

# Evidence Collection

Evidence may include:

- Screenshots
- Log entries
- SIEM alerts
- Configuration screenshots
- Scan reports
- Recovery reports

---

# Summary

These security test cases provide a structured approach for validating that the proposed security architecture performs as expected and supports the organisation's security requirements.