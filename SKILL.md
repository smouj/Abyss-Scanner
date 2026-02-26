---
name: abyss-scanner
description: "🔍 OSINT stealth/anti-fingerprint."
metadata:
  {
    "openclaw": {
      "emoji": "🔍",
      "version": "0.2.0",
      "author": "smouj",
      "lang_default": "en"
    }
  }
---

# 🔍 Abyss Scanner

## Purpose
Escáner OSINT con navegación stealth, rotación de huellas y estrategias anti-fingerprinting para investigación en superficies complejas manteniendo trazabilidad y límites éticos.

## Tags
- security
- reliability
- automation
- openclaw-skill

## Execution contract
1. Validate request and constraints.
2. Generate minimal safe plan.
3. Execute in reversible steps.
4. Verify with explicit checks.
5. Return concise summary + next actions.

## Inputs expected
- Goal
- Constraints (time/cost/privacy)
- Optional files/URLs

## Outputs
- Plan
- Actions executed
- Verification results
- Rollback notes

## Guardrails
- Never expose secrets.
- No destructive operation without explicit confirmation.
- Fail safe with actionable diagnostics.

## Commands
```bash
# Placeholder entrypoint
printf "abyss-scanner: validate -> execute -> verify\n"
```

## Test checklist
- [ ] Happy path
- [ ] Error handling
- [ ] Idempotency
- [ ] Guardrails respected
