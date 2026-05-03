# validator-rules.md

## 1. Overview
This document defines the canonical **Validator Rules Standard** for Beast System 3.0 — a SAIA‑Class S compliant, deterministic, audit‑ready specification governing how validators are defined, evaluated, and enforced across all workflows, lifecycles, and state‑machines.

Validators ensure:
- structural integrity  
- semantic correctness  
- safety and wellbeing compliance  
- identity and document consistency  
- workflow and lifecycle validity  
- audit‑ready explainability  

Validators are the **core enforcement layer** of the governance engine.

---

## 2. Core Principles
- Deterministic: same inputs → same validator outcome  
- Non‑punitive: validators cannot encode punishment  
- Dignity‑preserving: avoid degrading semantics  
- Trauma‑preventive: prefer supportive validation paths  
- Audit‑ready: every validator must be explainable  
- Composable: reusable across domains  
- Declarative: describe what must be true, not how to compute it  
- Machine‑readable: JSON‑serializable  
- Cross‑domain: identity, case, wellbeing, community, audit  

---

## 3. Canonical Validator Rules Object
```json
{
  "id": "string",
  "version": "string",
  "description": "string",
  "domain": "global",
  "lastUpdated": "YYYY-MM-DD",

  "validators": {},
  "groups": {},
  "invariants": {},
  "metadata": {}
}
