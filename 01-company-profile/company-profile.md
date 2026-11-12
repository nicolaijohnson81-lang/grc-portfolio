# Company Profile: Meridian Ledger (Fictional)

> **Note:** Meridian Ledger is a fictional company created for this portfolio. Any resemblance to a real organization is coincidental.

## Business Overview

| Item | Detail |
|---|---|
| Industry | Payroll & employee-benefits SaaS |
| HQ | New York, NY (hybrid; 1 office + remote staff in 6 states) |
| Employees | ~150 full-time + ~20 contractors |
| Customers | ~400 small and mid-sized businesses (roughly 60,000 of their employees in the platform) |
| Revenue | ~$28M ARR, growing ~35% year over year |
| Stage | Series B; preparing for first SOC 2 Type II audit |

## What Meridian Does

Small businesses use Meridian to run payroll, manage health and retirement benefits enrollment, and store employee records. That means Meridian holds sensitive data for people who are **not** its own employees: its customers' workers.

## Data Handled

| Data Type | Examples | Sensitivity |
|---|---|---|
| PII | Names, addresses, SSNs, dates of birth | High |
| Financial | Bank account and routing numbers for direct deposit, salaries | High |
| Health-related | Benefits elections, dependent info, some plan claims data | High (HIPAA-relevant) |
| Customer business data | Company tax IDs, payroll schedules | Medium |
| Internal | Source code, contracts, HR records | Medium |

## Technology Environment

| Area | System |
|---|---|
| Identity / SSO | Microsoft Entra ID |
| Productivity | Microsoft 365 (Exchange, SharePoint, Teams) |
| Production hosting | AWS (EC2, RDS PostgreSQL, S3) |
| Source code | GitHub (cloud) |
| CRM / Support | Salesforce, Zendesk |
| Endpoints | ~170 laptops (mix of Windows and macOS) |
| Payments | Third-party ACH processor via API |

## Regulatory & Contractual Drivers

- **SOC 2 Type II**: enterprise prospects now require it before signing
- **HIPAA**: acts as a Business Associate for benefits-related health data
- **NY SHIELD Act**: reasonable security safeguards for NY residents' private data
- **Customer contracts**: security questionnaires and breach-notification clauses

## Current Security Situation (Starting Point)

Meridian grew quickly and security has been handled informally by a 4-person IT/DevOps team. No dedicated security or GRC staff. Known issues leadership has mentioned:

- No formal risk register; risks are discussed in Slack but never tracked
- MFA is enforced for employees but **not** for contractors
- Offboarding is a manual help-desk ticket; access removal is sometimes delayed by days
- An incident response plan exists as a 2-page doc from 2023 that has never been tested
- Vendor security reviews happen only when a customer asks
- Backups run nightly, but restores have never been tested
- No security awareness training program

## Why This Company

<!-- TODO (Nicolai): In 2-3 sentences, explain why you chose this scenario and what it lets you demonstrate. Write this yourself — it's your interview talking point. -->
