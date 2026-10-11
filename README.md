# .github

## Default branch

This repository's default branch is `production`, unlike the organisation's default of `develop`, because changes here are not breaking in nature and are not expected to be made frequently. If a change is breaking, make it in [`standard`](https://github.com/marketsentinel/standard) instead.

## Branch flow

Feature branches are created from and merged back into `production` instead of `develop`.

## Inventory

| Path | Purpose |
| --- | --- |
| `ISSUE_TEMPLATE/` | Mandatory issue forms for every repository in the organisation. |
| `ISSUE_TEMPLATE/1-feat.yml` … `5-docs.yml` | One form per Conventional Commits type: `feat`, `fix`, `perf`, `refactor` and `docs`. The number prefix sets the order in the template chooser. |
| `ISSUE_TEMPLATE/6-everything-else.yml` | One form for the remaining types: `build`, `chore`, `ci`, `revert`, `style` and `test`. |
| `ISSUE_TEMPLATE/config.yml` | Disables blank issues so every issue uses a form. |