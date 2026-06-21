---
name: candidate-qualification
description: >-
  Evaluates candidate profiles against a job description and hiring
  criteria. Use when the user provides candidate profiles plus a role
  definition and wants consistent screening, matched requirements, and
  an interview recommendation.
license: MIT
metadata:
  author: ProfileSpider
  version: "1.0"
  category: qualification
  source: https://profilespider.com/resources/candidate-qualification
---

# Candidate Qualification

## Purpose

Evaluate candidate profiles against a job description and hiring criteria with an evidence-based fit score.

## When to use this skill

- Screening a sourced shortlist against one role
- Standardizing first-pass candidate review
- Documenting why a candidate advances or not
- Spotting must-have requirements that are missing

## When not to use this skill

- You have no structured job description or criteria
- You need to assess protected characteristics (never do this)
- The decision requires information not present in the profile

## Required inputs

- A job description
- Required skills
- Candidate profiles

## Optional inputs

- Preferred skills
- Seniority expectations
- Location or work-authorization requirements
- Compensation band

## Rules

1. Score only against the stated job requirements.
2. Use evidence from the candidate profile; do not assume unstated experience.
3. Do not infer health, religion, ethnicity, sexual orientation, political affiliation, or other sensitive personal attributes.
4. Treat missing required items as gaps, not failures, unless the user marks them disqualifying.
5. Apply the same criteria to every candidate.

## Process

1. Parse the job description into required and preferred criteria.
2. Map each criterion to evidence in the candidate profile.
3. Score required criteria first, then preferred.
4. List matched requirements, gaps, and risks.
5. Recommend advance, hold, or pass with a reason.

## Output format

Return one record per candidate with the following fields:

- candidate_fit_score
- required_criteria_matched
- missing_requirements
- risk_factors
- interview_recommendation

## Validation

- Confirm each matched requirement cites profile evidence.
- Confirm no sensitive attributes were inferred.
- Confirm the recommendation follows from the criteria.

## Limitations

- A profile is not a full assessment; use the score as a screen, not a decision.
- Self-reported experience may be inaccurate and should be verified.
