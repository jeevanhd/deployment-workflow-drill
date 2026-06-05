# Incident Log

This incident log highlights operational failures caused by the current uncontrolled deployment workflow.

## Recent incidents

### Incident 1: Bad deployment reached production
- **Date:** 2026-05-18
- **Summary:** A feature branch was deployed directly to production without proper validation.
- **Impact:** Checkout service returned incorrect totals for 30 minutes.
- **Root cause:** No deployment gate prevented direct pushes from non-release branches.

### Incident 2: Rollback delayed
- **Date:** 2026-05-12
- **Summary:** A failed release required rollback, but the team spent 45 minutes determining the rollback procedure.
- **Impact:** Extended customer downtime and increased investigation time.
- **Root cause:** There was no rollback playbook or pre-deployment readiness check.

### Incident 3: Validation skipped
- **Date:** 2026-04-29
- **Summary:** A release bypassed functional validation and shipped a broken checkout flow.
- **Impact:** Several orders failed and manual remediation was required.
- **Root cause:** The deployment process did not require validation gates or build verification.

### Incident 4: Wrong version released
- **Date:** 2026-04-01
- **Summary:** Production received the wrong version after manual deployment commands were executed.
- **Impact:** Confusion, rollback, and missing release notes.
- **Root cause:** No release movement documentation or enforced deployment sequence.

## Incident patterns

- Incidents are often caused by poor release discipline.
- The team lacks a consistent deployment workflow.
- Production readiness checks are missing.
- Communication and escalation are informal and reactive.
