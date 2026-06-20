# Department Transfer Access Change

This document shows an IAM workflow for updating user access when an employee changes roles or departments.

## Scenario

An employee is moving from the Sales department to the Finance department. Their access needs to be reviewed so unnecessary permissions are removed and new required access is approved.

## Employee Information

| Field              | Details           |
| ------------------ | ----------------- |
| Employee Name      | Alex Rivera       |
| Current Department | Sales             |
| New Department     | Finance           |
| Current Job Title  | Sales Coordinator |
| New Job Title      | Finance Assistant |
| Effective Date     | 2026-07-13        |
| Manager            | Jordan Lee        |
| Employment Type    | Full-time         |

## Access to Remove

| System                    | Current Access      | Reason for Removal                        |
| ------------------------- | ------------------- | ----------------------------------------- |
| CRM                       | Sales user          | No longer part of Sales department        |
| Sales Shared Drive        | Sales folder access | No longer needs Sales documents           |
| Sales Reporting Dashboard | Standard user       | No longer responsible for Sales reporting |

## Access to Add

| System                  | Requested Access       | Business Reason                     | Approval Required              |
| ----------------------- | ---------------------- | ----------------------------------- | ------------------------------ |
| Finance Shared Drive    | Finance folder access  | Required for Finance documents      | Manager                        |
| Finance System          | Finance assistant role | Required for invoice support tasks  | Manager + Finance System Owner |
| Expense Management Tool | Standard user          | Required for expense review support | Manager                        |

## IAM Review

| Review Item                 | Status                        |
| --------------------------- | ----------------------------- |
| Old access reviewed         | Complete                      |
| Unneeded access removed     | Required                      |
| New access approved         | Pending system owner approval |
| Privileged access requested | No                            |
| Least privilege followed    | Yes                           |
| MFA still required          | Yes                           |

## Access Change Steps

1. Confirm department transfer with manager.
2. Review current group memberships and application access.
3. Remove Sales-related access.
4. Add Finance department group access.
5. Request Finance System owner approval.
6. Apply approved Finance System role.
7. Confirm access changes with the new manager.
8. Document all removals and additions.

## Notes

This is a fictional IAM lab example. No real employee, company, or credential information is included.
