---
name: recruiting-sourcing-planner
description: >-
  Converts a job description into a structured candidate-sourcing
  workflow. Use when the user provides a role and wants candidate
  criteria, search terms, source recommendations, and a screening
  process. Must avoid sourcing on sensitive personal attributes.
license: MIT
metadata:
  author: ProfileSpider
  version: "1.0"
  category: workflow-planning
  source: https://profilespider.com/resources/recruiting-sourcing-planner
---

# Recruiting Sourcing Planner

## Purpose

Convert a job description into a structured candidate-sourcing workflow.

## When to use this skill

- Kicking off a new requisition
- Turning a role into Boolean search terms
- Choosing where to source candidates
- Standardizing first-pass screening

## When not to use this skill

- You have no job description or criteria
- You want to filter on protected characteristics (never do this)
- You need the sourcing executed now

## Required inputs

- A job description

## Optional inputs

- Must-have vs nice-to-have skills
- Locations or work authorization
- Target companies

## Rules

1. Base criteria and terms on professional requirements only.
2. Do not infer health, religion, ethnicity, sexual orientation, political affiliation, or other sensitive personal attributes.
3. Make exclusion criteria professional and explicit.
4. Recommend accessible, public sources.
5. Keep screening consistent across candidates.

## Process

1. Parse the job description.
2. Define candidate criteria and profile types.
3. Draft search terms.
4. Recommend sources and screening fields.
5. Define exclusions and a review process.

## Output format

Return a sourcing workflow with the following fields:

- candidate_criteria
- target_profile_types
- search_terms
- source_recommendations
- screening_fields
- exclusion_criteria
- review_process

## Validation

- Confirm criteria are professional, not personal.
- Confirm search terms reflect requirements.
- Confirm the review process is consistent.

## Limitations

- Sourcing plans depend on candidate availability.
- Search terms may need iteration per platform.
