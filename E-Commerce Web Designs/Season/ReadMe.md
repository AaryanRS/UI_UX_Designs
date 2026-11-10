# Season 

## 1. Project Overview
**Season** is an avant-garde digital storefront and editorial showcase balancing high-fashion luxury with the structural discipline of architectural brutalism. Built with an asymmetric 12-column grid, persistent analog grain, massive display typography, and stark monochrome lookbook imagery, the interface commands attention through stark proportions, negative space, and electric micro-interactions.

---

## 2. Visual Design & Aesthetic Language

### Aesthetic Archetype
* **Modern Brutalist Luxury**: Raw surfaces, monospaced metrology data, zero border-radii, architectural line work, and severe contrast paired with high-end luxury editorial sensibilities.
* **Surface Grain Overlay**: Persistent full-screen SVG fractal noise grain overlay (`feTurbulence` with `baseFrequency='0.9'`, `numOctaves='3'`, `opacity: 0.08`, `mix-blend-mode: multiply`) generating a tactile, tangible archival texture across the entire digital canvas.

### Color Palette & Tokens
* **Base Background (Sand / Cement Beige)**: `#E3E2DE` / `#FBF9F5` — Warm neutral architectural concrete tone.
* **Deep Monolith Black**: `#1B0E0D` — High-density brownish-black utilized for hero blocks, high-contrast panels, and primary text.
* **Secondary Earth / Oxide Brown**: `#61220F` — Warm tertiary accent for oversized editorial headings, sub-labels, and callouts.
* **Primary Signal Action (Burnt Red / Ochre)**: `#C72A09` — High-tension primary action button fills, active status indicators, and accent typography.
* **Acid Neon Green (Interaction Accent)**: `#31EF07` — High-visibility micro-interaction accents, animated link underlines, quick-view badges, and submit actions.
* **Structural Divider Lines**: `#D9D9D9` & `rgba(27, 14, 13, 0.15)` — Razor-thin 1px architectural grid rules with zero rounded edges.

---

## 3. Typography Hierarchy

### Primary Fonts
* **Display / Headings**: `Clash Grotesk` (or `Syne` / brutalist heavy geometric grotesque)
  * Weight: 700 / 800 Bold
  * Tracking / Letter-spacing: `-0.04em` to `-0.05em` (ultra-tight)
  * Line-height: `0.75` to `0.85` (compact vertical collision)
  * Hero Scale: `13.5vw` desktop, with staggered indentations (`20vw`) creating rhythmic negative space tension.
* **Editorial Subheadings**: `Syne` / `Clash Grotesk` Medium (`32px`–`48px`) with `3rem` paragraph indentations.
* **Body Copy**: `General Sans` / Inter (Clean grotesque neutral sans-serif) at `14px`–`16px` for reading legibility.
* **Technical Metrology / Archival Data**: `Space Mono` / `JetBrains Mono` / Monospace
  * Formatted with all-caps tracking-widest (`letter-spacing: 0.15em`), brackets (`[SPEC: HW-24-WINTER]`), and serial numbering (`01 // FOUNDATION`).

---

## 4. Layout Architecture & Sections

1. **Sticky Top Navigation Bar**:
   * Utilizes `mix-blend-mode: difference` with `#E3E2DE` text to dynamically invert and remain readable over dark imagery or light backgrounds.
   * Animated link underlines scaling from `scaleX(0)` to `scaleX(1)` with `cubic-bezier(0.165, 0.84, 0.44, 1)`.
2. **Full-Bleed 100vh Hero**:
   * Immersive backdrop image at 60% opacity against `#1B0E0D`.
   * Colossal split-indented headline ("GHOST // VOID LINE") spanning 13.5vw.
   * Monospace metrology specs and burnt-red CTA (`#C72A09`).
3. **Manifesto Grid (12 Columns)**:
   * Cols 1–4: Archival serial metadata, release IDs, and limited commission edition counts.
   * Cols 5–12: High-density editorial statement with highlighted keywords in `#61220F`.
4. **Category Ribbon Divider**:
   * Screen-width horizontal banner bounded by `#D9D9D9` rules with `12vw` "OUTERWEAR" typography.
5. **Asymmetrical Editorial Product Matrix**:
   * Offset column hierarchy: Item 01 occupies 7 columns, while Item 02 occupies 5 columns with a `128px` vertical drop offset.
   * Technical spec data tags (`[SPEC // 100% FELTED WOOL 840GSM]`), hover image scaling (`1.05`), and electric `#31EF07` micro-tags.
6. **Production CAD / Material Rigor Module**:
   * Dark brutalist data matrix with technical metrics (Textile Mass, Thermal Barrier, Industrial Hardware Clasps, Global Allocation Limits).
7. **Runway Chronology & Dispatch Archive**:
   * 3-column brutalist lookbook grid showcasing harsh-contrast monochrome photography.
8. **Industrial Footer & Archival Watermark**:
   * 4-column structured directory, dark newsletter card with neon `#31EF07` action, and an 8vw low-opacity watermark brand imprint.
