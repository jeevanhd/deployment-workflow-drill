# Release Gates

Define the controls that must be satisfied before a release is allowed to proceed.

## Required approvals

- Who must approve production releases?
- What is the minimum number of approvers?
- Which teams must review the release?

## Validation checks

- What build or test validations are required?
- Which checks must pass before approval?
- How are exceptions handled?

## Health verification requirements

- What health validations must run after deployment?
- Which service endpoints must be verified?
- How long should health be monitored?

## Rollback readiness requirements

- What rollback options must be prepared before deployment?
- What information must be documented?
- How is rollback triggered?
