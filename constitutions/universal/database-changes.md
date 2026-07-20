---
id: universal.database-changes
title: Database Changes
category: universal
version: 1.0.0
status: active
owners:
  - data-platform
applies_to:
  - all
depends_on:
  - universal.engineering-principles
---

# Database Changes

## Purpose

Make database evolution reliable, reviewable, and recoverable.

## Mandatory requirements

- Schema changes MUST use versioned migrations.
- Production rollouts MUST preserve backward compatibility unless explicitly approved.
- Destructive changes MUST NOT be made without review, recovery planning, and data impact analysis.
- Data migrations MUST include verification steps.
- Index changes MUST consider query performance and rollout cost.
- Rollback or recovery plans MUST exist for risky changes.

## Recommended practices

- Deploy additive changes before code that depends on them.
- Backfill data in controlled batches when volume is significant.
- Measure query plans for high-traffic tables.

## Verification

Reviewers inspect migrations, rollout order, rollback or recovery plans, data verification, and performance evidence.
