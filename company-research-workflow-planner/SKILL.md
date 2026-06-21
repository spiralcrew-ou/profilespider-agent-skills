---
name: company-research-workflow-planner
description: >-
  Creates a repeatable process for researching and comparing
  companies. Use when the user wants a structured, reusable
  company-research workflow with objectives, sources, fields, and
  validation.
license: MIT
metadata:
  author: ProfileSpider
  version: "1.0"
  category: workflow-planning
  source: https://profilespider.com/resources/company-research-workflow-planner
---

# Company Research Workflow Planner

## Purpose

Create a repeatable process for researching and comparing companies.

## When to use this skill

- Standardizing company research across a team
- Building a repeatable account-research playbook
- Defining the fields every profile needs
- Setting completion criteria for research tasks

## When not to use this skill

- You want one company researched now (use Company Research)
- You have no research objective
- You need the research executed, not planned

## Required inputs

- A research objective

## Optional inputs

- Required output fields
- Approved sources
- A comparison framework

## Rules

1. Define explicit required fields and completion criteria.
2. Sequence research logically.
3. Include validation steps.
4. Keep the output structure consistent.
5. Note assumptions where objectives are broad.

## Process

1. Parse the research objective.
2. Define sources and required fields.
3. Order the research sequence.
4. Add validation steps.
5. Define output structure and completion criteria.

## Output format

Return a research process with the following fields:

- research_objectives
- source_types
- required_fields
- research_sequence
- validation_steps
- output_structure
- completion_criteria

## Validation

- Confirm required fields cover the objective.
- Confirm validation steps are present.
- Confirm completion criteria are testable.

## Limitations

- A process is only as good as the sources it uses.
- Completion criteria may need tuning over time.
