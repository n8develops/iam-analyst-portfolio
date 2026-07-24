# Project 3: RBAC Entitlement Matrix & Access Audit

## Executive Summary
> _Fill in after completion: 2-3 sentences on what you built and the key finding._
> Example: "Simulated a 20-user, 4-department org and conducted a full access audit,
> identifying N instances of privilege creep and N SoD violations, then produced a
> formal remediation plan aligned to least-privilege principles."

## Objective
Simulate a real-world compliance review by auditing over-privileged users and enforcing
Role-Based Access Control (RBAC) across a simulated organization.

## Environment
- Simulated org: 15–20 user accounts across HR, Engineering, Finance, Sales
- Tooling: Excel / Google Sheets

## Approach

### 1. RBAC Matrix Design
- Mapped job titles per department to required application access and entitlements
- Defined Separation of Duties (SoD) rules
  - Example: Finance — a user cannot hold both *Invoice Creator* and *Invoice Approver*

### 2. Access Audit
- Generated a simulated access report listing all assigned permissions
- Flagged:
  - **Privilege creep** — users who changed departments but retained old access
  - **SoD violations** — conflicting permission pairs held by the same user

### 3. Remediation Plan
- Documented actionable steps to strip unnecessary access and realign to least privilege

## Key Findings
> _Fill in after the audit — e.g. number of flagged accounts, most common violation type._

## Deliverables
- [ ] `docs/RBAC_Matrix.xlsx` — completed entitlement matrix
- [ ] `docs/Access_Audit_Report.pdf` — formal findings + remediation plan (2 pages)

## Skills Demonstrated
RBAC design · Separation of Duties (SoD) · Privilege creep detection · Access governance ·
Compliance audit reporting · Least-privilege remediation planning
