# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## What This Repository Is

This is a **Claude Code skill repository** for Onfly products. It contains two skills for building interfaces and content. The primary language is **Portuguese (Brazilian)**.

## Skills

### `onfly-retrospective-design`
Retrospective experiences for corporate travel. Invoke with `$onfly-retrospective-design`.
- `SKILL.md` — Rules, flow, tone, AI patterns, guardrails
- `references/screen-playbooks.md` — Screen flows per product x profile (source of truth)
- `references/mock-data-schema.md` — Mock data structure for consistency
- `references/evaluation-criteria.md` — Quality framework for pitch alignment
- `references/implementation-prompts.md` — User-facing prompt menu (not consumed during implementation)
- `claude-master-prompt.md` — Slim prompt that invokes the skill with architecture/UX/delivery specs

### `linkedin-feed-publisher`
Transforms slides/screens into LinkedIn posts and share actions. Invoke with `$linkedin-feed-publisher`.
- `SKILL.md` — Writing rules for feed, flow, delivery format, guardrails
- `references/post-playbooks.md` — Post structures by objective (launch, case, learning, behind-the-scenes, hiring)
- `references/style-guards.md` — Tone, hooks, anti-patterns, hashtag rules
- `references/share-action.md` — Share button implementation (UX flow, payload, states, fallbacks)

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

## Using the Skills

Each skill detects the target project's tech stack before implementing. Read only the references you need per task.

- `$onfly-retrospective-design` — for retrospective interfaces. Key refs: `screen-playbooks.md` (screens), `mock-data-schema.md` (data), `evaluation-criteria.md` (pitch).
- `$linkedin-feed-publisher` — for LinkedIn copy or share buttons. Key refs: `post-playbooks.md` (post structures), `style-guards.md` (tone), `share-action.md` (implementation).
