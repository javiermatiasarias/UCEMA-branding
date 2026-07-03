# UCEMA MBA Design System

Design system for MBA course presentations at Universidad del CEMA (UCEMA), Buenos Aires, Argentina.
Built from the official brand book (UCEMA_BrandBook_V2022_02_Institucional.pdf) and the institutional PowerPoint template (Pesentacion_Institucional_UCEMA.pptx).

---

## Sources
- `uploads/Pesentacion_Institucional_UCEMA.pptx` — official slide template
- `uploads/UCEMA_BrandBook_V2022_02_Institucional.pdf` — brand guidelines
- `uploads/logo.svg` — original UCEMA logo (phoenix crest + wordmark) → copied to `assets/logo.svg`

---

## Content Fundamentals

**Language:** Spanish (Argentine). Titles use sentence case. No emoji. Formal but not stiff.
**Tone:** Authoritative, precise, evidence-based. Aligned with economics, technology, innovation, science.
**Copy style:** Concise bullets; avoid full sentences in slides. Titles are declarative or question-form.
**Casing:** Sentence case for titles (NOT ALL CAPS unless for emphasis or section numbers).

---

## Visual Foundations

### Colors
Primary brand color is **crimson `#940028`** — a deep, rich red extracted directly from the logo SVG.
Two background families:
- **Light** — white `#FFFFFF` with crimson accents (standard content slides)
- **Crimson** — solid `#940028` (section dividers, high-impact slides)
- **Dark/Tech** — deep navy-slate `#0D1218` (modern, technology-forward slides — an intentional extension of the brand for MBA tech/innovation contexts)

Crimson is used for: titles on white, all accent lines/rules, logo block background, bold highlight text.
Dark navy is used for: tech-forward content, data-heavy slides, "modern science" aesthetic.

### Typography
**Primary font:** Barlow + Barlow Condensed (Google Fonts)
> ⚠️ Substitution note: The original brand uses **Acumin Pro** (Adobe). Barlow is the closest freely available alternative — same humanist-grotesque proportions, similar weight range. Replace with Acumin Pro if a license is available.

- **Display/headings:** Barlow Condensed 700–800 — punchy, authoritative, space-efficient
- **Body/bullets:** Barlow 400–600 — clean, readable at 22–28px

### Layout
- Slide dimensions: **1280 × 720 px** (16:9)
- Standard horizontal inset: 80px
- Standard vertical inset: 64px
- Logo always appears in a crimson block (`#940028` background). Standard positions: bottom-left (cover), top-right sidebar (section/content), bottom-right (closing).

### Slide backgrounds
Two main backgrounds for variety:
1. White — most content slides
2. Crimson `#940028` — section openers, quotes, high-impact moments
3. Dark `#0D1218` — tech/data slides (modern extension)

### Accent elements
- 3px horizontal or vertical crimson line (`#940028`) as section separator / title underline
- Subtle large watermark letterform ("U" or section number) in near-invisible dark tint on crimson/dark slides
- Logo block always shown — never omit it

### Corners & Borders
- No rounded corners. All geometric, sharp (border-radius: 0).
- Cards/callouts: thin 1px crimson left border, or full crimson bg.

### Shadows
None. Flat design. Depth via color contrast and whitespace only.

### Animation
Slides are static. No transitions in the design system itself.

### Imagery
- Photography: cool/neutral tone, people in academic/professional settings.
- Avoid busy or colorful stock photography — let the brand colors lead.
- Placeholder slots used in templates; drop real imagery to fill.

---

## ICONOGRAPHY
- No dedicated icon system in the official brand.
- Lucide Icons (CDN) used as a supplement for data/tech slides where icons are needed.
- Unicode geometric shapes (▶ ◆ —) may be used sparingly as bullet replacements.
- No emoji.

---

## File Index

```
assets/
  logo.svg              ← UCEMA logo (phoenix crest + wordmark, crimson bg)
  image2.jpeg           ← Cover slide background (dark crimson)
  image3.jpeg           ← Section slide background (crimson gradient)
  image4.jpeg           ← Content slide background (white + gray sidebar)
  image5.jpeg           ← Closing slide (white)

tokens/
  colors.css            ← All CSS custom properties for color
  typography.css        ← Font imports + type scale tokens
  spacing.css           ← Spacing scale + slide layout tokens

styles.css              ← Root entry (imports all tokens)

guidelines/
  colors-primary.card.html    ← Crimson brand palette
  colors-neutral.card.html    ← Neutrals + dark tech palette
  type-display.card.html      ← Display type specimens
  type-body.card.html         ← Body type specimens
  brand-logo.card.html        ← Logo usage & clearspace

slides/
  01-cover.card.html          ← Cover / title slide
  02-section.card.html        ← Section divider
  03-content.card.html        ← Standard content (white)
  04-dark.card.html           ← Dark/tech slide
  05-twocol.card.html         ← Two-column layout
  06-quote.card.html          ← Full-bleed quote slide
  07-closing.card.html        ← Closing / thank you
```

---

## Intentional Additions vs. Brand Book
| Addition | Reason |
|---|---|
| Dark navy (`#0D1218`) background | Modern tech/innovation look the user requested |
| Barlow font | Free substitute for licensed Acumin Pro |
| Barlow Condensed for display | More impact at large slide sizes |
| Two-column slide layout | Common MBA teaching need not in original template |
| Quote slide | High-impact moments, not in original template |
