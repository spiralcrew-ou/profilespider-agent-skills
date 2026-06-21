---
name: research-gap-analysis
description: >-
  Identifies missing information required to complete qualification,
  segmentation, or outreach preparation. Use when the user provides
  records and a goal and wants prioritized research gaps with sources.
license: MIT
metadata:
  author: ProfileSpider
  version: "1.0"
  category: analysis
  source: https://profilespider.com/resources/research-gap-analysis
---

# Research Gap Analysis

## Purpose

Identify missing information required to complete qualification, segmentation, or outreach prep.

## When to use this skill

- Finding what blocks qualification or segmentation
- Prioritizing enrichment work
- Scoping research before outreach
- Turning "incomplete data" into a task list

## When not to use this skill

- You have no goal to assess gaps against
- The dataset is already complete
- You want the gaps filled, not identified

## Required inputs

- Records
- The goal (qualify, segment, or prep outreach)

## Optional inputs

- Required fields for the goal
- Approved research sources

## Rules

1. Assess gaps against the stated goal.
2. Explain why each gap matters and its impact.
3. Suggest a realistic research source per gap.
4. Prioritize gaps by impact.
5. List assumptions to verify.

## Process

1. Parse the goal and required fields.
2. Compare records to requirements.
3. List missing fields and their impact.
4. Suggest sources and assign priority.
5. Record unresolved assumptions.

## Output format

Return one record per identified gap with the following fields:

- missing_field
- why_it_matters
- impact_on_decision
- suggested_research_source
- priority
- unresolved_assumptions

## Validation

- Confirm gaps map to the goal.
- Confirm priorities reflect impact.
- Confirm assumptions are flagged.

## Limitations

- It identifies gaps; it does not fill them.
- Source suggestions may vary in availability.
