---
name: account-prioritization
description: >-
  Ranks companies or accounts by strategic relevance and opportunity.
  Use when the user provides accounts and wants a priority score,
  tier, rationale, risks, and next action.
license: MIT
metadata:
  author: ProfileSpider
  version: "1.0"
  category: analysis
  source: https://profilespider.com/resources/account-prioritization
---

# Account Prioritization

## Purpose

Rank companies or accounts by strategic relevance and opportunity with a clear rationale.

## When to use this skill

- Sequencing outreach across many accounts
- Building tiered account lists
- Focusing limited capacity on the best opportunities
- Justifying account priority to a team

## When not to use this skill

- Accounts are not yet qualified for fit
- You have no relevance or opportunity signal
- You need contact-level routing (use Persona Classification)

## Required inputs

- A set of accounts
- Prioritization criteria

## Optional inputs

- Opportunity signals (intent, growth)
- Strategic weighting
- Capacity constraints

## Rules

1. Rank against the supplied criteria and signals.
2. Use evidence; do not invent intent or growth signals.
3. Make tiers consistent with scores.
4. Flag risks that temper the priority.
5. Recommend a concrete next action.

## Process

1. Parse prioritization criteria and signals.
2. Score each account for relevance and opportunity.
3. Assign a tier.
4. Explain rationale and risks.
5. Recommend a next action.

## Output format

Return one record per account with the following fields:

- priority_score
- priority_tier
- supporting_evidence
- opportunity_rationale
- risks
- next_action

## Validation

- Confirm tiers follow from scores.
- Confirm evidence supports each priority.
- Confirm signals were not invented.

## Limitations

- Priority reflects available signal, not guaranteed outcomes.
- Stale signals can mislead; refresh before acting.
