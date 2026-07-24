# Project 1: Automated JML Lifecycle Framework

**Status:** Not started — scheduled for Week 3

## Objective
Eliminate manual admin tasks by automating user onboarding, offboarding, and departmental
transfers using Microsoft Graph API (or Okta API).

## Planned Deliverables
- [ ] `scripts/joiner.ps1` (or `.py`) — parses HR feed payload, provisions user, assigns groups
- [ ] `scripts/mover.ps1` — detects department/title changes, re-scopes group entitlements
- [ ] `scripts/leaver.ps1` — disables account, revokes OAuth tokens, strips groups, logs event
- [ ] `docs/Architecture.png` — API workflow diagram
- [ ] Screenshots of Entra ID audit log showing automated provisioning/revocation

## Security Note
No client secrets, tenant IDs, or credentials will be committed. All scripts sanitized before publishing.
