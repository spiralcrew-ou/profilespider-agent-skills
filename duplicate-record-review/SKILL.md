---
name: duplicate-record-review
description: >-
  Identifies likely duplicate profiles or companies using available
  record evidence. Use when the user provides a list and wants
  duplicate groups, match confidence, and merge recommendations.
  Describe records as likely duplicates unless there is an exact
  deterministic match.
license: MIT
metadata:
  author: ProfileSpider
  version: "1.0"
  category: data-cleanup
  source: https://profilespider.com/resources/duplicate-record-review
---

# Duplicate Record Review

## Purpose

Identify likely duplicate profiles or companies using available record evidence.

## When to use this skill

- De-duplicating a merged or re-scraped list
- Catching the same company under different names
- Preventing double outreach to one contact
- Producing a reviewable merge plan

## When not to use this skill

- The records share no comparable identifiers
- You need an irreversible automatic merge (always review)
- The list is already known to be unique

## Required inputs

- A list of company or profile records

## Optional inputs

- Match keys to prioritize (domain, email)
- A confidence threshold
- Fields that must match exactly

## Rules

1. Describe matches as likely unless an exact deterministic key matches.
2. Report match confidence and the evidence behind it.
3. Never auto-merge; recommend and flag for review.
4. List conflicting fields explicitly.
5. Prefer the most complete record as the survivor.

## Process

1. Compare records on available keys.
2. Group likely duplicates.
3. Assess confidence and list matching/conflicting fields.
4. Recommend a survivor and merges.
5. Set manual-review status.

## Output format

Return one record per duplicate group with the following fields:

- duplicate_group
- match_confidence
- matching_fields
- conflicting_fields
- merge_recommendation
- manual_review_status

## Validation

- Confirm only exact key matches are called certain.
- Confirm conflicts are listed for each group.
- Confirm no merge is performed automatically.

## Limitations

- Without unique keys, matches are probabilistic.
- Distinct entities can share names; review before merging.
