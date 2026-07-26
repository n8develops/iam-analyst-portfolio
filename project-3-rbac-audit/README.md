# Project 3: RBAC Entitlement Matrix & Access Audit

## Executive Summary
Simulated a 20-user, 5-department org and conducted a full access audit, identifying
4 access violations: 1 Separation of Duties violation, 2 instances of privilege creep,
and 1 orphaned account. Produced a formal audit report with risk ratings and a
remediation plan aligned to least-privilege principles.

## Objective
Simulate a real-world compliance review by auditing over-privileged users and enforcing
Role-Based Access Control (RBAC) across a simulated organization.

## Environment
- Simulated org: 20 user accounts across HR, Finance, Sales, Engineering, and IT
- Tooling: Google Sheets

## Approach

### 1. RBAC Matrix Design
- Mapped job titles per department to required application access and entitlements
- Defined Separation of Duties (SoD) rules
  - Example: Finance — a user cannot hold both *Invoice Creator* and *Invoice Approver*

### 2. Access Audit
- Generated a simulated access report listing all assigned permissions
- Compared actual access against the RBAC matrix to flag:
  - **Privilege creep** — users who changed departments but retained old access
  - **SoD violations** — conflicting permission pairs held by the same user
  - **Orphaned access** — terminated employees with access not yet revoked

### 3. Remediation Plan
- Documented actionable steps to strip unnecessary access and realign to least privilege
- Identified a systemic gap: manual offboarding/transfer processes allowed these
  violations to occur, recommended automated deprovisioning tied to HR status changes

## Key Findings
| Employee | Category | Risk |
|---|---|---|
| Kevin O'Brien | SoD Violation (Invoice Creator + Approver) | High |
| Sophia Marsh | Privilege Creep (retained Salesforce access post-transfer) | Medium |
| Hannah Kim | Orphaned Access (active 30 days post-termination) | High |
| Grace Nakamura | Privilege Creep / Stale HR Record | Medium |

Full findings, risk rationale, and remediation actions documented in the Audit Report.

## Deliverables
- [x] `docs/RBAC_Matrix.xlsx` — completed entitlement matrix and audit workbook
- [x] `docs/Access_Audit_Report.pdf` — formal findings + remediation plan

## Skills Demonstrated
RBAC design · Separation of Duties (SoD) · Privilege creep detection · Access governance ·
Compliance audit reporting · Least-privilege remediation planning · Risk assessment
