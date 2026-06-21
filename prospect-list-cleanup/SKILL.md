---
name: prospect-list-cleanup
description: >-
  Normalizes and improves the consistency of prospect-list data. Use
  when the user provides a messy prospect or lead export and wants
  standardized records, flagged issues, and a cleanup summary.
license: MIT
metadata:
  author: ProfileSpider
  version: "1.0"
  category: data-cleanup
  source: https://profilespider.com/resources/prospect-list-cleanup
---

# Prospect List Cleanup

## Purpose

Normalize and improve the consistency of prospect-list data before outreach or import.

## When to use this skill

- Preparing an export for CRM or outreach import
- Standardizing names, casing, and formats
- Flagging incomplete or broken rows
- Producing a defensible cleanup audit

## When not to use this skill

- You need verified emails or enrichment, not cleanup
- The file has no consistent columns to normalize
- You want hard de-duplication (use Duplicate Record Review)

## Required inputs

- A prospect or lead list

## Optional inputs

- A target column schema
- Formatting conventions (casing, phone format)
- Fields that are mandatory

## Rules

1. Standardize formatting; do not invent missing values.
2. Flag incomplete and suspect rows rather than deleting them.
3. Record every change in normalization notes.
4. Preserve the original value when flagging an error.
5. Apply the same conventions to every row.

## Process

1. Profile the columns and detect formats.
2. Normalize casing, names, companies, and formats.
3. Flag incomplete and suspected-error rows.
4. Record normalization notes.
5. Produce a cleanup summary with counts.

## Output format

Return the cleaned list plus a summary with the following fields:

- standardized_records
- incomplete_records
- suspected_errors
- normalization_notes
- cleanup_summary

## Validation

- Confirm no values were invented.
- Confirm flagged rows retain their original data.
- Confirm the summary counts match the records.

## Limitations

- It standardizes formatting, not factual accuracy.
- Suspected errors are heuristics and should be reviewed.
