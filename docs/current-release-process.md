# Current Release Process

The checkout service team currently follows a direct deployment process with minimal governance.

## How releases happen today

1. A developer pushes code directly to `main`.
2. The deployment pipeline runs automatically and deploys immediately.
3. No human approval step is required.
4. The release is declared complete once the deployment commands finish.
5. No separate validation gate is executed before release.
6. No rollback plan is prepared before deployment.
7. No health checks are recorded after deployment.

## Operational weaknesses

- **Direct deployments:** Any developer with write access can trigger production releases.
- **No approval stage:** There is no formal sign-off or release authorization.
- **No validation gates:** No build verification, smoke tests, or staging checks are required.
- **No rollback plan:** Teams do not prepare rollback actions before deployment.
- **No release checklist:** There is no formal release movement documentation.
- **No health checks:** Post-deployment health is not explicitly verified or logged.

## Team assumptions

- "If the deploy step passes, the release is successful."
- "Rollback can be handled if something fails in production."
- "We do not need a separate approval or validation process."

## Why this is risky

This process is operationally risky because it relies entirely on a single deployment step and assumes the first execution is correct. Production incidents have already shown that this assumption is unsafe.
