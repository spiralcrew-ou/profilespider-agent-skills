---
name: supplier-qualification
description: >-
  Assesses potential suppliers against defined commercial,
  operational, and compliance requirements. Use when the user provides
  supplier records plus sourcing requirements and wants a consistent
  shortlist with strengths and risks.
license: MIT
metadata:
  author: ProfileSpider
  version: "1.0"
  category: qualification
  source: https://profilespider.com/resources/supplier-qualification
---

# Supplier Qualification

## Purpose

Assess potential suppliers against defined commercial, operational, and compliance requirements.

## When to use this skill

- Shortlisting suppliers from a sourcing long-list
- Comparing vendors against the same requirements
- Surfacing compliance or location risks early
- Documenting why a supplier is in or out

## When not to use this skill

- You have no defined requirements or risk criteria
- You need audited financials the records do not contain
- Final selection requires legal or compliance sign-off this cannot replace

## Required inputs

- Supplier records
- Product or service requirements
- Risk and compliance criteria

## Optional inputs

- Location requirements
- Capacity or volume needs
- Certifications required
- Budget or pricing band

## Rules

1. Score only against the supplied requirements.
2. Use evidence from the records; do not assume certifications or capacity.
3. Distinguish stated facts from inferences.
4. Flag compliance-relevant gaps explicitly.
5. Apply criteria consistently to every supplier.

## Process

1. Parse requirements and risk criteria.
2. Evaluate each supplier against them.
3. Identify strengths and risks with evidence.
4. Score fit from 0 to 100.
5. List missing information and recommend a next step.

## Output format

Return one record per supplier with the following fields:

- supplier_fit_score
- strengths
- risks
- missing_information
- recommended_next_step

## Validation

- Confirm risks and strengths cite record evidence.
- Confirm compliance gaps are surfaced, not assumed away.
- Confirm scores are comparable across suppliers.

## Limitations

- A record-based screen is not due diligence; verify before contracting.
- Certifications listed in data should be independently confirmed.
