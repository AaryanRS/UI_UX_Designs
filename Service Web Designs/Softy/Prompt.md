{
  "project_name": "Softy — Digital Wellness Landing Page",
  "theme": "Digital Living Room / Digital Minimalism & Gen-Z Lifestyle",
  "device_target": "mobile",
  "design_system": {
    "palette": {
      "background": "#FDFCF8",
      "primary_accent": "#FFB7B2",
      "sage": "#E8EFE8",
      "lavender": "#EFEDF4",
      "text_dark": "#292524",
      "text_muted": "#78716C",
      "borders": "#E7E5E4"
    },
    "typography": {
      "primary_font": "Outfit, sans-serif",
      "accent_font": "Reenie Beanie, cursive",
      "heading_scale": "48px-72px",
      "tracking": "-0.025em",
      "case": "sentence-case"
    },
    "effects": {
      "grain_overlay": {
        "type": "SVG feTurbulence",
        "base_frequency": 0.65,
        "opacity": 0.35,
        "mix_blend_mode": "overlay",
        "position": "fixed",
        "z_index": 50,
        "pointer_events": "none"
      },
      "border_radius": "2rem to 4rem (rounded-3xl, rounded-[2.5rem], rounded-full)",
      "ambient_shadow": "0 4px 20px -2px rgba(0,0,0,0.05)",
      "background_blobs": {
        "colors": ["#FFE4E1", "#E6E6FA"],
        "blur": "blur-3xl",
        "opacity": 0.60,
        "animation": "float 6s ease-in-out infinite"
      }
    }
  },
  "sections": [
    {
      "id": "navigation",
      "type": "floating_pill",
      "backdrop_blur": "20px",
      "background": "rgba(255, 255, 255, 0.70)",
      "border": "1px solid rgba(231, 229, 228, 0.6)",
      "elements": [
        "Coral #FFB7B2 circular brand logo with white dot",
        "Brand text 'softy' in Outfit medium",
        "CTA pill button in #292524 'Open App'"
      ]
    },
    {
      "id": "hero",
      "layout": "center_aligned",
      "badge": "• a digital living room",
      "headline": "Feel screen-time turn gentle again.",
      "headline_cursive_word": "gentle",
      "subheadline": "An intentionally slow, tactile sanctuary designed to quiet digital overstimulation and restore everyday presence.",
      "cta_buttons": [
        { "text": "Begin mindful breathing", "bg": "#FFB7B2", "color": "#292524", "style": "pill with soft shadow" },
        { "text": "Explore rituals", "bg": "#FFFFFF", "border": "1px solid #E7E5E4", "style": "pill" }
      ]
    },
    {
      "id": "horizontal_scenario_scroll",
      "scroll_direction": "horizontal",
      "cards": [
        { "timestamp": "07:15 AM", "title": "Morning fog", "description": "One mindful breath before incoming feeds arrive.", "accent_hover": "#FFB7B2" },
        { "timestamp": "02:40 PM", "title": "Screen fatigue", "description": "Soft micro-pauses that unspool afternoon tension.", "accent_hover": "#9bbba0" },
        { "timestamp": "09:30 PM", "title": "Bedtime scroll", "description": "Trade late-night loops for calming ambient rain.", "accent_hover": "#b3a8d1" }
      ]
    },
    {
      "id": "app_preview",
      "layout": "cascading_mockups",
      "center_phone": {
        "dimensions": "300x620px",
        "screen_bg": "#FDFCF8",
        "interactive_element": "Pulsing coral #FFB7B2 'Breathe' ripple button"
      }
    },
    {
      "id": "diary_testimonials",
      "style": "physical_diary_cards",
      "entries": [
        {
          "rotation": "+1deg",
          "quote": "I replaced my impulsive 11 PM Instagram habit with Softy's 4-minute soft wind meditation. My sleep score jumped, but more importantly, my mind finally stopped buzzing.",
          "author": "Maya L., Product Designer",
          "signature_style": "32px line + Reenie Beanie font"
        },
        {
          "rotation": "-1deg",
          "quote": "The tactile haptics and pastel breathing circle make taking a break feel like wrapping myself in a warm linen blanket. It's the only wellness app that doesn't feel like homework.",
          "author": "Julian K., Architecture Student",
          "signature_style": "32px line + Reenie Beanie font"
        }
      ]
    },
    {
      "id": "faq_accordion",
      "items": [
        { "q": "How is Softy different from other apps?", "icon": "rotating plus (+45deg)" },
        { "q": "Is it really 100% ad-free?", "icon": "rotating plus (+45deg)" },
        { "q": "Can I use it offline while traveling?", "icon": "rotating plus (+45deg)" }
      ]
    },
    {
      "id": "waitlist_conversion",
      "bg": "#292524",
      "badge_icon": "rounded-square with coral glowing dot",
      "headline": "Step into the living room.",
      "subheadline": "Join 14,000+ early wanderers embracing a more delicate digital rhythm.",
      "form": {
        "input_placeholder": "your.cozy.email@gmail.com",
        "submit_button": "Claim my early invitation",
        "button_bg": "#FFB7B2"
      }
    }
  ]
}