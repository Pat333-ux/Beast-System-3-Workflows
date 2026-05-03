# transition-rules.md

## 1. Overview
This document defines the canonical Transition Rules Standard for Beast System 3.0 — a SAIA‑Class S compliant, deterministic, audit‑ready specification governing how transitions occur across all state‑machines, workflows, and lifecycles. Transition rules determine which transitions are allowed, which conditions must be satisfied, which validators must pass, which policies must be respected, and which invariants must never be violated.

## 2. Core Principles
- Deterministic: same inputs → same transition outcome  
- Non-punitive: transitions cannot encode punishment  
- Dignity-preserving: transitions avoid degrading semantics  
- Trauma-preventive: prefer lower-intensity transitions when adequate  
- Audit-ready: every transition must be explainable  
- Cross-domain: applies to user, case, event, workflow, and system state-machines  
- Policy-bound: must comply with domain policies  
- Condition-driven: transitions occur only when conditions are satisfied  

## 3. Canonical Transition Rules Object
```json
{
  "id": "string",
  "version": "string",
  "description": "string",
  "domain": "global",
  "lastUpdated": "YYYY-MM-DD",
  "ruleGroups": {},
  "invariants": {},
  "metadata": {}
}
