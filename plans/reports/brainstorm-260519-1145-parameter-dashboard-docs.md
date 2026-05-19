# Brainstorm Report: Parameter Dashboard User Documentation

**Date:** 2026-05-19  
**Status:** Approved  
**Audience:** Ad Network Clients (non-technical)

## Objective

Create GitBook documentation for Parameter Dashboard users explaining:
1. What parameters they can customize
2. Pricing model (free vs. paid)

## Key Decisions

### Audience
- Ad Network Clients who purchase playable ads
- Non-technical users (no dev background)
- Primary goal: understand what they can change via dashboard

### Pricing Model
| Category | Pricing |
|----------|---------|
| Auto-scanned UI components | FREE |
| Auto-detected config values | FREE |
| Custom implementation (new features) | Case-by-case quote |

**Key insight:** If the system auto-detects it, it's free. Only manual development work is charged.

### Documentation Structure (Use-Case Based)

```
📚 Parameter Dashboard Handbook
├── 🚀 Getting Started
│   ├── What is the Parameter Dashboard?
│   ├── Accessing Your Dashboard
│   └── Quick Start: Your First Change
├── ✏️ Text & Headlines
├── 🖼️ Images & Visuals
├── 🎨 Colors & Branding
├── 🔘 Interactive Elements
├── 📊 Game UI Elements
├── ⚙️ Game Settings
├── 🎬 Screens & Views
├── 💼 Custom Development
└── ❓ FAQ & Support
```

### Content Principles

| Principle | Implementation |
|-----------|----------------|
| No jargon | "Change text" not "Modify LabelParameter" |
| Action-oriented | "How to replace your logo" not "Image parameters" |
| Visual learning | Dashboard screenshots for each section |
| Clear free/paid | "Everything you see = free" |
| Simple request flow | Contact for custom work |

## Technical Alignment

Aligned with `/t1k-cocos-cocos-base-playable-parameter` skill:

### Auto-Scanned (FREE)
- **UI Components:** Label, Sprite, Button, ProgressBar, Slider, Toggle, etc.
- **UI Composites:** Any detected node pattern (CurrencyUI, HPBar, etc.)
- **Config Values:** All values from `*Config.ts` files

### Custom Development (PAID)
- New game mechanics
- Custom shader effects
- Server-side integration
- Complex progression logic

## Next Steps

1. Create GitBook content files following structure above
2. Include dashboard screenshots (placeholder locations)
3. Write user-friendly copy for each section
4. Set up pricing/quote request flow

## References

- `/t1k-cocos-cocos-base-playable-parameter` — Orchestrator skill
- `/t1k-cocos-cocos-base-playable-parameter-scan` — Scan modes
- `/t1k-cocos-cocos-base-playable-parameter-composite` — Preset catalog
