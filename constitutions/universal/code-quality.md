---
id: universal.code-quality
title: Code Quality
category: universal
version: 1.0.0
status: active
owners:
  - engineering-leadership
applies_to:
  - all
depends_on:
  - universal.engineering-principles
---

# Code Quality

## Purpose

Set baseline expectations for readable, reliable, and reviewable code.

## Mandatory requirements

- Code MUST use clear names that communicate domain intent.
- Units of code MUST be cohesive and avoid unnecessary complexity.
- Failures MUST NOT be ignored or hidden without an explicit reason.
- Secrets, tokens, private keys, and credentials MUST NOT be committed.
- Formatting and static analysis MUST pass before merge.
- Dead code MUST be removed when it is no longer used.
- Commits SHOULD be organized so reviewers can understand behavior changes.

## Recommended practices

- Remove duplication when it obscures intent or creates maintenance risk.
- Prefer explicit error handling and actionable messages.
- Keep abstractions proportional to demonstrated complexity.

## Verification

Run formatters, linters, static analysis, and tests. Reviewers inspect naming, error paths, complexity, and removed or unused code.
