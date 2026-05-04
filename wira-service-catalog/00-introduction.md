# WIRA Service Catalog — Introduction

## Purpose
This catalog defines the backend service taxonomy for WIRA, a Kenyan blue‑collar service marketplace. It standardizes job scopes, pricing anchors, and skill requirements at **Level 3 granularity** (specific, scope‑bounded tasks). It is not customer‑facing; it is used for AI symptom mapping, fundi matching, dispatch logic, and price estimation.

## Methodology
1. **Trade scoping:** Ten trade categories were selected based on common Kenyan household and SME service demand (Kiambu/Nairobi context).
2. **Level 3 job definition:** Each job is defined as a discrete unit of work with known scope, tools, time range, and parts.
3. **Symptom mapping:** Customer‑language symptom phrases are mapped to candidate Level 3 jobs, ranked by likely frequency.
4. **Standard vs inspection:** Jobs are tagged `standard_service: true` whenever the scope can be confidently known upfront. Inspection‑required jobs are reserved for genuinely uncertain root‑causes.
5. **Kenyan context:** Brands, system types, and failure modes are aligned to the Kenyan market (PPR vs GI piping, gravity‑fed tanks, 240V single‑phase, common appliance and vehicle brands).

## Sources and Pricing Policy
- **Parts pricing** is taken from Kenyan retail listings where available. When a reliable local source is not available, the field is explicitly marked **“no reliable source — flag for field validation.”**
- **Base prices** are **placeholders only** and must be field‑validated before launch.
- All sources are documented per trade in the **Bibliography** section.

## Limitations & Known Gaps
- Many Level 3 jobs require field validation of price and duration in Kiambu/Nairobi.
- Some specialty parts (inverter compressors, premium brand spares) lack consistent public pricing.
- Unusual installations (industrial, high‑rise commercial, three‑phase systems) are excluded.

## How to Use
- **AI mapping:** Use Layer 2 symptoms to shortlist candidate Level 3 jobs.
- **Dispatch:** Use Skill Tier, Tools, and standard_service flags to match fundis.
- **Pricing:** Apply base price + modifiers; validate during pilot.

## Versioning
- **Draft version:** v0.1 (work‑in‑progress)
- **Date:** 2026‑05‑04
