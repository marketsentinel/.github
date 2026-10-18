<!--
If this is a promotion pull request (e.g. develop → staging, staging → production): delete everything.

Useful guides:
- [How to make code changes](https://github.com/marketsentinel/library/wiki/guide_how-to-make-code-changes)
- [How to make a feature safe to revert](https://github.com/marketsentinel/library/wiki/guide_how-to-make-a-feature-safe-to-revert)
-->

## Safe to revert

Mark `[x]` when a condition is met. If a condition does not apply, mark it and add `(N/A)`.

- [ ] The feature is behind a feature flag that is off by default
- [ ] The feature does not depend on another unreleased feature
- [ ] Database changes are backward-compatible with the current `production` code
- [ ] Stateful AWS resources have `DeletionPolicy: Retain` and `UpdateReplacePolicy: Retain`
- [ ] New data formats, events and API fields can be read by the current `production` code
- [ ] Dependency upgrades are in their own pull request

## Cannot be reverted

<!-- Describe anything a revert will not undo, such as emails sent, data deleted or secrets rotated, and how to recover. Otherwise write 'None'. -->

None
