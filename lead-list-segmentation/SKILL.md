---
name: lead-list-segmentation
description: >-
  Divides a lead list into useful commercial segments. Use when the
  user provides a combined lead list and wants segments with criteria,
  sizes, recommended treatment, and priority.
license: MIT
metadata:
  author: ProfileSpider
  version: "1.0"
  category: segmentation
  source: https://profilespider.com/resources/lead-list-segmentation
---

# Lead List Segmentation

## Purpose

Divide a lead list into useful commercial segments with criteria, size, and priority.

## When to use this skill

- Splitting one list into messaging-ready segments
- Prioritizing where to spend outreach effort
- Tailoring campaigns per segment
- Reporting list composition to stakeholders

## When not to use this skill

- The list has no fields to segment on
- You need per-record scoring (use Lead Qualification)
- The list is too small to segment meaningfully

## Required inputs

- A lead list

## Optional inputs

- Segmentation dimensions (industry, size, region, fit)
- A priority rule
- Target segment count

## Rules

1. Define explicit, non-overlapping criteria per segment.
2. Report accurate segment sizes.
3. Base segments on supplied fields only.
4. Recommend treatment proportional to value.
5. Make priorities consistent and justified.

## Process

1. Profile the list fields.
2. Choose segmentation dimensions.
3. Define segment criteria.
4. Assign records and count sizes.
5. Recommend treatment and priority.

## Output format

Return one record per segment with the following fields:

- segment_name
- segment_criteria
- included_records
- segment_size
- recommended_treatment
- priority

## Validation

- Confirm segment criteria do not overlap.
- Confirm sizes sum sensibly to the list.
- Confirm priorities follow the value logic.

## Limitations

- Segment quality depends on field completeness.
- Static segments need refreshing as the list grows.
