# Parris Haute Parfumerie — Editorial Landing Page

A scroll-choreographed, high-fashion editorial digital experience for **Parris**, an artisanal haute parfumerie. The interface blends classical French Didone typographic hierarchy with modern scroll-linked choreography, atmospheric still-life photography, and tactile editorial composition.

---

## 1. Project Brief & Overview

- **Brand:** Parris — Haute Parfumerie & Botanical Extraction Atelier
- **Archetype:** Luxury Editorial / Niche Perfumery Commerce & Archive
- **Platform:** Responsive Desktop Web (with mobile-adaptive layouts)
- **Concept:** Translating physical perfumery architecture—resins, tinctures, amber glass, and raw botanical harvests—into a sequential, cinematic digital reading experience.

---

## 2. Visual Design & Atmosphere

### 2.1 Aesthetic Language
- **Didone Editorial Register:** Inspired by classical high-fashion monographs and heritage French perfumery gazettes.
- **Strict Geometric Restraint:** Hairline borders (`1px solid`), zero border radii (`rounded-none`), sharp box geometry, zero drop shadows, and zero synthetic gradients.
- **Warm Tactility:** Photography is layered using blending modes (`mix-blend-mode: multiply`) directly over natural plaster grounds so that typography and texture co-exist as physical ink on textured paper.

---

## 3. Color Palette & Token Architecture

| Role | Color Name | Hex Code | Description & Usage |
| :--- | :--- | :--- | :--- |
| **Ground** | Plaster Off-White | `#F7F7F4` | Primary global background; natural mineral ground. |
| **Paper Tint 1** | Linen / Paper Neutral | `#E4E5E0` | Band backgrounds for catalog tables & technical sheets. |
| **Paper Tint 2** | Warm Vellum | `#F1F1ED` | Low-contrast structural card containers. |
| **Blush Band 1** | Soft Rose Blush | `#F3D6DC` | Heroic statement background band and philosophy modules. |
| **Blush Band 2** | Warm Quartz Blush | `#F5D9DF` | Secondary tinted module ground for protocol FAQs. |
| **Ink** | Near-Black Ink | `#070707` | Deepest typographic ink for high-contrast Bodoni glyphs. |
| **Dark Stage** | Chiaroscuro Noir | `#070707` / `#050505` | Stage 3 olfactory architecture backdrop. |
| **Accent** | Dusty Pink | `#EF6F79` | Dominant accent: script touches, prices, active note pills. |
| **Secondary** | Sage Herbarium | `#B7BAA9` / `#AEB1A0` | Subtle hairline dividers and botanical metadata tags. |
| **Muted** | Studio Grey | `#999999` | Secondary metadata labels and small-caps tracking. |

---

## 4. Typography System

### Primary Typeface: Bodoni Moda (Variable Font)
- **Role:** Carries 98% of the typographic workload across the entire page.
- **Scale & Treatments:**
  - **Poster Wordmark:** `font-size: min(clamp(3.5rem, 34vw, 20rem), calc(88vw / (chars * 0.60)))`, weight 600, letter-spacing `-0.05em`, line-height `0.8`.
  - **Display Headlines:** Editorial Didone roman and italic pairings, font weights 400 to 600.
  - **Tracking Hierarchy:** Display headlines tracked tightly (`-0.03em` to `-0.05em`).
  - **Furniture & Folio:** Micro-labels, date stamps, and coordinates set in uppercase small caps at `10.5px`, tracked widely at `+0.18em` to `+0.20em`, weight 500.

### Secondary Accent: Caveat Brush
- **Role:** The expressive, organic human signature contrasting Didone formality.
- **Rationing Rule:** Strictly limited to **3 key moments** on the entire page.
- **Color & Rotation:** Always styled in Dusty Pink (`#EF6F79`) with subtle manual tilt (`-1.5deg` to `+1.8deg`).

---

## 5. Animation, Scroll Choreography & Physics

The page is built around **three tall pinned stages** interleaved with fluid editorial sections, driven by a single requestAnimationFrame-throttled scroll observer:

### Stage 1: The Multiply Hero (300svh Pin)
- **Structure:** `position: sticky; top: 0; height: 100svh; overflow: hidden;`
- **Imagery:** Still-life amber perfume flacon with `mix-blend-mode: multiply` set across the plaster ground.
- **Scrub Behavior:**
  - Image smoothly scales from `1.04` to `1.11` while drifting upward `3%`.
  - Poster Didone typography floats above the photograph without blending, creating an illusion of letterforms pressed into the amber glass.
  - Headline lifts `46px` and gently fades out as scroll progress advances from `0.0` to `1.0`.

### Stage 2: Bottom-Up Clip-Path Reveal (320svh Pin)
- **Structure:** `position: sticky; top: 0; height: 100svh;`
- **Choreography:**
  - Second flacon still life wipes upward from the bottom edge via dynamic clipping:  
    `clip-path: inset(0 0 calc(100% - var(--p) * 100%) 0)`.
  - **Difference Blending Headline:** Centered title *"LIGHT PASSING THROUGH AMBER"* set in `mix-blend-mode: difference; color: #FFFFFF;`, inverting gracefully against both the light plaster ground and climbing dark photo contours.
  - **Delayed Caption:** Caption block stays hidden until `--p >= 0.45`, preventing empty-ground layout artifacts.

### Stage 3: Cumulative Olfactory Notes (360svh Pin)
- **Structure:** 2-column chiaroscuro stage set on near-black `#070707`.
- **Right Column:** Dramatic extraction flacon photography scaling gently downward from `1.08` to `1.00`.
- **Left Column:** Four formulation layers (Top, Heart, Base, Fixative) lighting up cumulatively based on scroll calculation `floor(p * 4)`:
  - Inactive rows stay subdued at `opacity: 0.28`.
  - Active rows transition into crisp white Didone with dusty pink index markers and right-aligned extraction durations.

### Micro-Staggers & Intersection Observers
- **Word-Level Rise:** Splitting headlines into inline-block spans with a `38ms` stagger rising `0.4em`.
- **Data-Reveal Orchestration:** Editorial table rows and details summaries carry staggered entrance offsets calculated via `cubic-bezier(0.16, 1, 0.3, 1)`.
- **Accessibility:** Full `prefers-reduced-motion` fallbacks that unclip all images, normalize blending modes, and display static composition rows.
