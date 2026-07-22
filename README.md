# Drafting a Controlled Deployment Workflow

## The Problem

You have joined the platform engineering team responsible for releasing the company's production services.

The application itself works. Containers build successfully. Kubernetes manifests exist. Deployments technically reach production.

The problem is that nobody has defined **how releases should move safely through the deployment process**.

Some deployments bypass validation entirely. Some releases go directly to production without approvals. Health checks are inconsistent. Rollback procedures exist only in people's memories. When incidents occur, every engineer responds differently.

The organization wants a deployment workflow that is predictable, repeatable, auditable, and safe.

Your job is to review the current release process, identify operational weaknesses, and design a complete controlled deployment workflow that the engineering team can adopt immediately.

The goal is not to deploy software.

The goal is to engineer the process that governs deployment.

---

# Getting Started

Fork and clone the assignment repository.

```bash
git clone https://github.com/kalviumcommunity/deployment-workflow-drill.git

cd deployment-workflow-drill
```

Create your working branch:

```bash
git checkout -b feature/deployment-workflow
```

All work for this assignment must be completed on this branch.

When finished:

```bash
git add .
git commit -m "feat: add controlled deployment workflow design"

git push origin feature/deployment-workflow
```

Open a Pull Request from:

```text
feature/deployment-workflow → main
```

---

# Tasks

## Task 1 — Audit the Existing Deployment Process

Review the repository documentation, deployment notes, release instructions, workflow files, and deployment diagrams provided in the repository.

Create:

```text
DEPLOYMENT-AUDIT.md
```

Identify at least five deployment-process weaknesses.

For each weakness:

- Describe the issue
- Explain the operational risk
- Explain the potential release impact
- Recommend a control that would reduce the risk

Examples include:

- Missing approval stages
- No rollback preparation
- Missing validation checks
- No release ownership
- No health verification
- No deployment visibility
- No release freeze process

General statements do not count.

Each weakness must include specific evidence.

---

## Task 2 — Design the Controlled Deployment Workflow

Create:

```text
DEPLOYMENT-WORKFLOW.md
```

Design the complete release movement process.

Your workflow must include:

### Build Validation Stage

Define:

- What gets validated
- Who owns validation
- What blocks release progression

### Release Approval Stage

Define:

- Who approves
- Approval criteria
- Escalation process

### Deployment Execution Stage

Define:

- Deployment sequence
- Release ownership
- Production release procedure

### Health Verification Stage

Define:

- Verification checks
- Success criteria
- Monitoring requirements

### Recovery Stage

Define:

- Failure handling process
- Rollback trigger conditions
- Incident ownership

Represent the release movement clearly.

---

## Task 3 — Create Release Gate Standards

Create:

```text
RELEASE-GATES.md
```

Define at least five release gates.

For each gate document:

- Gate name
- Purpose
- Validation criteria
- Failure consequence
- Responsible owner

Example categories:

- Build Success Gate
- Test Coverage Gate
- Security Scan Gate
- Approval Gate
- Production Readiness Gate
- Health Verification Gate

Explain why bypassing each gate creates risk.

---

## Task 4 — Create Deployment Recovery Documentation

Create:

```text
ROLLBACK-PLAYBOOK.md
```

Document:

### Immediate Rollback Procedure

- Trigger conditions
- First actions
- Decision owner

### Partial Failure Procedure

- Detection method
- Containment strategy
- Recovery path

### Full Deployment Failure Procedure

- Escalation process
- Communication steps
- Recovery workflow

For each scenario explain:

- What happened
- How engineers respond
- How service is restored

---

## Task 5 — Design a Deployment Workflow Diagram

Create:

```text
DEPLOYMENT-DIAGRAM.md
```

Include a deployment flow diagram showing:

```text
Code Commit
    ↓
Build Validation
    ↓
Approval Gate
    ↓
Deployment
    ↓
Health Verification
    ↓
Production Success
```

Include failure paths:

```text
Validation Failure
Deployment Failure
Health Check Failure
Rollback Trigger
```

The diagram must clearly show:

- Release movement
- Approval points
- Validation checkpoints
- Recovery paths

---

# Submission

Submit two items.

## 1. GitHub Pull Request Link

Example:

```text
https://github.com/YOUR-USERNAME/deployment-workflow-drill/pull/12
```

Requirements:

- PR must be public
- PR must remain open
- All required files must exist
- Work must be completed on feature/deployment-workflow

---

## 2. Video Explanation

Record a 3–5 minute walkthrough.

Explain:

- Deployment weaknesses identified
- Why the workflow was redesigned
- Release gates introduced
- Recovery strategy
- Most important operational safeguard added

Upload to Google Drive.

Set sharing to:

```text
Anyone with the link can view
```

Verify accessibility before submission.

# Relese Notes

this is a release
