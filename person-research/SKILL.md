---
name: person-research
description: >-
  Creates structured professional research summaries from public
  profile information. Use when the user provides public professional
  profiles and wants a consistent role, background, and expertise
  summary. Must avoid inferring sensitive personal attributes.
license: MIT
metadata:
  author: ProfileSpider
  version: "1.0"
  category: research
  source: https://profilespider.com/resources/person-research
---

# Person Research

## Purpose

Create structured professional research summaries from public profile information, safely.

## When to use this skill

- Preparing for a sales or recruiting conversation
- Summarizing a sourced profile list consistently
- Identifying relevant experience for a role or account
- Flagging what is unknown about a contact

## When not to use this skill

- You only have a name with no professional context
- You need personal, private, or sensitive attributes (never infer these)
- You want verified contact details rather than a summary

## Required inputs

- Public professional profile information

## Optional inputs

- The role or account context
- Specific expertise you care about

## Rules

1. Use only supplied public, professional information.
2. Do not infer health, religion, ethnicity, sexual orientation, political affiliation, or other sensitive personal attributes.
3. Do not speculate about personality, intent, or private life.
4. Separate stated facts from inferences.
5. List unknowns as research gaps.

## Process

1. Parse the public profile.
2. Summarize role, background, and expertise.
3. Tie relevant experience to the stated context.
4. List affiliations explicitly stated.
5. Record research gaps.

## Output format

Return one summary per person with the following fields:

- current_role
- professional_background
- areas_of_expertise
- relevant_experience
- affiliations
- research_gaps

## Validation

- Confirm no sensitive attributes were inferred.
- Confirm each field cites profile evidence.
- Confirm gaps are listed, not filled.

## Limitations

- Profiles may be outdated or incomplete.
- Professional relevance is an interpretation, not a fact.
