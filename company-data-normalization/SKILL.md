---
name: company-data-normalization
description: >-
  Normalizes company names, industries, domains, locations, and
  descriptions. Use when the user provides company records and wants
  consistent canonical fields with confidence and unresolved items
  flagged.
license: MIT
metadata:
  author: ProfileSpider
  version: "1.0"
  category: data-cleanup
  source: https://profilespider.com/resources/company-data-normalization
---

# Company Data Normalization

## Purpose

Normalize company names, domains, industries, and locations into consistent values.

## When to use this skill

- Standardizing company fields before a join or merge
- Cleaning a multi-source company list
- Preparing data for segmentation or analysis
- Resolving inconsistent industry labels

## When not to use this skill

- You need to detect duplicates (use Duplicate Record Review)
- The records contain no company identifiers
- You need verified, authoritative registry data

## Required inputs

- Company records

## Optional inputs

- A canonical industry taxonomy
- A location format standard
- Known aliases to map

## Rules

1. Produce canonical values; do not invent unknown fields.
2. Map industries only to the supplied taxonomy when given.
3. Report a confidence level per record.
4. List unresolved fields explicitly.
5. Preserve originals alongside normalized values.

## Process

1. Parse each company record.
2. Normalize name and domain.
3. Map industry and standardize location.
4. Assign confidence.
5. List unresolved fields.

## Output format

Return one record per company with the following fields:

- normalized_company_name
- normalized_domain
- standardized_industry
- standardized_location
- normalization_confidence
- unresolved_fields

## Validation

- Confirm domains are root domains without protocol.
- Confirm industries match the taxonomy when provided.
- Confirm low-confidence rows are flagged.

## Limitations

- Normalization is heuristic without an authoritative registry.
- Ambiguous names may need manual disambiguation.
