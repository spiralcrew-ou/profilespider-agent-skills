---
name: competitor-research
description: >-
  Compares a group of companies by products, positioning, market
  focus, and differentiators. Use when the user provides several
  company records and wants a structured competitive comparison.
license: MIT
metadata:
  author: ProfileSpider
  version: "1.0"
  category: research
  source: https://profilespider.com/resources/competitor-research
---

# Competitor Research

## Purpose

Compare a group of companies by products, positioning, market focus, and differentiators.

## When to use this skill

- Building a competitive landscape from a company set
- Comparing positioning across rivals
- Finding white space and differentiation angles
- Preparing competitive briefs

## When not to use this skill

- You have only one company (use Company Research instead)
- The records lack product or positioning signal
- You need pricing data the records do not include

## Required inputs

- Two or more company records

## Optional inputs

- Comparison dimensions you care about
- Your own product for white-space framing

## Rules

1. Compare every company on the same dimensions.
2. Use supplied evidence; do not invent features or pricing.
3. Separate facts from interpretation.
4. Make overlaps and gaps explicit.
5. Keep the table structure consistent.

## Process

1. Choose comparison dimensions (or use supplied ones).
2. Extract each company against those dimensions.
3. Build the comparison table.
4. Summarize positioning, strengths, weaknesses.
5. Identify overlaps and differentiation opportunities.

## Output format

Return a single comparison with the following fields:

- comparison_table
- positioning_summary
- strengths
- weaknesses
- overlaps
- differentiation_opportunities

## Validation

- Confirm all companies share the same dimensions.
- Confirm claims cite evidence.
- Confirm opportunities follow from the comparison.

## Limitations

- Comparisons reflect supplied data, not full market knowledge.
- Positioning is interpretive and may need validation.
