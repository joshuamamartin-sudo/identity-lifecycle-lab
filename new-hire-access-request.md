# New Hire Access Request

This document shows a basic IAM access request workflow for a fictional new employee.

## Scenario

A new employee is joining the company and needs access to the systems required for their role. Access should be approved before provisioning and should follow least privilege.

## Employee Information

| Field           | Details         |
| --------------- | --------------- |
| Employee Name   | Maya Chen       |
| Department      | Finance         |
| Job Title       | Finance Analyst |
| Start Date      | 2026-07-06      |
| Manager         | Jordan Lee      |
| Employment Type | Full-time       |
| Location        | Remote          |

## Requested Access

| System         | Access Level              | Business Reason                         | Approval Required              |
| -------------- | ------------------------- | --------------------------------------- | ------------------------------ |
| Company Email  | Standard user             | Required for communication              | Manager                        |
| HR Portal      | Employee self-service     | Required for payroll and benefits       | Manager                        |
| Finance System | Finance analyst role      | Required for invoice and reporting work | Manager + Finance System Owner |
| Shared Drive   | Finance department folder | Required for department documents       | Manager                        |
| VPN            | Standard remote access    | Required for remote work                | IT/Security                    |

## IAM Review

| Review Item                    | Status                  |
| ------------------------------ | ----------------------- |
| Access matches job role        | Approved                |
| Privileged access requested    | No                      |
| MFA required                   | Yes                     |
| Manager approval received      | Yes                     |
| System owner approval required | Yes, for Finance System |
| Least privilege followed       | Yes                     |

## Provisioning Steps

1. Create user account.
2. Assign standard employee access.
3. Add user to Finance department group.
4. Assign Finance System role after system owner approval.
5. Require MFA setup during first login.
6. Confirm access with manager.
7. Document completion in the access request record.

## Notes

This is a fictional IAM lab example. No real employee or company information is included.
