# Offboarding Checklist

This document shows a basic IAM offboarding workflow for removing access when an employee leaves the company.

## Scenario

An employee is leaving the company. Their access must be disabled or removed on time to reduce security risk.

## Employee Information

| Field            | Details            |
| ---------------- | ------------------ |
| Employee Name    | Riley Morgan       |
| Department       | Finance            |
| Job Title        | Finance Analyst    |
| Last Working Day | 2026-07-24         |
| Manager          | Jordan Lee         |
| Employment Type  | Full-time          |
| Offboarding Type | Standard departure |

## Offboarding Checklist

| Task                                   | Owner        | Status   |
| -------------------------------------- | ------------ | -------- |
| Confirm last working day with manager  | HR           | Complete |
| Disable user account                   | IT/IAM       | Pending  |
| Revoke VPN access                      | IT/IAM       | Pending  |
| Remove application access              | IT/IAM       | Pending  |
| Remove shared drive access             | IT/IAM       | Pending  |
| Remove group memberships               | IT/IAM       | Pending  |
| Transfer file ownership if needed      | Manager + IT | Pending  |
| Revoke MFA methods and active sessions | IT/IAM       | Pending  |
| Confirm no privileged access remains   | IT/IAM       | Pending  |
| Document completion                    | IT/IAM       | Pending  |

## Access to Remove

| System                  | Access Type            | Removal Action                                  |
| ----------------------- | ---------------------- | ----------------------------------------------- |
| Company Email           | Standard user          | Disable account or convert per retention policy |
| Finance System          | Finance analyst role   | Remove application role                         |
| Shared Drive            | Finance folder access  | Remove group membership                         |
| VPN                     | Standard remote access | Revoke access                                   |
| HR Portal               | Employee self-service  | Disable or remove access                        |
| Expense Management Tool | Standard user          | Remove application access                       |

## IAM Review

| Review Item                 | Status   |
| --------------------------- | -------- |
| Manager confirmed departure | Complete |
| HR record confirmed         | Complete |
| Privileged access found     | No       |
| Shared accounts used        | No       |
| Access removal documented   | Pending  |
| Completion confirmed        | Pending  |

## Offboarding Steps

1. Confirm departure date with HR and manager.
2. Review all assigned groups, roles, and applications.
3. Disable the primary user account at the required time.
4. Revoke remote access and active sessions.
5. Remove application roles and group memberships.
6. Confirm no privileged access remains.
7. Document all completed access removal actions.
8. Notify manager when offboarding is complete.

## Notes

This is a fictional IAM lab example. No real employee, company, or credential information is included.
