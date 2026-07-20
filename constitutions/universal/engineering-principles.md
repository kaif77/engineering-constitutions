---
id: universal.engineering-principles
title: Engineering Principles
category: universal
version: 1.0.0
status: active
owners:
  - engineering-leadership
applies_to:
  - all
depends_on: []
---

# Engineering Principles

## Purpose

Define the default engineering principles that apply to all Entgra projects.

## Mandatory requirements

- Teams MUST prefer correctness over cleverness.
- Code MUST be maintainable, readable, and owned by an accountable team.
- Public behavior MUST remain backward compatible unless an approved migration plan exists.
- Designs MUST be secure by default and testable before release.
- Services MUST expose enough observability to diagnose production behavior.
- Material decisions MUST be documented with evidence, trade-offs, and ownership.
- Changes SHOULD be small enough for meaningful review.

## Recommended practices

- Optimize for clear intent, simple control flow, and predictable operational behavior.
- Split large changes into reviewable increments.
- Record assumptions when requirements, data, or external systems are uncertain.

## Verification

Reviewers verify that changes have clear ownership, tests, documentation, and an explicit compatibility or migration story when behavior changes.
