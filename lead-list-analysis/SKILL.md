---
name: lead-list-analysis
description: >-
  Assesses the quality, composition, and usefulness of a lead list.
  Use when the user provides a lead list and wants completeness,
  distribution, quality issues, and recommended next actions.
license: MIT
metadata:
  author: ProfileSpider
  version: "1.0"
  category: analysis
  source: https://profilespider.com/resources/lead-list-analysis
---

# Lead List Analysis

## Purpose

Assess the quality, composition, and usefulness of a lead list with next actions.

## When to use this skill

- Sanity-checking a list before outreach
- Measuring field completeness and gaps
- Understanding list composition
- Deciding what to fix or enrich next

## When not to use this skill

- You want per-record scoring (use Lead Qualification)
- The file has no consistent structure
- You need market-level patterns (use Market Research)

## Required inputs

- A lead list

## Optional inputs

- Required fields for your use
- Your ICP for fit distribution
- A quality threshold

## Rules

1. Report real completeness rates, not estimates.
2. Surface concrete quality issues with counts.
3. Tie next actions to the issues found.
4. Do not invent missing values.
5. Keep the analysis structure consistent.

## Process

1. Profile the list size and fields.
2. Compute field completeness.
3. Summarize segment distribution.
4. Detect quality issues and missing data.
5. Recommend next actions.

## Output format

Return a list-quality report with the following fields:

- list_overview
- field_completeness
- segment_distribution
- quality_issues
- missing_data
- recommended_next_actions

## Validation

- Confirm completeness rates match the data.
- Confirm issue counts are accurate.
- Confirm actions address the issues.

## Limitations

- Analysis reflects the supplied list only.
- It measures completeness, not factual correctness.
