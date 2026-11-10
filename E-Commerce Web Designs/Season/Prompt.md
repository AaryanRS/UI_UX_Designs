{
  "project": {
    "name": "Season 04",
    "version": "1.0.0",
    "theme": "Modern Brutalist Luxury",
    "category": "E-Commerce / Luxury Fashion Editorial",
    "target_device": "desktop"
  },
  "aesthetic_specification": {
    "style_archetype": "Modern Brutalism / Technical Utilitarian Luxury",
    "viewport_texture": {
      "type": "svg_fractal_noise",
      "filter_tag": "feTurbulence",
      "base_frequency": 0.9,
      "num_octaves": 3,
      "opacity": 0.08,
      "mix_blend_mode": "multiply",
      "position": "fixed",
      "z_index": 50,
      "pointer_events": "none"
    },
    "color_palette": {
      "background_primary": "#E3E2DE",
      "surface_dark": "#1B0E0D",
      "text_primary": "#1B0E0D",
      "text_editorial_accent": "#61220F",
      "action_primary": "#C72A09",
      "micro_interaction_neon": "#31EF07",
      "border_subtle": "#D9D9D9",
      "border_dark": "rgba(27, 14, 13, 0.15)"
    },
    "typography": {
      "display_heading": {
        "family": "Clash Grotesk, Syne, sans-serif",
        "weight": "700",
        "letter_spacing": "-0.04em",
        "line_height": "0.85",
        "case": "uppercase"
      },
      "editorial_subheading": {
        "family": "Syne, Clash Grotesk, sans-serif",
        "weight": "500",
        "size_range": "32px - 48px",
        "paragraph_indent": "3rem"
      },
      "body": {
        "family": "General Sans, Inter, sans-serif",
        "size": "15px",
        "line_height": "1.6"
      },
      "metrology_technical": {
        "family": "Space Mono, JetBrains Mono, monospace",
        "weight": "400",
        "letter_spacing": "0.15em",
        "case": "uppercase",
        "format": "bracketed_coordinates_and_specs"
      }
    }
  },
  "layout_modules": [
    {
      "module_id": "global_navigation",
      "type": "sticky_top_bar",
      "blend_mode": "difference",
      "text_color": "#E3E2DE",
      "elements": {
        "brand_logo": { "text": "SEASON 04", "weight": "800", "size": "24px" },
        "links": ["SHOP", "EDITORIAL", "ARCHIVE", "MANIFESTO"],
        "hover_state": {
          "style": "bottom_underline",
          "color": "#31EF07",
          "thickness": "2px",
          "easing": "cubic-bezier(0.165, 0.84, 0.44, 1)"
        },
        "utility_actions": ["SEARCH [88K]", "BAG (02)"]
      }
    },
    {
      "module_id": "hero_cover",
      "type": "split_indented_hero",
      "height": "100vh",
      "background_color": "#1B0E0D",
      "background_media": {
        "type": "grayscale_high_contrast_photography",
        "opacity": 0.6,
        "mood": "raw concrete brutalist architecture with avant-garde outerwear"
      },
      "headline": {
        "size": "13.5vw",
        "line_1": { "text": "GHOST", "align": "left", "color": "#E3E2DE" },
        "line_2": { "text": "VOID LINE", "indent": "20vw", "color": "#C72A09" }
      },
      "bottom_dock": {
        "specs": "[SPEC: HW-24-WINTER] // RAW STRUCTURAL ARMOR",
        "cta": {
          "label": "EXPLORE COLLECTION [ \u2193 ]",
          "background": "#C72A09",
          "color": "#FFFFFF",
          "border_radius": "0px"
        }
      }
    },
    {
      "module_id": "manifesto_statement",
      "type": "asymmetric_12_column_grid",
      "columns_1_to_4": {
        "role": "technical_metadata",
        "items": [
          "RELEASE ID: S7-04-DE_2026",
          "ARCHIVE CODE: BRUT-VOL-09",
          "CONSTRUCTION: MONOLITHIC ARMORED",
          "LIMITED COMMISSION RUN OF 120 TOTAL UNITS"
        ]
      },
      "columns_5_to_12": {
        "role": "large_editorial_text",
        "highlight_color": "#61220F",
        "statement": "WE REJECT ORNAMENTATION IN PURSUIT OF PURE FORM. SEASON 04 EXCAVATES STRUCTURAL SILHOUETTES FROM BRUTALIST ARCHITECTURAL PRECEDENTS."
      }
    },
    {
      "module_id": "category_ribbon",
      "type": "full_width_typography_divider",
      "title": "OUTERWEAR",
      "font_size": "12vw",
      "color": "#61220F",
      "borders": { "top": "1px solid #D9D9D9", "bottom": "1px solid #D9D9D9" }
    },
    {
      "module_id": "product_matrix",
      "type": "asymmetrical_grid",
      "card_01": {
        "width_columns": 7,
        "aspect_ratio": "4:5",
        "title": "01 | ARCHITECTURAL TRENCH COAT",
        "price": "\u20ac1,850",
        "spec": "100% FELTED HEAVYWEIGHT WOOL // CUSTOM CAST ZINC BUCKLES"
      },
      "card_02": {
        "width_columns": 5,
        "aspect_ratio": "3:4",
        "vertical_offset_top": "128px",
        "title": "02 | COCOON PUFFER JACKET",
        "price": "\u20ac1,420",
        "spec": "MEMBRANE RIPSTOP // HIGH-NECK COLLAR // GOOSE DOWN 90:10"
      },
      "interactive_behaviors": {
        "image_hover": "scale(1.05)",
        "badge": {
          "label": "QUICK VIEW",
          "background": "#31EF07",
          "color": "#1B0E0D"
        }
      }
    },
    {
      "module_id": "cad_metrology_module",
      "type": "dark_matrix_spec_sheet",
      "background": "#1B0E0D",
      "metrics": [
        { "label": "01 | TEXTILE MASS", "value": "840", "unit": "GSM DENSITY HEAVY FELTED WOOL" },
        { "label": "02 | THERMAL BARRIER", "value": "800+", "unit": "FILL POWER ETHICALLY SOURCED DOWN" },
        { "label": "03 | INDUSTRIAL CLASPS", "value": "Z-12", "unit": "DIE-CAST ZINC ALLOY QUICK CLAMPS" },
        { "label": "04 | GLOBAL ALLOCATION", "value": "120", "unit": "NUMBERED UNITS GLOBALLY" }
      ]
    },
    {
      "module_id": "lookbook_chronology",
      "type": "3_column_dispatch_archive",
      "image_style": "monochrome_brutalist_editorial",
      "captions": ["PARIS SALON 14:00 [ARCHIVED]", "BERLIN KRAFTWERK 21:00 [ARCHIVED]", "TOKYO DISPATCH 04:00 [CURRENT]"]
    },
    {
      "module_id": "footer",
      "type": "industrial_brutalist_footer",
      "columns": ["FOUNDATION", "DIRECTORY", "PROTOCOL", "DISPATCH NEWSLETTER"],
      "newsletter": {
        "background": "#1B0E0D",
        "input_style": "minimal_underline",
        "submit_action": { "label": "SEND \u2192", "background": "#31EF07" }
      },
      "ghost_watermark": {
        "text": "SEASON 04",
        "size": "8vw",
        "opacity": 0.08,
        "color": "#1B0E0D"
      }
    }
  ]
}
