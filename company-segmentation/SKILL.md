---
name: company-segmentation
description: >-
  Groups companies by industry, business model, size, maturity,
  market, or strategic fit. Use when the user provides company records
  and wants consistent segment assignments with definitions and
  confidence.
license: MIT
metadata:
  author: ProfileSpider
  version: "1.0"
  category: segmentation
  source: https://profilespider.com/resources/company-segmentation
---

# Company Segmentation

## Purpose

Group companies by industry, business model, size, maturity, market, or strategic fit.

## When to use this skill

- Grouping a target account list for ABM
- Defining tiers for a go-to-market plan
- Aligning messaging to company type
- Reporting account-base composition

## When not to use this skill

- The records lack firmographic signal
- You need per-contact personas (use Persona Classification)
- You want market-wide patterns (use Market Research)

## Required inputs

- Company records

## Optional inputs

- Your segment definitions
- Dimensions to weight (model, size, maturity)

## Rules

1. Assign one primary segment per company.
2. Use consistent, explicit segment definitions.
3. Support assignments with record evidence.
4. Report confidence per assignment.
5. Do not invent firmographic data.

## Process

1. Establish segment definitions.
2. Evaluate each company against them.
3. Assign the best-fit segment.
4. Record supporting characteristics and confidence.
5. Add segment-level observations.

## Output format

Return one record per company with the following fields:

- company_segment
- segment_definition
- supporting_characteristics
- confidence
- segment_level_observations

## Validation

- Confirm one segment per company.
- Confirm assignments cite evidence.
- Confirm definitions are applied consistently.

## Limitations

- Segments depend on firmographic completeness.
- Edge-case companies may fit multiple segments.
