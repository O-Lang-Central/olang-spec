# Changelog: v1.0 → v1.1

## Added
- Parallel execution blocks (`Run in parallel [for <duration>] ... End`)
- Conditional logic (`If ... Else ... EndIf`) with system-provided boolean symbols
- Explicit symbol lifecycle and semantic enforcement rules
- Structured error codes (`SYMBOL_UNDEFINED`, `POLICY_VIOLATION`, etc.)
- Capability declaration contract (JSON schema)
- Execution trace format (normative)

## Clarified
- Distinction between **conformance** (static resolver contract) and **trust** (runtime policy)
- Kernel responsibilities vs. capability responsibilities
- "Resolver" in workflow syntax = "capability" in governance model

## Removed
- Dynamic capability loading (deferred to v1.2+)
- Custom type system (type safety deferred to resolver conformance layer)