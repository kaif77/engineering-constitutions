---
id: universal.observability
title: Observability
category: universal
version: 1.0.0
status: active
owners:
  - platform-operations
applies_to:
  - all
depends_on:
  - universal.engineering-principles
  - universal.security
---

# Observability

## Purpose

Ensure systems can be operated and diagnosed in production.

## Mandatory requirements

- Services MUST emit structured logs for meaningful events and failures.
- Logs and traces MUST carry correlation identifiers across service boundaries where possible.
- Services MUST expose health checks appropriate for their runtime.
- Important user, system, and dependency behavior SHOULD have metrics.
- Alerts MUST be actionable and tied to user impact or operational risk.
- Logs MUST avoid sensitive information.
- Security-sensitive actions SHOULD produce audit trails.

## Recommended practices

- Prefer consistent metric names and labels.
- Include enough context to debug failures without exposing restricted data.
- Review alert thresholds after incidents or noisy alert periods.

## Verification

Reviewers verify logging fields, correlation propagation, health checks, metric coverage, alert ownership, and sensitive-data filtering.
