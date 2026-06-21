---
name: market-research
description: >-
  Analyzes a dataset of companies or profiles to identify market
  patterns. Use when the user provides a larger dataset and wants
  segments, dominant categories, gaps, and emerging patterns.
license: MIT
metadata:
  author: ProfileSpider
  version: "1.0"
  category: research
  source: https://profilespider.com/resources/market-research
---

# Market Research

## Purpose

Analyze a dataset of companies or profiles to identify market segments and patterns.

## When to use this skill

- Understanding a scraped market dataset
- Finding natural segments in a large list
- Spotting dominant and underserved categories
- Sizing where the opportunity concentrates

## When not to use this skill

- The dataset is too small to show patterns
- You need statistically rigorous market sizing
- You want per-record actions (use Lead List Analysis)

## Required inputs

- A dataset of companies or profiles

## Optional inputs

- Dimensions of interest (industry, size, geography)
- A hypothesis to test

## Rules

1. Analyze the whole dataset, not a convenient subset.
2. Report counts and proportions where possible.
3. Do not over-generalize beyond what the data supports.
4. State source skew and limitations.
5. Separate observed patterns from speculation.

## Process

1. Profile the dataset structure and fields.
2. Identify recurring characteristics and categories.
3. Derive natural segments.
4. Identify gaps and emerging patterns.
5. State limitations.

## Output format

Return a market analysis with the following fields:

- market_segments
- recurring_characteristics
- dominant_categories
- gaps
- emerging_patterns
- research_limitations

## Validation

- Confirm segment claims reflect the data distribution.
- Confirm limitations note any sampling skew.
- Confirm no invented statistics.

## Limitations

- Findings describe the supplied dataset, not the whole market.
- Source bias in collection carries into the analysis.
