---
name: job-title-normalization
description: >-
  Converts inconsistent job titles into standardized role, department,
  and seniority labels. Use when the user provides records with
  free-text titles and wants consistent role family, department, and
  seniority fields.
license: MIT
metadata:
  author: ProfileSpider
  version: "1.0"
  category: data-cleanup
  source: https://profilespider.com/resources/job-title-normalization
---

# Job Title Normalization

## Purpose

Convert inconsistent job titles into standardized role, department, and seniority labels.

## When to use this skill

- Standardizing titles for segmentation or routing
- Filtering a list by seniority reliably
- Mapping titles to departments for targeting
- Cleaning multi-source contact data

## When not to use this skill

- The records have no title field
- Titles are in languages you have not configured
- You need verified org-chart data

## Required inputs

- Records containing job titles

## Optional inputs

- A role-family taxonomy
- A seniority scale
- Department definitions

## Rules

1. Map to the supplied taxonomy and scale when provided.
2. Preserve the original title.
3. Report confidence and ambiguity.
4. Do not invent seniority not implied by the title.
5. Be consistent across identical titles.

## Process

1. Parse each title.
2. Map to role family and department.
3. Assign seniority.
4. Record confidence and ambiguity.
5. Output original and normalized values.

## Output format

Return one record per title with the following fields:

- original_title
- normalized_title
- role_family
- department
- seniority
- confidence
- ambiguity_notes

## Validation

- Confirm identical titles map identically.
- Confirm low-confidence rows are flagged.
- Confirm seniority is implied by the title.

## Limitations

- Titles vary by company; mapping is heuristic.
- Inflated or vague titles may misstate seniority.
