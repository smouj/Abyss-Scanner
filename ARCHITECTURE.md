# 🔍 Abyss Scanner — Agent Runtime Architecture

## Architectural intent
This skill architecture is aligned to how an OpenClaw agent should execute this domain safely, with observable checkpoints and reversible actions.

## Agent execution flow
```mermaid
flowchart LR
  A[Input task] --> B[Scope + safety gate]
  B --> C[Stealth profile]
  C --> D[Execution]
  D --> E[Verification]
  E --> F[Outcome report]
```

**Canonical flow:** Objective -> Legal/ethical gate -> Stealth profile -> Evidence capture -> Confidence report

## Core components
Stealth browsing controls, anti-fingerprint pacing, OSINT extraction, confidence scoring.

## Control points (mandatory)
- Pre-check: validate scope, permissions, and policy constraints.
- Runtime-check: stop on suspicious or out-of-scope behavior.
- Post-check: verify objective completion + attach evidence.

## Error and rollback model
- On recoverable errors: retry with bounded policy.
- On high-risk or unknown states: fail-safe and require user confirmation.
- Always provide minimal rollback instructions in final output.

## Observability
- log key decisions (redacted)
- emit concise status (started/running/success/fail)
- include verification metrics when available
