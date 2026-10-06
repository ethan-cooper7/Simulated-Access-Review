# Simulated Access Review - IAM Audit Lab


Created a simulated access review for 40 users across finance, HR, and IT, identified excessive &amp; outdated permissions, documented business justification and recommended least privilege changes.

## Environment

- 3 departments (Finance, HR, IT)
- 41 fictional users
- Role Based Access Control (RBAC)
- Security groups
- Application & systems access
- Privileged access
- User lifecycle management

## Objective
Evaluate user access against job responsibilities, identity, violations of least privilege, document security findings, and perform appropriate remediation.


## Project Data
> [!IMPORTANT]
> The following file contains the fictional organization's users, departments, security groups, and access assignments.
> - [Northstar Analytics Group](https://github.com/user-attachments/files/33109468/Northstar_Analytics_Group.xlsx)

Preview:
<img width="1560" height="547" alt="Finance" src="https://github.com/user-attachments/assets/be321654-da4e-4a81-96b7-f67b8e5b48dd" />



## Audit Findings

| Ticket | Finding | Severity | Status |
|---|---|---|---|
| IAM-001 | Expired contractor account | 🔴 Critical | Open |
| IAM-002 | Legacy department access | 🟠 High | Open |
| IAM-003 | Standard user with admin access | 🟠 High | Open |
| IAM-004 | Excessive HRIS access | 🟡 Medium | Open |
| IAM-005 | Help Desk admin privileges | 🟠 High | Open |
| IAM-006 | Unauthorized leadership group | 🟠 High | Open |
| IAM-007 | Missing account expiration | 🟡 Medium | Open |

## Remediation

- **IAM-001:** Daniel Adams is no longer a recruiter in HR. His account should not have any access. Best action is to disable his account.
- **IAM-002:** Ethan Robinson transferred to the IT department. He still has access to finance groups. Best action is to remove the finance groups and allow IT group access.
- **IAM-003:** Noah Williams, a finance staff accountant, has administrative access; this is excessive privilege. Best action is to remove the admin group.
- **IAM-004:** Lily Evans, the HR intern, has excessive HRIS access which can lead to sensitive data exposure. Best action is to restrict HRIS access.
- **IAM-005:** Grayson Howard has administrative access as a help desk technician. This is a privilege escalation issue. Best action is to remove the admin group and assign standard access.
- **IAM-006:** Amelia Young, procurement analyst, has an unauthorized leadership group. Best action is to remove the leadership group.
- **IAM-007:** Wyatt Gray is an IT intern. He is missing an account expiration for his internship end date. Best action is to set the expiration date on the account.

## Remediation Audit

| Ticket | Finding | Action | Status |
|---|---|---|---|
| IAM-001 | Expired contractor account | Disable account | Resolved |
| IAM-002 | Legacy department access | Remove finance groups | Resolved |
| IAM-003 | Standard user with admin access | Remove admin group | Resolved |
| IAM-004 | Excessive HRIS access | Restrict HRIS access | Resolved |
| IAM-005 | Help Desk admin privileges | Remove admin group | Resolved |
| IAM-006 | Unauthorized leadership group | Remove leadership group | Resolved |
| IAM-007 | Missing account expiration | Set expiration date | Resolved |
