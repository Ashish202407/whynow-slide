# Lanmea Capital - Deck Project Context

Last updated: 2026-02-27

---

## Project Overview

Building interactive single-file HTML presentation decks for **Lanmea Capital**, a fund-of-funds focused on India & Southeast Asia private markets (PE/VC). The decks are web-based (not PPT) - horizontal slide navigation, animations, hover effects, and PDF export.

The founder is **Friederike Meyer**. Key team members: Ashish Bahuguna, Laukik Tathed.

---

## Folder Structure

```
/home/ashish/projects/Lanmea/
├── Call recording.txt                          # Transcript of kickoff call with Friederike
├── SESSION-CONTEXT.md                          # This file
├── india-market-appendix.html                  # v1 - original build
├── india-market-appendix-v2.html               # v2 - slide 2 data corrections
├── india-market-appendix-v3.html               # v3 - slide 2 chart + quote box added
├── india-market-appendix-v4.html               # v4 - slide 3 data corrections
├── india-market-appendix-v5.html               # v5 - slide 3 bottom insight box
├── india-market-appendix-v6.html               # v6 - slide 4 split into 4A + 4B
├── india-market-appendix-v7.html               # v7 - slide 4A full-width timeline redesign
├── india-market-appendix-v8.html               # v8 - (previous latest)
├── india-market-appendix-v9.html               # v9 - slide 4A design polish
├── india-market-appendix-v10.html              # v10 - slide 4B rebuilt as card template
├── india-market-appendix-v11.html              # v11 - all green swapped to maroon
├── india-market-appendix-v12.html              # v12 - (incomplete, skip)
├── india-market-appendix-v13.html              # v13 - slide 6 GP ecosystem redesign
├── india-market-appendix-v15.html              # v15 - slide 8 global capital rotation redesign
├── india-market-appendix-v16.html              # v16 - slide 8 enhanced (animated bars, SVG arrows, flags, pill macro)
├── india-market-appendix-v17.html              # v17 - slide 6 rebuilt 3+3 grid + slide 8 from v16
├── india-market-appendix-v18.html              # v18 - all green removed, maroon-only palette
├── india-market-appendix-v19.html              # v19 - text opacity bump (secondary 0.72, muted 0.50)
├── india-market-appendix-v20.html              # v20 - slide 9 rebuilt (dumbbell chart iterations)
├── india-market-appendix-v21.html              # v21 - slide 9 dumbbell chart polish (larger dots, pills, India emphasis)
├── india-market-appendix-v22.html              # v22 - slide 9 dumbbell replaced with SVG slope chart
├── india-market-appendix-v23.html              # v23 (LATEST) - slide 9 full rebuild: two-column card layout
└── Lanmea Friede/
    └── 05.30 Inputs for Claudecode/
        ├── LC logo.svg                         # Full "lanmea capital" wordmark
        ├── LC_logo_royal maroon.svg            # "LC" icon mark (#6B0A14)
        ├── STYLE-GUIDE.md                      # Design system reference
        ├── lanmea-appendix-outline-india-sea.md # Content outline (India + SEA)
        └── style-reference.html                # Working 4-slide example deck (code template)
```

Also created:
```
/home/ashish/projects/0 Deck Learnings/
└── General Deck Building Guide.md             # Generalized deck-building guide (not Lanmea-specific)
```

---

## What's Been Built

### India Market Appendix Deck (11 slides)

| Slide | Type | Title |
|-------|------|-------|
| 1 | Cover (cream) | India Private Markets - Market Context & Data |
| 2 | Light | India - The Macro Opportunity |
| 3 | Cream | India Private Capital - Market Snapshot |
| 4A | Light | Four Decades of Private Capital in India (Foundations) |
| 4B | Cream | Institutional Scale & Maturation |
| 5 | Light | India's Fund Manager Ecosystem |
| 6 | Cream | The Selection Imperative in India |
| 7 | Light | Global Capital Rotation Toward India |
| 8 | Cream | India's Position in Global Private Markets |
| 9 | Light | Why India, Why Now |
| 10 | Back Cover (dark) | India Private Markets |

---

## Version History

### v1 (`india-market-appendix.html`)
- Initial full build of all 10 slides
- All CSS, JS, navigation, logos embedded
- Content from `lanmea-appendix-outline-india-sea.md` (India section only)
- All em dashes / en dashes replaced with "-"

### v2 (`india-market-appendix-v2.html`)
Changes on **slide 2** (India Macro Opportunity):
- Subtitle: "The world's fastest-growing major economy, for the fourth consecutive year" -> "Among the world's fastest-growing major economies"
- GDP label: "GDP - 4th Largest" -> "GDP (2025) - 4th Largest"
- Working age: "65%+" -> "~68%"
- Urban: "~35%" -> "~37%"
- Consumption: "70% of GDP driven by domestic consumption" -> "Consumption ~72% of GDP (HH ~61.5% + Govt ~10.1%)"
- Import cover: added "(latest available)" underneath
- Bottom callout: lowercased "Largest Economy" -> "largest economy"

### v3 (`india-market-appendix-v3.html`)
Changes on **slide 2**:
- Added **Nominal GDP bar chart** below Demographics bullets (left side)
  - 7 bars: 2021-2030E ($3.17T to $7.3T)
  - Solid bars for actuals (2021-2025), hatched/dashed bars for projections (2027E, 2030E)
  - All values labeled above bars
- Added **quote box** below Macro Stability section (right side)
  - Light red tint background (~5% opacity)
  - Maroon quotation mark
  - Quote: "India is moving from 'high-growth' to 'high-growth with improving stability'..."
  - Left-aligned layout with quotation mark on the left

### v4 (`india-market-appendix-v4.html`)
Changes on **slide 3** (India Private Capital - Market Snapshot):
- KPI "Active Funds" -> "Active Funds (IVCA Members)"
- KPI "Combined AUM" -> "Combined AUM (IVCA Members)"
- KPI "Share of APAC PE/VC" -> "Share of Asia-Pacific PE/VC (2024)"
- Bar chart data completely replaced:
  - 2018: $26.3B, 2019: $45.1B, 2020: $62.6B, 2021: $69.8B, 2022: $61.6B, 2023: $39.3B, 2024: $42.9B
- Exit value: removed "$12B (2020) ->", now just "$33B (2024)"
- Public exits: "growing" -> "grew", added "(2023 -> 2024)"
- Global IPO: added "(by Volume)" and "Q1 2025" to heading
- FDI: "since 2000" -> "Since Apr 2000"
- M&A: deleted "deal value up 66% YoY in first nine months"
- Market Signal box: added "(2022 -> 2024)" timeframe
- Fixed bar chart callout colors for 2021 and 2024 (were white/invisible, now green and maroon)

### v5 (`india-market-appendix-v5.html`)
Changes on **slide 3** (India Private Capital - Market Snapshot):
- Added full-width **light red insight box** at the bottom (within slide margins)
  - Paragraph: "India's private capital market is shifting from 'growth-only' to a more institutional regime..."
  - Three bullet points with maroon/green dots: buyout share, exit values, APAC share
  - Matches styling of slide 2 quote box (rgba maroon background, rounded corners)
- Bumped source-note stagger from 6 to 7 to animate after the new box

### v6 (`india-market-appendix-v6.html`)
**Slide 4 split into two slides (4A + 4B):**

**Slide 4A - Foundations** (light):
- Title: "Four Decades of Private Capital in India"
- Subtitle: "How the rails were built (policy -> regulation -> investable structures)"
- Left: 4-era timeline (Late 1980s-2013) with "What happened" / "Why it matters" annotations
  - Color-coded labels: maroon for "What happened", green for "Why it matters"
- Right: "By 2013, the market looked more investable" box with 6 bullets (cream bg, maroon accent)
  - "Net:" conclusion bullet separated with border-top and green dot
- Bottom: Milestone strip with 3 year chips (1991, 1996, 2012) + takeaway quote

**Slide 4B - Institutional Scale & Maturation** (cream):
- Title: "Institutional Scale & Maturation"
- Subtitle: "More strategies, better exits - and sharper dispersion between managers"
- Left: 3-era timeline (2014-Present) with "What changed" / "LP lens" annotations
  - First 2 eras green dots, last era maroon dot (maturation/selection theme)
- Right-top: "What improved structurally" box with 6 bullets (white bg, green accent)
  - Growth bullets green dots, governance bullets maroon dots
- Right-bottom: "So what for LPs" tinted paragraph box (light red bg, italic quote)
- Bottom: 2016 milestone chip (green) + ecosystem note

**Slide 3 bottom box text replaced:**
- Removed old paragraph + 3 bullet points
- New two-paragraph format with color-coded labels:
  - "What's changing:" (maroon) - institutional deal structures, control transactions, liquidity pathways
  - "What it means:" (green) - deeper opportunity set, widening dispersion, manager selection driven outcomes

**Other changes:**
- Deck now 11 slides (was 10)
- Background alternation fixed for slides 5-9 (all swapped to maintain light/cream pattern)
- Card backgrounds in slides 5-9 updated for proper contrast after swap
- Added CSS rules: `.slide-light .mini-card` and `.slide-light .conv-card` use cream bg
- Slide counter updated to 01/11

### v7 (`india-market-appendix-v7.html`)
**Slide 4A redesign** (Foundations) - 2x2 grid layout:
- Layout: `.two-col` grid with 2 eras per column (Eras 1-2 left, Eras 3-4 right)
- Each era uses the deck's signature 3px accent line (maroon for left column, green for right)
- Era titles in Gelasio serif with muted pipe separator
- Content per era: "Context:" (maroon label) + paragraph, 3 bullets (medium-border dots), "Why it matters:" (green label) + paragraph
- Eras within each column separated by subtle `border-top` divider
- All 4 eras rewritten with expanded content
- Below grid: 4 milestone chips (1988, 1991, 1996, 2012) in standard maroon pill style
- Below chips: summary box (~85% width, cream bg, maroon accent line) with paragraph
- Stagger animations: header(1), top eras(2), bottom eras(3), chips(4), box(5), source(6)

### v9 (`india-market-appendix-v9.html`)
**Slide 4A design polish** (Foundations):
- Font sizes bumped across the board: era years 11→13px, era title 9→10px, context label 7→8px, context/bullets/why-it-matters body 8.4-8.6→9.5px
- Increased spacing between bullet list and "Why it matters" box (margin-bottom 8→14px)
- Hover effect: cards now transition to light-red background (`rgba(107,10,20,0.05)`) with maroon-tinted border and shadow
- Milestone chips rearranged: switched from equal-width grid to flex `space-between` so 2012 anchors to far right
- Summary box replaced: removed bordered/gradient box, text is now centered, larger (11px), semi-bold (500), with 3px maroon accent line placed below the text

### v10 (`india-market-appendix-v10.html`)
**Slide 4B rebuilt to match 4A template** (Institutional Scale & Maturation):
- Same `.s4a-grid` 2-column card layout as 4A: 2 cards top row, 3rd card centered below (50% width via `.s4b-3card`)
- 3 era cards: 2014-2016 (green), 2017-2020 (green), 2021-Present (maroon)
- Same card components: Context label + paragraph, 2 bullets each, "Why it matters" box
- Same hover effect (light-red), font sizes, and spacing as 4A
- Card backgrounds adjusted for cream slide (white gradient for contrast)
- Timeline rail with 2 milestone chips: "2016 | Startup India launched" + "2016 | IBC enacted" (same rail format as 4A)
- Summary paragraph centered below, no accent line
- **Also on 4A**: removed the small vertical maroon accent line from summary
- All content updated per user-provided text

### v11 (`india-market-appendix-v11.html`)
**All green swapped to maroon** across entire deck:
- CSS variable `--green` changed from `#1D3B29` to `#6B0A14`
- All hardcoded `rgba(29,59,41,...)` replaced with `rgba(107,10,20,...)`
- One hardcoded `#1D3B29` hex replaced
- Deck is now fully monochrome in brand maroon

### v13 (`india-market-appendix-v13.html`)
**Slide 6 (GP Ecosystem) fully redesigned**:
- Title: "India's Fund Manager Ecosystem"
- Subtitle: "Domestic fundraising has reached global scale, the manager universe is broader, and outcomes are increasingly selection-driven"
- **Top row**: 2 hero proof-point boxes
  - Left: "Domestic Scale" — Kedaara $1.73B (2024) + ChrysCapital ~$2.2B (2025) as large Gelasio numbers
  - Right: "AIF Platform Scale" — 3 stats in tinted cells ($189.7B commitments, $81.8B raised, $77.7B invested)
- **Bottom row**: 3 equal cards with 3px maroon top accent + hover effect
  - "Manager Breadth" — ~60-65% hero stat + 2 bullets
  - "Performance-Led Fundraising" — ~190% vs ~80% Q1/Q4 visual comparison blocks
  - "Emerging Manager Pipeline" — ~28% hero stat + 2 bullets
- **Summary**: centered text (11px, weight 500) about selection > exposure
- New CSS classes: `.gp-hero-*`, `.gp-fund-*`, `.gp-aif-*`, `.gp-card-*`, `.gp-vs-*`
- Slide 4A title changed to "India's Private Capital Foundations"
- Slide 4B title changed to "Institutional Scale-Up"
- Slide 4B chips updated: 4 chips (2016 Startup India, 2017 GST, 2021 peak, 2023 correction)
- Slide 4B 3rd card left-aligned (not centered)

### v15 (`india-market-appendix-v15.html`)
**Slide 8 redesigned** (Global Capital Rotation Toward India):
- Title: "Global Capital Rotation Toward India"
- Layout: 60/40 grid — hero chart left, GP tiles right
- **Hero chart**: Clustered bar chart showing $100M+ deals by 7 global managers (2014-18 avg vs 2024)
  - India: 8 → 15 (1.9x), Japan: 4 → 7 (1.8x), Greater China: 11 → 3 (-73%)
  - Maroon bars for 2024, muted bars for 2014-18 avg, legend + footnote
- **GP tiles**: 4 commitment boxes (Carlyle ~30-35%, Bain Capital ~$10B, Blackstone ~$100B, KKR ~$20B)
  - Numbers-first layout: big Gelasio figure + 1-line descriptor, hover effect
- **Macro strip**: FDI equity inflows $50.0B (FY25) + $35.18B Apr-Sep FY26 (+18% YoY)
- **Takeaway**: "As global capital concentrates in India, access + selection discipline become the key edge."
- New CSS classes: `.gcr-layout`, `.gcr-chart-*`, `.gcr-cluster-*`, `.gcr-bar-*`, `.gcr-tile-*`, `.gcr-macro-*`

### v16 (`india-market-appendix-v16.html`)
**Slide 8 enhanced** (Global Capital Rotation Toward India):
- Animated bar growth from zero (scaleY via `gcr-growBar` keyframes, staggered per cluster)
- SVG curve arrows above each cluster with draw-in animation (`gcr-drawLine`) + delta labels (1.9x, 1.8x, -73%)
- Country flag SVGs in circular badges (India tricolor, Japan sun, China star)
- Background flow SVG — subtle directional sweep curves (`gcr-flow-bg`)
- GP tiles: slide-in-from-right animation (`gcr-slideRight`), 3px maroon left border accent
- Macro pill: rounded pill shape with gradient background, green arrow YoY badge (`gcr-yoy-badge`)
- Pull-quote takeaway: italic Gelasio with 3px maroon left border (`gcr-pullquote`)
- Chart wrap: box-shadow, white bg, fade-up animation on slide active

### v17 (`india-market-appendix-v17.html`)
**Slide 6 rebuilt** (India's Fund Manager Ecosystem) — 3+3 grid layout:
- Subtitle updated: "Domestic fundraising has reached global scale, competition is structurally deeper, and fundraising is increasingly performance-led"
- `.gp-hero-row` changed from 2-column to 3-column grid
- **Top row — 3 hero blocks:**
  - "Domestic Scale" — Kedaara $1.73B + ChrysCapital ~$2.2B, italic supporting line
  - "Competition Deepening" — horizontal bar chart (~110 in 2016 vs ~175 in 2024), ~60% callout
  - "Domestic Fundraising Engine" — ~$6B → ~$8B stat tiles with arrow, "~30% step-up" pill badge, cadence line
- **Bottom row — 3 cards:**
  - "Onshore Capability" — 2x hero stat, "Local execution infrastructure" accent-line item
  - "Performance-Led Fundraising" — ~190% vs ~80% comparison, italic dispersion signal line
  - "Emerging Manager Pipeline" — ~28% hero stat, 2 accent-line bullets (maiden funds + "Alpha source")
- **Summary**: centered text with 40px maroon accent line above
- CSS spacing: hero-row gap 14px, card-row gap 14px, row gap 18px, card padding 20px 22px 18px

**Slide 8 reverted to v16 design** (Global Capital Rotation Toward India):
- Animated bars, SVG curve arrows, country flags, background flow SVG
- Pill-shaped macro strip with green YoY badge
- Pull-quote takeaway with maroon left border
- Full keyframe animations: gcr-fadeUp, gcr-fadeIn, gcr-growBar, gcr-drawLine, gcr-slideRight

### v18 (`india-market-appendix-v18.html`)
**All green removed from entire deck** — maroon-only color palette:
- **Slides 2 & 3**: GDP bar chart bars, Deal Value Trajectory bars, section labels, section underlines, accent lines, "Market Signal" label, "What it means" label — all green → maroon
- **Slide 4A CSS**: Timeline line gradient, `.tl-green` dot/hover, `.s4-era-card.s4-green` accent, `.s4-why` box bg/border/label, timeline rail gradient, `.s4a-node.s4-node-green` dot/year
- **Slide 4B CSS**: `.s4b-stage.s4b-green` left bar, `.s4b-stage .label-green`, `.s4b-panel-head .line`, `.s4b-pill.s4-good` border/bg
- **Slide 6 CSS**: `.s6-card.s6-green` accent/kicker, `.s6-band-vc` and `.s6-band-buyout` gradients, `.s6-stat-value.s6-up`
- **Global CSS**: `.pill-green` now renders in maroon
- **Slide 1 (Cover)**: decorative line hex `#1D3B29` → `#6B0A14`
- **Slide 8 (India in Global Context)**: "APAC PE Buyout" section label/underline, accent line, "India + SEA" label
- CSS variable `--green: #1D3B29` definition retained (unused) for reference

### v19 (`india-market-appendix-v19.html`)
**Text opacity bump** across entire deck:
- `--text-secondary` opacity: 0.65 → 0.72
- `--text-muted` opacity: 0.40 → 0.50
- Improves readability of body text and labels without changing the color system

### v20 (`india-market-appendix-v20.html`)
**Slide 9 rebuilt** (India's Position in Global Private Markets):
- Dumbbell chart added showing 2019-23 avg vs 2024 deal values for 6 APAC markets
- Hero metrics bar: $176B APAC PE Deal Value, ~20% India share, ~0.3% Asia PE/VC-to-GDP
- Bottom insight cards with accent-line items
- Overflow fixes applied: cards margin-top 16→10px, card padding 18px 20px → 14px 16px, summary margin-top 16→8px

### v21 (`india-market-appendix-v21.html`)
**Slide 9 dumbbell chart polish**:
- Dot size increased to 12px (India 14px), line thickness to 3px
- Value labels repositioned beside dots (same Y level) with 6px gap using `left:calc(P% ± 12px)`
- % change labels wrapped in pill badges (`background:rgba(107,10,20,0.06);border-radius:10px`)
- India row emphasis: tinted background `rgba(107,10,20,0.04)`, maroon label, larger dots
- Bottom cards padding increased to 18px 20px, margin-top 12px
- Summary font-size 11→12.5px, margin-top 8→9px

### v22 (`india-market-appendix-v22.html`)
**Slide 9 dumbbell chart replaced with SVG slope chart**:
- Two vertical axes at 15% (2019-23 avg) and 85% (2024) connected by angled lines per country
- India highlighted: 3px maroon hero line, 9px dots, tinted background band `rgba(107,10,20,0.015)`
- Other countries: 1.5-2px faint lines, 7px dots
- Change labels (-47%, -17%) centered at line midpoints
- HTML labels overlaid on SVG via absolute positioning (`right:calc(85% + 12px)` for left, `left:calc(85% + 12px)` for right)
- Bottom 3 countries offset vertically to prevent label collision

### v23 (`india-market-appendix-v23.html`) - LATEST
**Slide 9 complete rebuild** — two-column card layout replacing slope chart:
- **Layer 1 (Hero metrics bar)**: $176B APAC PE Deal Value (2024), ~20% India share (up from ~15% in 2018), ~0.3% Asia PE/VC-to-GDP vs ~1.1% North America
- **Layer 2 (Two-column cards)**:
  - Left card "APAC Positioning": 6-country horizontal bar chart (Greater China $47B, India $38B, Aus-NZ $33B, Japan $22B, South Korea $20B, SEA $16B), accent-line insight on share shift, footnote
  - Right card "Global Context": 3-region PE/VC-to-GDP bars (North America 1.1%, Europe 0.4%, Asia 0.3%), runway callout box ("India: $4.19T economy, ~$43B annual PE-VC"), two accent-line items (low penetration + nascent asset classes)
- **Layer 3 (Summary)**: "India is APAC's second-largest PE market and gaining share. Globally, private markets penetration remains a fraction of developed markets — the structural runway is long."
- Cards use edge-col-card pattern: 18px radius, 28px padding, 3px maroon top accent strip
- Sources: Bain APAC PE Report 2025, AVCJ, IMF WEO, OECD, Preqin, Deloitte APAC PE Almanac 2025

---

## What's NOT Done Yet

### Southeast Asia Deck (7 slides)
The content outline exists in `lanmea-appendix-outline-india-sea.md` (Section 2) but no HTML has been built yet. Slides planned:
- S-1: SEA - The Macro Opportunity
- S-2: SEA Private Capital - Market Snapshot
- S-3: SEA's Private Capital Journey (history)
- S-4: SEA's Fund Manager Landscape
- S-5: Why Selection Matters Even More in SEA
- S-6: Global Capital and SEA
- S-7: Why SEA, Why Now

### Other Items from the Call
- **Main deck summary slide**: "Why India and Southeast Asia Now" slide for the main deck (summary of the appendix)
- **Data room**: password-protected web page for LPs (future phase)
- **Investor portal**: LP login portal on website (future phase)
- **Analytics/tracking**: Clarity integration for engagement tracking (future phase)

---

## Design System Quick Reference

- **Primary accent**: Maroon `#6B0A14` (all themes — credit discipline, risk, governance, value creation, growth)
- **Secondary accent**: ~~Green `#1D3B29`~~ removed from v18 onward — deck is now monochrome maroon
- **Backgrounds**: White `#FFFFFF` (light slides), Cream `#F4F7F3` (alternate slides), Dark `#241818` (back cover)
- **Fonts**: Gelasio (serif, headings/numbers), Inter (sans, body/labels)
- **Body text weight**: 300 (light)
- **Slide padding**: 88px top, 100px sides, 60px bottom
- **Reference height**: 810px (scaled via JS)
- **Architecture**: Single-file HTML, embedded base64 logos, Google Fonts only external dependency

---

## Key Decisions Made

1. **All em/en dashes replaced with hyphens "-"** across the deck
2. **India deck first**, SEA deck later
3. **Bar charts preferred** over SVG line charts (line charts had rendering issues)
4. **Light backgrounds only** for appendix decks (per style guide)
5. **Versioned copies** (v1, v2, v3, v4) rather than overwriting - allows rollback
6. **Data corrections applied incrementally** - Friederike/team providing updated numbers per slide
