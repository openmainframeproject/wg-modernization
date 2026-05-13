# Content Schema

All framework documents in this repository follow a common structure so that content
is consistently navigable, reviewable, and referenceable across the five modernization
domains.

## Required frontmatter

Every document under `framework/` must include the following YAML frontmatter block:

```yaml
---
title: ""
domain: ""        # one of: applications | data | operations | interoperability | security
status: ""        # one of: draft | review | approved
version: ""       # semantic version, e.g. 0.1
authors: []
last-updated: ""  # ISO date, e.g. 2024-06-01
---
```

## Document lifecycle

**draft** — Work in progress. Content is incomplete or under active revision. Open
for early feedback but not yet ready for formal review.

**review** — Content is complete enough for WG review. The author has opened a pull
request and requested at least one maintainer to review. Discussion and objections
are recorded on the PR.

**approved** — The document has met the review criteria below and is considered a
stable WG output. Changes require a new PR moving the document back to `review`.

## Review criteria

A document moves from `review` to `approved` when:

- At least one WG maintainer has approved the pull request
- There are no unresolved objections after 7 days from the review request
- The frontmatter fields are fully populated
- Terminology is consistent with `modernization-definition.md`
