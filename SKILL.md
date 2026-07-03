---
name: ucema-mba-design
description: Use this skill to generate well-branded slide presentations and academic materials for Universidad del CEMA (UCEMA) MBA courses. Contains brand colors, typography, logo assets, and slide templates aligned with the UCEMA identity — modernized for technology, science and innovation contexts.
user-invocable: true
---

Read the README.md file within this skill, and explore the other available files.

When creating slide presentations or MBA course materials:
- Use crimson #940028 as the primary brand color
- Use Barlow / Barlow Condensed as the font (substitute for Acumin Pro)
- Include the UCEMA logo (assets/logo.svg) on every slide — placed in a crimson block
- Reference the slide templates in slides/ for layout patterns
- Dark slides (#0D1218) are approved for tech/innovation/data contexts
- All slides are 1280×720px (16:9)

If the user invokes this skill without other guidance, ask what course/topic the presentation covers, how many slides, and whether they want the light, crimson, or dark background style — then build a full deck using the dc_write tool and deck_stage.js.
