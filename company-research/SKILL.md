---
name: company-research
description: >-
  Turns company records into structured company research summaries.
  Use when the user provides company names or records and wants a
  consistent overview, market position, and relevance assessment.
license: MIT
metadata:
  author: ProfileSpider
  version: "1.0"
  category: research
  source: https://profilespider.com/resources/company-research
---

# Company Research

## Purpose

Turn company records into a structured research summary: overview, market position, and relevance.

## When to use this skill

- Building account research before outreach
- Producing comparable company profiles at scale
- Summarizing a target account list
- Flagging what still needs manual research

## When not to use this skill

- The records contain no usable company signal
- You need real-time financials or news the data lacks
- You want verified contact details rather than a profile

## Required inputs

- Company names or records

## Optional inputs

- Your offering or angle for relevance scoring
- Industries of interest
- Fields you want prioritized

## Rules

1. Use only supplied information and clearly marked context.
2. Do not invent financials, headcounts, or customers.
3. Separate facts from inferences.
4. List research gaps rather than filling them.
5. Keep the structure identical across companies.

## Process

1. Parse each company record.
2. Summarize overview, industry, offering, and customers.
3. Assess market position from available signal.
4. List research gaps.
5. Assess relevance to the stated goal.

## Output format

Return one profile per company with the following fields:

- company_overview
- industry
- products_or_services
- target_customers
- market_position
- research_gaps
- relevance_assessment

## Validation

- Confirm each field is supported or marked as a gap.
- Confirm no invented figures appear.
- Confirm relevance ties to the stated goal.

## Limitations

- Profiles are only as current as the input data.
- Market position is an interpretation, not a ranking.
