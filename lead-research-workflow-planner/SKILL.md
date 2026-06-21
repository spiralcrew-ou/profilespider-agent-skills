---
name: lead-research-workflow-planner
description: >-
  Designs an end-to-end process for finding, extracting, enriching,
  qualifying, and exporting leads. Use when the user wants a
  repeatable lead workflow plan rather than a single source plan.
license: MIT
metadata:
  author: ProfileSpider
  version: "1.0"
  category: workflow-planning
  source: https://profilespider.com/resources/lead-research-workflow-planner
---

# Lead Research Workflow Planner

## Purpose

Design an end-to-end process for finding, extracting, enriching, qualifying, and exporting leads.

## When to use this skill

- Standing up a repeatable lead process
- Documenting a pipeline for a team
- Scoping a list-build project end to end
- Aligning sourcing, enrichment, and QC

## When not to use this skill

- You only need to choose sources (use Directory Research Planner)
- You want the work executed now (this plans it)
- The goal is undefined

## Required inputs

- A lead-generation goal or ICP

## Optional inputs

- Tools available
- Output/CRM requirements
- Volume targets

## Rules

1. Cover the full pipeline, not just sourcing.
2. Order stages logically with QC before export.
3. Tie fields to the qualification goal.
4. State risks and assumptions.
5. Keep the plan tool-agnostic unless tools are given.

## Process

1. Parse the goal and constraints.
2. Define ordered workflow stages.
3. Specify sources, fields, and enrichment.
4. Add quality-control steps.
5. Define output and list risks.

## Output format

Return a workflow plan with the following fields:

- workflow_stages
- source_types
- extraction_fields
- enrichment_steps
- quality_control_steps
- output_format
- risks_and_assumptions

## Validation

- Confirm stages are ordered and complete.
- Confirm QC precedes export.
- Confirm fields support qualification.

## Limitations

- A plan is not execution; results depend on tooling.
- Volume targets may need source validation.
