# Issue Description: Add Missing GitHub Workflows for Building and Sending Agendas

## Context / Problem
In `INSTRUCTIONS.md`, there are configuration guidelines for automation workflows:
- `schedules:` ISO-8601 interval setup in `.github/workflows/build_agenda.yml`
- Updating `[COMMUNITY NAME]` and `[MAILING LIST EMAIL]` in `.github/workflows/send_agenda.yml`

However, the `.github/workflows` folder is missing entirely, along with both `build_agenda.yml` and `send_agenda.yml`. This prevents automated build/send of meeting agendas.

## Proposed Solution
Create the `.github/workflows/` directory and add:
1. `build_agenda.yml` workflow which automatically builds the agenda from issues labelled `meeting` and posts it.
2. `send_agenda.yml` workflow which emails the agenda to the mailing list.

---

# PR Description: ci: Add build and send meeting agenda workflows

## Description
This pull request creates the missing GitHub workflow files:
- `.github/workflows/build_agenda.yml`
- `.github/workflows/send_agenda.yml`

These workflows automate the process of building the agenda (based on issues with the `meeting` label) and emailing it to the group mailing list as outlined in `INSTRUCTIONS.md`.

Fixes #3 (or equivalent issue)

## Type of change
- [x] New feature (non-breaking change which adds functionality)

## Checklist:
- [x] My code follows the style guidelines of this project
- [x] I have performed a self-review of my own code
- [x] I have made corresponding changes to the documentation
