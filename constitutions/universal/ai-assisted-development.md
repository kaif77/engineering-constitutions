---
id: universal.ai-assisted-development
title: AI-Assisted Development
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
  - universal.testing
---

# AI-Assisted Development

## Purpose

Set expectations for responsible use of AI coding tools.

## Mandatory requirements

- Developers remain accountable for AI-generated output.
- AI-generated code MUST be reviewed, understood, and tested before merge.
- Prompts MUST NOT include secrets, credentials, customer data, or restricted data.
- AI-generated citations, package recommendations, and technical claims MUST be verified.
- Licensing and attribution requirements MUST be preserved.
- AI tools MUST NOT bypass security, review, or approval controls.
- Specifications and documentation MUST be updated when implementation behavior changes.

## Recommended practices

- Prefer small, reviewable AI-assisted changes.
- Record important assumptions made during generation.
- Ask tools to explain risky code paths before accepting them.

## Verification

Reviewers verify tests, provenance-sensitive changes, prompt safety for shared examples, documentation updates, and compliance with normal review controls.
