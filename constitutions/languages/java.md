---
id: language.java
title: Java
category: language
version: 1.0.0
status: active
owners:
  - java-platform
applies_to:
  - java
depends_on:
  - universal.code-quality
  - universal.testing
  - universal.dependency-management
---

# Java

## Purpose

Provide Java-specific engineering guidance.

## Mandatory requirements

- Java projects MUST define the supported Java runtime version.
- Builds MUST use a reproducible tool such as Maven or Gradle with committed configuration.
- Public APIs MUST avoid exposing mutable internals.
- Exceptions MUST carry actionable context without leaking sensitive data.
- Dependency scopes MUST be intentional.

## Recommended practices

- Prefer immutable value types for shared data.
- Use static analysis and formatting consistently.
- Keep concurrency primitives explicit and reviewed.

## Verification

Reviewers check build configuration, Java version, dependency scopes, exception handling, and static-analysis output.
