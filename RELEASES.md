# Release Notes

---

## v1.1.0 - 2026-07-22 (Deploy #15)

### Change Scope

- Added: Deployment release documentation
- Changed: Updated README deployment information
- Fixed: Documentation clarity for deployment workflow

### Validation

- GitHub Actions: PASS
- Local tests: PASS
- Manual verification:
  - README renders correctly
  - Repository cloned successfully

### Risks

- Documentation changes only.
- Low deployment risk.
- Monitor workflow execution after deployment.

### Rollback

Target:
v1.0.0

Steps:

1. Checkout previous tag

```
git checkout v1.0.0
```

2. Redeploy previous version.

3. Verify deployment health.

### Traceability

Tag:
v1.1.0

Build:
GitHub Actions Run #<run-id>

Commit:
cd5fd09

Repository:
https://github.com/jeevanhd/deployment-workflow-drill
