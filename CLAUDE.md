# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## What This Repository Is

This is a **Claude Code skill repository** containing product specifications for two Onfly retrospective products. It holds the design skill (`onfly-retrospective-design`) and all reference materials needed to build the products. The primary language is **Portuguese (Brazilian)**.

## Repository Structure

- `claude-master-prompt.md` — Slim implementation prompt that invokes the skill and adds architecture/UX/delivery specs not covered by references.
- `skills/onfly-retrospective-design/SKILL.md` — Skill definition: rules, flow, format, tone, AI patterns, guardrails.
- `skills/onfly-retrospective-design/references/`:
  - `screen-playbooks.md` — Screen-by-screen flows for every product x profile combination (source of truth for screens)
  - `evaluation-criteria.md` — Quality framework for pitch and business value alignment
  - `mock-data-schema.md` — Data structure for mock data (company, employees, trips, expenses, monthly summaries)
- `skills/onfly-retrospective-design/references/implementation-prompts.md` — User-facing menu of ready-to-paste prompts (not consumed by the skill during implementation)

## Products

**Wrapped Onfly** — Annual retrospective. Cinematic, emotional, pitch-ready. 10 screens for gestor, 10 for colaborador, 5 abbreviated when gestor views an individual.

**Capsula de Viagens** — Monthly retrospective. Compact, recurring, habit-forming. 6 screens for gestor, 5 for colaborador, 5 abbreviated when gestor views an individual.

Both support 3 viewing modes: gestor (company-wide), colaborador (personal), gestor viewing individual team members.

## Key Constraints

- **No backend** — all data is mocked following `references/mock-data-schema.md`
- **Stack detection** — detect the tech stack from the target project; do not assume React or any specific framework
- **Maps are visual mocks** (SVG/static images), not Mapbox/Leaflet integrations
- **Every flow must include at least one AI-generated insight** — narrative, interpretation, or recommendation (not a chatbot)
- **Gestor viewing team = coaching/recognition, never surveillance**
- **Wrapped = immersive/editorial; Capsula = compact/operational** — they must feel different
- **Visual direction**: premium, editorial, dynamic. Avoid generic SaaS dashboard. Avoid literal Spotify copying.
- **Responsive**: mobile + desktop

## Using the Skill

Invoke with `$onfly-retrospective-design`. Read only the references you need — `screen-playbooks.md` for screen flows, `evaluation-criteria.md` for pitch alignment, `mock-data-schema.md` for data structure. The skill detects the target project's stack before implementing.
