# workflow-specification.md

## 1. Overview
This document defines the canonical workflow specification format for Beast System 3.0 — a SAIA‑Class S compliant, deterministic, audit‑ready method for describing any workflow (onboarding, verification, wellbeing, community, escalation, audit, or custom domain workflows). All engines must be able to parse, validate, and execute workflows defined in this format.

## 2. Core Principles
- Deterministic: same inputs → same transitions → same outcomes  
- Non‑punitive: workflows cannot encode punishment  
- Dignity‑preserving: no shaming or degrading semantics  
- Trauma‑preventive: prefer lower‑intensity paths when adequate  
- Audit‑ready: every transition is loggable and explainable  
- Cross‑domain interoperable: identity, case, wellbeing, community, audit  
- Policy‑bound: governed by at least one policy artifact  

## 3. Canonical Workflow Object
```json
{
  "id": "string",
  "version": "string",
  "description": "string",
  "domain": "string",
  "lastUpdated": "YYYY-MM-DD",
  "states": {},
  "transitions": {},
  "policies": {},
  "integration": {},
  "audit": {},
  "metadata": {}
}
