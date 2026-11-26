# Softy — Digital Wellness Landing Page

## Overview
**Softy** is a web-first service landing page designed around the philosophy of a **"digital living room"**—a tactile, intentional, and deliberately slow digital sanctuary that counters online overstimulation and hyper-productivity fatigue. 

The experience fuses **Digital Minimalism** with **Gen-Z Lifestyle aesthetics**, prioritizing restorative micro-habits, soothing haptics, and guilt-free mindfulness over rigid streak mechanics and notifications.

---

## Design System & Foundations

### 1. Color Palette
- **Background**: `#FDFCF8` (Warm tactile cream / off-white paper tone)
- **Primary Accent (Peach / Coral)**: `#FFB7B2` (Gentle warmth, primary call-to-actions, pulsing breathing indicator)
- **Sage**: `#E8EFE8` (Morning dew calm, nature grounding)
- **Lavender**: `#EFEDF4` (Evening unwind, ambient dreams)
- **Dark Stone (Primary Text & Contrast)**: `#292524` (High-legibility soft-black, waitlist anchor block)
- **Muted Stone (Secondary Text)**: `#78716C` (Desaturated microcopy, timestamps, and subtitles)
- **Subtle Borders**: `#E7E5E4` / `rgba(231, 229, 228, 0.6)`

### 2. Typography
- **Primary Sans-Serif**: `Outfit`
  - Clean, geometric, softly rounded letterforms.
  - Headings: 48px–72px with tight tracking (`-0.025em`) and strict sentence-case formatting.
- **Expressive Accent**: `Reenie Beanie`
  - Playful, authentic cursive handwriting used for organic emphasis words ("gentle", "touch & breathe", "unfiltered thoughts") and diary signatures.

### 3. Tactile Visual Effects
- **Fractal Noise / Grain Overlay**: Persistent 35% opacity SVG noise filter with `feTurbulence` (baseFrequency 0.65) and `mix-blend-mode: overlay` covering the viewport (`z-index: 50`, `pointer-events: none`) to give the UI an analog, paper-like grain.
- **Organic Geometry**: High border-radius containers ranging from `2rem` (32px) to `4rem` (64px) and full pill shapes (`rounded-full`).
- **Shadows**: Soft ambient elevation `0 4px 20px -2px rgba(0,0,0,0.05)`.
- **Background Blobs**: 60% opacity pastel blobs (`#FFE4E1` and `#E6E6FA`) blurred with `blur-3xl` and running on 6-second low-velocity floating keyframe animations.

---

## Structure & Key Components

1. **Floating Pill Navigation**
   - 70% white opacity with 20px backdrop-blur (`backdrop-blur-md`).
   - Circular Coral `#FFB7B2` logo with a crisp white center dot.
   - Micro links and a dark stone `#292524` pill action button ("Open App").

2. **Center-Aligned Hero Section**
   - Status badge ("• a digital living room").
   - 60px Outfit bold headline with cursive accent text.
   - Dual pill CTA buttons: Primary Coral with ambient glow and Secondary White with 1px stone border.

3. **Horizontal Scenario Scroll**
   - Horizontal snap-scrolling rail showcasing real daily moments (07:15 AM Morning Fog, 02:40 PM Screen Fatigue, etc.) in 288x160px cards with hover accent color transitions.

4. **Cascading App Preview Mockup**
   - Center device viewport with a pulsing `#FFB7B2` "Breathe" button and tactile pacing ring.
   - Cascading preview cards representing ritual journaling and soothing audio soundscapes.

5. **Physical Diary Entry Testimonials**
   - Realistic physical paper notes with slight rotations (`+1°` / `-1°`).
   - Genuine user narratives signed with an authentic 32px rule line and `Reenie Beanie` cursive signatures.

6. **Interactive FAQ Accordion**
   - Fluid expanding/collapsing answers with animated rotating plus-to-close icons.

7. **High-Contrast Dark Waitlist Section**
   - Full-width rounded container in `#292524` with floating ambient gradients, glowing dot insignia, email input, and scale-on-hover submit button.
