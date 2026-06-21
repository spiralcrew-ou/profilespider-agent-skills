---
name: directory-research-planner
description: >-
  Turns an ICP or research goal into a plan for finding and scraping
  suitable directories. Use when the user has a target audience but is
  unsure where to find them, and wants source categories, queries, and
  an extraction workflow.
license: MIT
metadata:
  author: ProfileSpider
  version: "1.0"
  category: workflow-planning
  source: https://profilespider.com/resources/directory-research-planner
---

# Directory Research Planner

## Purpose

Turn an ICP or research goal into a plan for finding and scraping suitable directories.

## When to use this skill

- Planning where to source a new list
- Translating an ICP into search queries
- Choosing the right directory types
- Scoping a scraping project before starting

## When not to use this skill

- You already have your source list
- You need the data extracted now (this plans, it does not scrape)
- Your audience is not present in public directories

## Required inputs

- An ICP or research goal

## Optional inputs

- Known good sources
- Geographies to focus on
- Fields you must collect

## Rules

1. Tie every recommendation to the stated ICP/goal.
2. Suggest public, accessible source types.
3. Make inclusion and exclusion criteria explicit.
4. Recommend an efficient extraction order.
5. Note assumptions where the goal is vague.

## Process

1. Parse the ICP or goal.
2. Identify directory and source types.
3. Draft search queries.
4. Define fields and inclusion/exclusion criteria.
5. Recommend an extraction workflow.

## Output format

Return a sourcing plan with the following fields:

- directory_types
- suggested_source_categories
- search_queries
- fields_to_collect
- inclusion_criteria
- exclusion_criteria
- recommended_extraction_workflow

## Validation

- Confirm sources match the ICP.
- Confirm criteria are explicit and testable.
- Confirm the workflow is actionable.

## Limitations

- It plans sources; it does not verify they exist.
- Some audiences are not well represented in public directories.
