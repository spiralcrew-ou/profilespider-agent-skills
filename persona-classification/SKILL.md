---
name: persona-classification
description: >-
  Classifies professional profiles into buyer, influencer, user,
  decision-maker, founder, recruiter, or other personas. Use when the
  user provides profiles and wants persona labels with evidence and
  confidence. Must not infer sensitive personal attributes.
license: MIT
metadata:
  author: ProfileSpider
  version: "1.0"
  category: segmentation
  source: https://profilespider.com/resources/persona-classification
---

# Persona Classification

## Purpose

Classify professional profiles into buyer, influencer, user, decision-maker, and other personas.

## When to use this skill

- Routing contacts to the right messaging
- Mapping buying committees in target accounts
- Prioritizing decision-makers in a list
- Tailoring sequences by persona

## When not to use this skill

- Profiles lack a role or professional context
- You need sensitive personal attributes (never infer these)
- You want per-account scoring (use Qualification)

## Required inputs

- Professional profiles with roles

## Optional inputs

- Your persona definitions
- The product or deal context

## Rules

1. Classify from professional role evidence only.
2. Do not infer health, religion, ethnicity, sexual orientation, political affiliation, or other sensitive personal attributes.
3. Provide an alternate persona when signal is mixed.
4. Report confidence and missing information.
5. Use the supplied persona definitions when given.

## Process

1. Parse each profile and its role.
2. Match role evidence to persona definitions.
3. Assign a primary and alternate persona.
4. Estimate the decision-process role.
5. Report confidence and gaps.

## Output format

Return one record per profile with the following fields:

- persona
- likely_role_in_decision_process
- evidence
- confidence
- alternate_persona
- missing_information

## Validation

- Confirm no sensitive attributes were used.
- Confirm each persona cites role evidence.
- Confirm low-confidence rows are flagged.

## Limitations

- Titles do not always reflect real authority.
- Personas are interpretive and should be verified in conversation.
