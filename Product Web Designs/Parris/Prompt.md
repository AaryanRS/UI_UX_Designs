{
  "$schema": "https://json-schema.org/draft/2020-12/schema",
  "project": {
    "name": "Parris Haute Parfumerie",
    "version": "1.0.0",
    "type": "scroll-choreographed-editorial-landing",
    "device_target": "desktop",
    "theme_mode": "light",
    "design_tokens": {
      "palette": {
        "ground": "#F7F7F4",
        "paper_neutral": "#E4E5E0",
        "paper_light": "#F1F1ED",
        "blush_band_primary": "#F3D6DC",
        "blush_band_secondary": "#F5D9DF",
        "ink_primary": "#070707",
        "accent_dusty_pink": "#EF6F79",
        "secondary_sage": "#B7BAA9",
        "muted_grey": "#999999",
        "stage_dark": "#070707"
      },
      "typography": {
        "primary_font": "Bodoni Moda, serif",
        "accent_font": "Caveat Brush, cursive",
        "rules": [
          "Bodoni Moda handles all core typographic roles including headings, copy, and furniture.",
          "Display tracking between -0.03em and -0.05em.",
          "Small furniture uppercase tracked at +0.18em with 10.5px size.",
          "Caveat Brush strictly rationed to 3 appearances, always in #EF6F79, rotated between -1.5deg and 1.8deg."
        ]
      },
      "geometry": {
        "border_radius": "0px",
        "borders": "1px solid rgba(7, 7, 7, 0.15)",
        "box_shadow": "none",
        "gradients": "none"
      },
      "easing": "cubic-bezier(0.16, 1, 0.3, 1)"
    }
  },
  "layout_stages": [
    {
      "id": "stage_1_multiply_hero",
      "type": "pinned_stage",
      "height": "300svh",
      "pin_properties": {
        "position": "sticky",
        "top": "0",
        "height": "100svh",
        "overflow": "hidden",
        "background": "#F7F7F4"
      },
      "visual_layers": {
        "photo": {
          "subject": "Still life amber perfume flacon on travertine stone slab with dried botanicals",
          "placement": "absolute inset-0 w-full h-full object-cover",
          "blend_mode": "multiply",
          "scroll_scrub": {
            "scale": [1.04, 1.11],
            "translate_y_percent": [0, -3]
          }
        },
        "typography_overlay": {
          "position": "relative z-10 flex flex-col justify-between h-full p-8",
          "elements": [
            {
              "type": "overline",
              "font": "Caveat Brush",
              "color": "#EF6F79",
              "text": "recueillie au crépuscule — harvested at dusk",
              "rotation": "-1.2deg"
            },
            {
              "type": "poster_wordmark",
              "font": "Bodoni Moda",
              "weight": 600,
              "color": "#070707",
              "blend_mode": "normal",
              "text": "PARRIS",
              "formula": "min(clamp(3.5rem, 34vw, 20rem), calc(88vw / (chars * 0.60)))",
              "scroll_scrub": {
                "translate_y_px": [0, -46],
                "opacity": [1.0, 0.0]
              }
            },
            {
              "type": "pinned_straps",
              "count": 3,
              "alignment": "bottom horizontal bar",
              "font": "Bodoni Moda 10.5px tracked +0.18em",
              "items": [
                "EXTRACTION PAR DISTILLATION LENTE",
                "FLACONS EN CRISTAL SOUFFLÉ MAIN",
                "ATELIER GRASSE & PARIS — ÉDITION LIMITÉE"
              ]
            }
          ]
        }
      }
    },
    {
      "id": "statement_band_blush",
      "type": "editorial_band",
      "background": "#F3D6DC",
      "padding": "py-24 px-12",
      "content": {
        "lead_statement": "We formulate not for the salon, but for the skin after twilight — a quiet architecture of resin and rain.",
        "accent_script": {
          "font": "Caveat Brush",
          "text": "harvested at dusk",
          "color": "#EF6F79",
          "rotation": "1.5deg"
        },
        "columns": [
          {
            "num": "01",
            "title": "COLD EXTRACTION",
            "body": "Ninety-day slow maceration conducted within opaque violet-glass carboys to safeguard volatile aldehydes."
          },
          {
            "num": "02",
            "title": "ORGANIC CERTIFIED",
            "body": "Sourced from regions whose microclimates produce private vintages of sweet resinous labdanum."
          },
          {
            "num": "03",
            "title": "NUMBERED SEALS",
            "body": "Every flacon is hand-poured in small batches, wax-dipped with natural beeswax, and inscribed."
          }
        ]
      }
    },
    {
      "id": "stage_2_clip_reveal",
      "type": "pinned_stage",
      "height": "320svh",
      "pin_properties": {
        "position": "sticky",
        "top": "0",
        "height": "100svh",
        "overflow": "hidden"
      },
      "choreography": {
        "clipping_element": {
          "subject": "Fluted glass perfume flacon bathed in morning directional travertine light",
          "clip_path": "inset(0 0 calc(100% - var(--p) * 100%) 0)"
        },
        "headline_overlay": {
          "text": "LIGHT PASSING THROUGH AMBER",
          "font": "Bodoni Moda Italic",
          "color": "#FFFFFF",
          "blend_mode": "difference",
          "scroll_scrub": {
            "opacity": [1.0, 0.0]
          }
        },
        "caption": {
          "text": "Solar macerations capture the transient luminance of Mediterranean resin groves.",
          "reveal_threshold_progress": 0.45
        }
      }
    },
    {
      "id": "catalog_price_band",
      "type": "editorial_band",
      "background": "#E4E5E0",
      "padding": "py-20 px-12",
      "content": {
        "title": "ÉDITIONS & HARVEST RELEASES",
        "table_rows": [
          {
            "code": "PV-01",
            "name": "Cèdre Fumée No. 12",
            "botanicals": "Charred Atlas cedar, wild bergamot rind, smoked benzoin resin, vetiver root",
            "price": "€280"
          },
          {
            "code": "PV-02",
            "name": "Rose d'Octobre No. 04",
            "botanicals": "Drying de Grasse petals, damp earth, crushed pink peppercorn, chilled loam",
            "price": "€320"
          },
          {
            "code": "PV-03",
            "name": "Ambre Souterrain No. 19",
            "botanicals": "Fossilised amber resin, dark vetiver root, raw labdanum, sun-warmed granite",
            "price": "€295"
          },
          {
            "code": "PV-04",
            "name": "Iris de Falaise No. 07",
            "botanicals": "Iron-rich orris root aged three winters, grey musk, sea salt, dry chalk",
            "price": "€360"
          }
        ]
      }
    },
    {
      "id": "stage_3_notes_near_black",
      "type": "pinned_stage",
      "height": "360svh",
      "pin_properties": {
        "position": "sticky",
        "top": "0",
        "height": "100svh",
        "overflow": "hidden",
        "background": "#070707"
      },
      "columns": {
        "left": {
          "title": "The Olfactory Architecture",
          "rows_logic": "floor(var(--p) * 4)",
          "rows": [
            {
              "index": "01",
              "layer": "TOP",
              "notes": "BERGAMOT RIND & GALBANUM",
              "duration": "0 — 40 MINS"
            },
            {
              "index": "02",
              "layer": "HEART",
              "notes": "SMOKED BENZOIN TEARS & DAMASK ROSE",
              "duration": "40 MINS — 4 HRS"
            },
            {
              "index": "03",
              "layer": "BASE",
              "notes": "RAW LABDANUM & CISTUS RESIN",
              "duration": "4 — 14 HRS"
            },
            {
              "index": "04",
              "layer": "FIXATIVE",
              "notes": "VETIVER ROOT & FOSSILISED AMBER",
              "duration": "14 — 36 HRS"
            }
          ]
        },
        "right": {
          "subject": "Extracted crystal flacon still life on dark volcanic slate with raw frankincense tears",
          "scale_scrub": [1.08, 1.00],
          "badge": {
            "text": "ATELIER HARVEST 2024",
            "background": "#EF6F79",
            "color": "#070707"
          }
        }
      }
    },
    {
      "id": "faq_accordion_band",
      "type": "editorial_band",
      "background": "#F5D9DF",
      "padding": "py-20 px-12",
      "content": {
        "script_overline": {
          "font": "Caveat Brush",
          "text": "notes whispered in flint",
          "color": "#EF6F79"
        },
        "title": "QUESTIONS & PROTOCOLE",
        "faqs": [
          {
            "q": "How are the botanical extractions harvested?",
            "a": "Harvested by hand at daybreak across our network of biodynamic partner growers."
          },
          {
            "q": "Why do flacons vary slightly in colour and viscosity?",
            "a": "Because we refuse chemical standardization, seasonal climatic shifts impart unique tones to each vintage."
          },
          {
            "q": "What is the recommended maturation on the skin?",
            "a": "Our pure extractions adapt to your pulse point thermals, blossoming completely between 20 to 60 minutes."
          },
          {
            "q": "International private courier and climate-controlled dispatch.",
            "a": "Every order is packaged in temperature-stabilized insulated cases to preserve volatile essences during transit."
          }
        ]
      }
    }
  ],
  "accessibility": {
    "prefers_reduced_motion": {
      "clip_paths": "disabled; full image displayed directly",
      "blend_modes": "normal blending to prevent disappearing text",
      "transform_scales": "disabled",
      "cumulative_opacity": "all rows rendered at full visibility"
    }
  }
}