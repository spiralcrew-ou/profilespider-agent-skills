---
name: b2b-lead-qualification
description: >-
  Qualifies and scores B2B prospects against a supplied ideal customer
  profile. Use when the user provides a lead list, company records,
  prospect data, or qualification criteria and wants prioritization,
  fit analysis, or disqualification reasons.
license: MIT
metadata:
  author: ProfileSpider
  version: "1.0"
  category: qualification
  source: https://profilespider.com/resources/b2b-lead-qualification
---

# B2B Lead Qualification

## Purpose

Score and classify B2B prospects against a defined ideal customer profile, with reasoning and a recommended next action.

## When to use this skill

- Qualifying exported prospect lists before outreach
- Prioritizing accounts when you have more leads than capacity
- Separating high-fit and low-fit companies
- Documenting why a prospect matches an ICP

## When not to use this skill

- You have no defined ICP or qualification criteria yet
- You need verified contact details rather than fit scoring
- The dataset has no company or firmographic fields to score against

## Required inputs

- An ICP definition
- A prospect or company dataset
- Qualification criteria

## Optional inputs

- Exclusion criteria
- Weighted scoring rules
- Target locations
- Company size range
- Required technologies or industries

## Rules

1. Use only information present in the supplied dataset or explicitly provided by the user.
2. Do not invent missing company, contact, revenue, employee, technology, or location information.
3. Clearly distinguish known facts from assumptions.
4. Flag missing information that materially affects the score.
5. Apply the same scoring framework consistently to every prospect.

## Process

1. Parse the ideal customer profile.
2. Extract positive qualification criteria.
3. Extract disqualifying criteria.
4. Evaluate each prospect against both sets.
5. Assign a score from 0 to 100.
6. Explain the score using available evidence.
7. Recommend the next action.

## Output format

Return one record per prospect with the following fields:

- fit_score
- fit_level
- qualification_reason
- supporting_evidence
- missing_information
- recommended_next_action

## Validation

- Confirm every score is supported by evidence from the input.
- Confirm missing fields are listed rather than guessed.
- Confirm the same criteria were applied to every record.

## Limitations

- Scores reflect fit, not intent or buying readiness.
- A high score is not a guarantee of a sale; verify before investing heavily.
