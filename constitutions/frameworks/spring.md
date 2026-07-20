---
id: framework.spring
title: Spring
category: framework
version: 1.0.0
status: active
owners:
  - java-platform
applies_to:
  - spring
depends_on:
  - language.java
  - universal.api-design
  - universal.observability
---

# Spring

## Purpose

Provide Spring-specific guidance for Java services.

## Mandatory requirements

- Configuration properties MUST be typed and documented.
- Controllers MUST keep authorization and validation behavior explicit.
- Dependency injection MUST avoid hidden global state.
- Transaction boundaries MUST be clear for data-changing operations.
- Actuator or equivalent health endpoints MUST be configured safely.

## Recommended practices

- Keep business logic outside controller classes.
- Prefer constructor injection.
- Document profile-specific configuration.

## Verification

Reviewers check property definitions, validation, authorization, transaction boundaries, health endpoints, and dependency injection style.
