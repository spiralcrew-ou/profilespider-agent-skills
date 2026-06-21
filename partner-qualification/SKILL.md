---
name: partner-qualification
description: >-
  Evaluates potential channel, integration, affiliate, or strategic
  partners. Use when the user provides partner profiles plus
  partnership goals and wants fit scoring, partnership type, and
  outreach priority.
license: MIT
metadata:
  author: ProfileSpider
  version: "1.0"
  category: qualification
  source: https://profilespider.com/resources/partner-qualification
---

# Partner Qualification

## Purpose

Evaluate potential channel, integration, affiliate, or strategic partners against partnership goals.

## When to use this skill

- Prioritizing a partner long-list
- Classifying the likely partnership type per candidate
- Surfacing competitive or channel-conflict risks
- Sequencing partnership outreach

## When not to use this skill

- You have no partnership goals or target markets defined
- The records lack enough signal to assess fit
- You need contract terms rather than a fit assessment

## Required inputs

- Partner profiles
- Partnership goals
- Required capabilities

## Optional inputs

- Target markets
- Existing partners to avoid overlap
- Preferred partnership types

## Rules

1. Score against stated partnership goals only.
2. Use evidence from the profiles; do not assume capabilities.
3. Flag competitive overlap and channel conflict explicitly.
4. Separate facts from strategic assumptions.
5. Apply the same framework to every candidate.

## Process

1. Parse partnership goals and required capabilities.
2. Assess each candidate for fit and overlap.
3. Classify the most fitting partnership type.
4. Estimate strategic value and risks.
5. Score fit and assign an outreach priority.

## Output format

Return one record per partner with the following fields:

- partner_fit_score
- partnership_type
- strategic_value
- risks
- recommended_outreach_priority

## Validation

- Confirm partnership type follows from the evidence.
- Confirm risks include any competitive overlap.
- Confirm priorities are comparable across candidates.

## Limitations

- Strategic value is an estimate, not a forecast.
- Partnership fit depends on relationship factors not present in records.
