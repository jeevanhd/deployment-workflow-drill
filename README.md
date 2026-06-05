# Controlled Deployment Workflow Lab

## Overview

This lab simulates a checkout service team that has operated without a controlled deployment workflow for months.

Deployments are currently chaotic and risky:

- Any developer can deploy directly to production
- No approvals are required
- No validation gates are implemented
- No rollback preparation exists
- No health or post-deployment validation is recorded
- No operational visibility or release movement documentation exists

You are the Deployment Workflow Auditor. Your goal is analyze the current process, document weaknesses, and design a controlled deployment workflow that protects release quality.

## Student Tasks

Complete the following deliverables in this repository:

1. `DEPLOYMENT-AUDIT.md`
   - Identify at least 5 workflow weaknesses
   - Provide evidence, risk, and control recommendations

2. `DEPLOYMENT-WORKFLOW.md`
   - Design a controlled release workflow that includes:
     - Validation phase
     - Approval phase
     - Deployment phase
     - Health verification phase
     - Rollback preparation phase

3. `DEPLOYMENT-DIAGRAM.md`
   - Document the release flow:
     Build → Validation → Approval → Deploy → Verify → Monitor → Rollback if needed

4. `RELEASE-GATES.md`
   - Define required approvals, validation checks, health verification criteria, and rollback readiness requirements

5. `RECOVERY-PLAYBOOK.md`
   - Define failed deployment response, rollback triggers, escalation process, and communication process

## Assignment Requirements

- The repository uses a broken operational process by design
- The focus is on documenting governance and process improvement, not code changes
- Students must open a GitHub Pull Request from `feature/deployment-workflow` into `main`
- Commits should be meaningful and include clear messages
- A short video summary of findings and improvements is required

## Files Included

- `docs/current-release-process.md` — broken release process description
- `docs/deployment-history.md` — inconsistent release records
- `docs/incident-log.md` — production incident examples
- `.github/workflows/deploy.yml` — simplistic, unsafe deployment workflow
- `examples/release-request-example.md` — example release request with missing controls
- Assignment templates in the repository root for your deliverables

## How to Proceed

1. Create and switch to the branch `feature/deployment-workflow`
2. Review the existing release process documentation and workflow
3. Document the current weaknesses in `DEPLOYMENT-AUDIT.md`
4. Design the controlled workflow and operational gates
5. Add the required deliverables and meaningful commit messages
6. Open a PR from `feature/deployment-workflow` into `main`

## Lab Goals

By the end of this lab, you should be able to:

- Identify the missing controls in a release process
- Design a sequenced deployment workflow with approvals and validation
- Define operational readiness and rollback preparation
- Explain why each control is necessary to reduce release risk
