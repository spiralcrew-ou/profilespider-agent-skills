---
name: outreach-brief-generator
description: >-
  Converts structured prospect research into concise outreach
  preparation briefs. Use when the user provides prospect or account
  research and wants a brief with context, angles, and claims to
  verify. It generates a research brief and must not invent
  personalization or send outreach.
license: MIT
metadata:
  author: ProfileSpider
  version: "1.0"
  category: analysis
  source: https://profilespider.com/resources/outreach-brief-generator
---

# Outreach Brief Generator

## Purpose

Convert structured prospect research into concise outreach preparation briefs.

## When to use this skill

- Pre-call and pre-email preparation
- Turning research into a usable brief
- Grounding personalization in evidence
- Standardizing outreach prep across a team

## When not to use this skill

- You have no underlying research yet
- You want messages sent automatically (this only prepares)
- You expect invented personalization (it will not guess)

## Required inputs

- Structured prospect or account research

## Optional inputs

- Your offering and value props
- The outreach channel
- A specific contact

## Rules

1. Use only the supplied research and context.
2. Do not invent personalization, facts, or quotes.
3. Separate evidence from assumptions explicitly.
4. List claims requiring verification.
5. Produce a brief; never send outreach.

## Process

1. Parse the research and any offering context.
2. Summarize the account and contact context.
3. Derive evidence-based pain points and an angle.
4. Cite supporting evidence.
5. List claims requiring verification.

## Output format

Return one brief per prospect with the following fields:

- account_summary
- relevant_contact_context
- potential_pain_points
- supporting_evidence
- conversation_angle
- claims_requiring_verification

## Validation

- Confirm every point cites research evidence.
- Confirm assumptions are flagged for verification.
- Confirm nothing was fabricated.

## Limitations

- Brief quality depends on the input research.
- Pain points are hypotheses to confirm, not facts.
