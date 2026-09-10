---
name: consulting-ppt-creator
description: Create, revise, and visually quality-check polished consulting-style PowerPoint presentations. Use for executive, advisory, strategy, transformation, project-update, or other professional business decks, including restyling existing decks into a clear, restrained consulting visual system.
---

# Consulting PPT Creator

Create a polished consulting presentation with a restrained, professional visual system. Treat user-supplied brand assets as authoritative; otherwise use the default independent consulting style.

## Apply the presentation workflow

1. Read and follow the available `presentations:Presentations` skill, including its content, implementation, rendering, and QA requirements.
2. Read [references/brand-system.md](references/brand-system.md) before planning layouts or choosing colors.
3. Determine the audience, communication job, required decision or action, central takeaway, language, length, and source constraints. Infer reasonable defaults when the request is sufficient; ask only when a missing answer would materially change the deck.
4. Express the communication job internally as: “By the end, [audience] should [outcome] because [central takeaway].” Do not put this production sentence on a slide.
5. Build a cumulative narrative suited to the task. Prefer context → issue → evidence → implications → recommendation → action for advisory decks, while adapting the arc for technical, educational, or status decks.
6. Give every slide one narrative job and one primary claim. Use takeaway-style titles rather than topic labels.
7. Create the `.pptx` using the implementation route required by the presentation skill. Treat this request as explicit custom formatting; do not use the default Codex Grid visual theme.
8. Render and inspect every slide at full size. Fix clipping, overlap, awkward wrapping, inconsistent spacing, weak hierarchy, chart errors, and unresolved placeholders before delivery.

## Select the visual source

Use the first applicable route:

1. **Official template or reference supplied:** Use only that deck or template as the visual source. Preserve its master, typography, palette, spacing, footer, page markers, and brand chrome through the presentation skill’s template-following workflow.
2. **Official assets supplied without a template:** Use the supplied logos, fonts, palette, and guidance exactly as provided. Do not alter or redraw logos.
3. **No official assets supplied:** Apply the independent consulting system in [references/brand-system.md](references/brand-system.md). Do not add or imitate third-party branding.

Never reconstruct a third-party logo from text and shapes. Never invent proprietary fonts, brand rules, client data, credentials, quotes, or business outcomes.

## Shape the content

- Write concise, executive-ready copy in the user’s requested language.
- Use specific claims and active verbs. Keep the tone confident, clear, and human.
- Translate evidence into implications for the audience; do not create fact inventories.
- Prefer one strong composition per slide over dashboards, card grids, pills, or repeated UI panels.
- Use tables only for exact comparisons and charts only when the data supports a meaningful comparison or trend.
- Cite researched facts on-slide or in source notes as appropriate. Distinguish user-provided facts, sourced facts, and assumptions.
- End with a decision, recommendation, action plan, or synthesis that resolves the opening—not a generic “Thank you” page unless requested.

## Default assumptions

When the user does not specify otherwise:

- Use 16:9 widescreen.
- Match the user’s language.
- Target 8–12 slides for a general business deck.
- Use a white-led layout with black typography and restrained green accents.
- Prefer editable native text, charts, tables, and simple shapes.
- Use high-quality, relevant imagery only when it materially improves comprehension.

## Deliver

Return the final `.pptx` only after complete visual QA. Briefly state that the deck uses an independent consulting style when no user-supplied brand package was provided.
