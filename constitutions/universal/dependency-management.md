---
id: universal.dependency-management
title: Dependency Management
category: universal
version: 1.0.0
status: active
owners:
  - engineering-enablement
applies_to:
  - all
depends_on:
  - universal.engineering-principles
  - universal.security
---

# Dependency Management

## Purpose

Control dependency risk while allowing teams to use maintained ecosystem libraries.

## Mandatory requirements

- Dependencies MUST be approved, maintained, and appropriate for production use.
- Projects MUST use version pinning or lock files where the ecosystem supports them.
- Licenses MUST be compatible with project obligations.
- Vulnerability scanning MUST run for supported ecosystems.
- Unused dependencies MUST be removed.
- Major-version upgrades MUST be planned and reviewed for compatibility impact.

## Recommended practices

- Prefer well-maintained libraries with active security response.
- Keep direct dependencies smaller than transitive dependency graphs require.
- Document reasons for unusual or high-risk dependencies.

## Verification

Reviewers check lock files, license posture, vulnerability scan results, unused dependency reports, and upgrade notes.
