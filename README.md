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




## Audit Findings

| Ticket | Finding | Severity | Status |
|---|---|---|---|
| [IAM-001](tickets/IAM-001-Expired-Contractor.md) | Expired contractor account | 🔴 Critical | Open |
| [IAM-002](tickets/IAM-002-Department-Transfer.md) | Legacy department access | 🟠 High | Open |
| [IAM-003](tickets/IAM-003-Excessive-Privileges.md) | Standard user with admin access | 🟠 High | Open |
| [IAM-004](tickets/IAM-004-Intern-Access.md) | Excessive HRIS access | 🟡 Medium | Open |
| [IAM-005](tickets/IAM-005-Endpoint-Admin.md) | Help Desk admin privileges | 🟠 High | Open |
| [IAM-006](tickets/IAM-006-Leadership-Access.md) | Unauthorized leadership group | 🟠 High | Open |
| [IAM-007](tickets/IAM-007-Missing-Expiration.md) | Missing account expiration | 🟡 Medium | Open |
