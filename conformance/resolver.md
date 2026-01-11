# Resolver Conformance (v1.1)

A **resolver** is a static O-Lang workflow that adheres to the **Resolver Contract** (Spec §14).

## Requirements
- Must declare `inputs`, `outputs`, `steps`, and `failures`
- Must only use allowed capabilities (`Allow resolvers:`)
- Must be testable by the [O-Lang Resolver Test Harness](https://github.com/O-Lang-Central/resolver-test)

## Test Binding
- All tests in `R-001` to `R-XXX` in [resolver-test v1.0.0](https://github.com/O-Lang-Central/resolver-test/releases/tag/v1.0.0) are required for v1.1 resolver conformance.

## Certification
Passing these tests qualifies a resolver for the **"O-Lang Conformant Resolver"** badge (self-asserted or verified).