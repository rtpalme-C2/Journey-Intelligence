# Journey Intelligence — Brand System

## Identity
- **Project name:** Journey Intelligence
- **Chapter:** Life Stuff · Chapter 2 · Travel Advisory
- **Tagline:** Advisory · Curation · Insight

## Palette — Warm Brown / Brass

| Token | Hex | Usage |
|-------|-----|-------|
| `--night-slate` | `#1E1609` | Primary dark, page headers, body text |
| `--deep-steel` | `#2E2410` | Accent, table headers |
| `--steel` | `#6C500F` | Mid UI, secondary labels, hotel meta |
| `--warm-silver` | `#B8900C` | Text on dark backgrounds, accents |
| `--silver-mist` | `#D4AE3A` | Subtle rules and highlights on dark |
| `--paper` | `#F5F2EC` | Page background (light mode) |

**Role assignments:**
- Dark → Night Slate `#1E1609`
- Light → Paper `#F5F2EC`
- Accent → Deep Steel `#2E2410`

## Typography
- **Font:** Plus Jakarta Sans
- **Weights:** 200, 300, 400, 500, 600, 700 + italics
- **Eyebrow text:** uppercase, wide letter-spacing (0.2em+)
- **Display titles:** weight 200–300 (ultra-light, elegant)
- **Body text:** weight 400
- **Labels/meta:** weight 500–600

## Icon Mark — Meridian
- Vertical ellipse rx=9 ry=21 — the hero, always in Warm Silver `#B8900C`
- Globe circle r=21, faint — recedes into background
- Equator: full-width horizontal line, silver, slightly lighter than meridian
- 2 latitude hints above/below equator — tinted to bg color, clearly secondary
- Datum point: silver fill, dark center punch (r=2.4 outer, r=1 inner)
- **Avoided:** planes, compasses, maps, globe-as-primary — all read as airport
- Warm Silver is NOT cold chrome — it carries warmth consistent with the system

## Proposal Format
- **Tool:** HTML → PDF via Playwright (Chromium)
- **Page size:** US Letter (8.5 × 11in)
- **Margins:** 0.65in left/right, 0.6in top/bottom
- **Template file:** `proposal-template.html`
- **Two proposal types supported:**
  - Drivable — budget boxes, drive pill tag
  - Fly-to — weekend vs. weekday comparison table, flight pill tag
- **Section divider pages** separate trip types within combined documents

## File Naming Convention
- `McKinley_Cupp_Getaway_Trip_Ideas.pdf` — combined drivable + fly-to couples proposals
- `McKinley_Cupp_FollowUp_Ideas.pdf` — rail and cruise informational doc
- Source HTML files mirror PDF names

## Notes
- Always use HTML→PDF pipeline, never ReportLab
- Palette is warm brown/brass — NOT cool blue-grey
- Plus Jakarta Sans must be loaded from Google Fonts
- Print background must be enabled when rendering PDF
