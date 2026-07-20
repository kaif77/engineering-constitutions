---
id: universal.testing
title: Testing
category: universal
version: 1.0.0
status: active
owners:
  - quality-engineering
applies_to:
  - all
depends_on:
  - universal.engineering-principles
---

# Testing

## Purpose

Define minimum expectations for proving software behavior before release.

## Mandatory requirements

- Changes MUST include appropriate unit, integration, or end-to-end coverage.
- Defect fixes MUST include regression tests when technically feasible.
- Tests MUST be deterministic and isolated from unrelated external state.
- Assertions MUST verify meaningful behavior, including failure paths.
- Tests MUST NOT exist only to increase coverage numbers.
- Required test commands MUST be documented for contributors.

## Recommended practices

- Prefer fast unit tests for local confidence and focused integration tests for boundaries.
- Use stable fixtures and explicit setup instead of relying on execution order.
- Keep slow or environment-heavy tests clearly labeled.

## Verification

Reviewers verify relevant test coverage, run documented test commands, and inspect failure-path assertions for changed behavior.
