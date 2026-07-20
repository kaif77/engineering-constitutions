---
id: universal.security
title: Security Requirements
category: universal
version: 1.0.0
status: active
owners:
  - security-team
applies_to:
  - all
depends_on:
  - universal.engineering-principles
---

# Security Requirements

## Purpose

Define security requirements that apply to all Entgra engineering work.

## Mandatory requirements

- Secrets, credentials, customer data, and restricted data MUST NOT be committed.
- Access MUST follow least privilege.
- Inputs MUST be validated at trust boundaries.
- Outputs MUST be encoded where injection or rendering risks exist.
- Authentication and authorization MUST be enforced for protected operations.
- Dependencies MUST be reviewed and monitored for vulnerabilities.
- Logs MUST NOT expose secrets or sensitive personal data.
- Vulnerabilities MUST be reported through the documented security process.

## Recommended practices

- Trigger security review for authentication, authorization, cryptography, sensitive data, tenancy, or internet-facing changes.
- Use secure defaults and make unsafe behavior explicit.
- Keep audit trails for security-sensitive actions.

## Verification

Reviewers verify secret scanning, dependency scanning, permission scope, input validation, sensitive-data handling, secure logging, and required security-review evidence.
