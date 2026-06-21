---
name: territory-segmentation
description: >-
  Divides records into geographic or account-ownership territories.
  Use when the user provides records with location or account data and
  wants consistent territory assignments with unresolved locations
  flagged.
license: MIT
metadata:
  author: ProfileSpider
  version: "1.0"
  category: segmentation
  source: https://profilespider.com/resources/territory-segmentation
---

# Territory Segmentation

## Purpose

Divide records into geographic or account-ownership territories with allocation notes.

## When to use this skill

- Splitting a list across a sales team
- Applying geographic territory rules consistently
- Handling named-account ownership
- Auditing how accounts were allocated

## When not to use this skill

- Records have no location or account-owner data
- You need balanced quota modeling (this assigns, not balances quotas)
- Ownership rules are undefined

## Required inputs

- Records with location or account data
- Territory rules

## Optional inputs

- Named-account ownership map
- Tie-break rules
- Region definitions

## Rules

1. Apply named-account ownership before geographic rules.
2. Use only supplied location/account data.
3. Flag records that cannot be resolved.
4. Record the basis and any tie-breaks.
5. Be consistent across records.

## Process

1. Parse territory and ownership rules.
2. Apply named-account ownership.
3. Assign remaining records geographically.
4. Flag unresolved locations.
5. Record allocation notes.

## Output format

Return one assignment per record with the following fields:

- assigned_territory
- geographic_basis
- account_grouping
- unresolved_locations
- allocation_notes

## Validation

- Confirm named accounts override geography.
- Confirm unresolved records are flagged, not guessed.
- Confirm the basis is recorded per record.

## Limitations

- Assignment quality depends on location accuracy.
- It allocates by rules; it does not balance workloads.
