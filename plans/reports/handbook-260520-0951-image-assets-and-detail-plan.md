# Handbook Image Assets — Final List

**Date:** 2025-05-20  
**Status:** Documentation updated, images needed

---

## Summary

- **Total images needed:** 32
- **Documentation updated:** 7 files aligned with `t1k-cocos-cocos-base-playable-parameter` skill
- **New page created:** `reference/whats-included.md` — comprehensive parameter reference

---

## Image Asset List

### Getting Started (6 images)

| File Name | Dimensions | Description |
|-----------|------------|-------------|
| `dashboard-overview.png` | 1200x800 | Full dashboard interface. Show: ① Parameter sidebar, ② Preview panel, ③ Edit controls. Annotate with numbered callouts. |
| `dashboard-workflow.png` | 1000x300 | Horizontal 4-step flow: Select → Edit → Preview → Save. Arrows connecting each step. |
| `quick-start-login.png` | 800x500 | Login page at app.playablelabs.ai. Show email field, password field, Sign In button. |
| `quick-start-select-parameter.png` | 1000x600 | Dashboard with a parameter selected (highlight "CTA Button" in sidebar). Cursor/selection indicator visible. |
| `quick-start-edit-save.png` | 1000x600 | Edit panel close-up. Show text field being edited, preview updating in background, Save button highlighted. |
| `quick-start-before-after.png` | 1200x500 | Side-by-side comparison. Left: Original "Play Now" button. Right: Changed "Download Free" button. Clear Before/After labels. |

---

### Branding (10 images)

| File Name | Dimensions | Description |
|-----------|------------|-------------|
| `logo-upload-panel.png` | 800x500 | Logo upload interface. Show current logo thumbnail, Upload/Replace buttons, file size indicator. |
| `logo-requirements.png` | 1000x400 | Good vs bad comparison. Left: Correct (transparent PNG, ✓). Right: Incorrect (white background, ✗). |
| `logo-sizing-guide.png` | 800x400 | 512x512 square with logo centered, safe zone margins marked with dashed lines. |
| `color-picker.png` | 600x400 | Color picker interface. Show color wheel/gradient, selected swatch, hex input field showing `#FF5722`. |
| `color-hex-input.png` | 500x200 | Close-up of hex input field. Show format: `#FF5722` for solid, `#FF572280` for alpha. |
| `color-transparency.png` | 800x300 | Same color at 100%, 80%, 50% opacity. Show hex codes beneath each: `#FF5722`, `#FF5722CC`, `#FF572280`. |
| `button-anatomy.png` | 800x400 | Button with numbered callouts: ① `spriteFrame` (background), ② `spriteColor`, ③ `labelString`, ④ `labelColor`, ⑤ `labelFontSize`. |
| `button-states.png` | 900x300 | Three buttons side-by-side: Normal, Pressed (darker), Disabled (grayed). Labels below each. |
| `button-cta-examples.png` | 1000x400 | Two columns: Good CTAs (✓ "Download Now", "Play Free", "Get the App") vs Bad (✗ "Click Here", "OK", "Continue"). |
| `text-styling-options.png` | 800x400 | Same text with different styles: Regular, Bold, With Outline, With Shadow. Show property names. |

---

### Gameplay (8 images)

| File Name | Dimensions | Description |
|-----------|------------|-------------|
| `hp-bar-anatomy.png` | 800x200 | HP bar with callouts: ① Fill (`spriteColor`), ② Background, ③ Border, ④ Indicator (damage flash). |
| `hp-bar-color-schemes.png` | 1000x300 | 4 HP bars: Classic (green), Modern (teal), Aggressive (red), Brand (custom). Hex codes below each. |
| `timer-states.png` | 800x200 | Three timers: Normal (white, "0:45"), Warning (yellow, "0:10"), Critical (red, "0:03"). |
| `score-display.png` | 600x300 | Score with callouts: ① Icon (`spriteFrame`), ② Number (`labelColor`), ③ Background. |
| `ui-parameter-dashboard.png` | 1000x600 | Dashboard screenshot showing Game UI section expanded: HP Bar, Timer, Score parameters visible. |
| `difficulty-included-vs-custom.png` | 1000x400 | Two columns: "Included" (slider adjustments, dashboard icon) vs "Custom" (code icon, "Quote Required" badge). |
| `config-vs-ui-layer.png` | 1000x400 | Diagram showing: UI Layer (visual) → How it looks. Config Layer (gameplay) → How it plays. |
| `timing-parameters.png` | 800x400 | Timer duration slider, delay input, speed multiplier controls. Show NumberParameter fields. |

---

### Screens (8 images)

| File Name | Dimensions | Description |
|-----------|------------|-------------|
| `end-card-overview.png` | 1200x600 | Win screen (left, celebratory) and Lose screen (right, encouraging). Clear labels. |
| `end-card-elements.png` | 800x600 | Single end card with callouts: ① Background (`SpriteParameter`), ② Title (`LabelParameter`), ③ Subtitle, ④ CTA Button (`ButtonParameter`). |
| `end-card-cta.png` | 600x400 | CTA button close-up with property controls visible: `labelString`, `spriteColor`, `labelColor` inputs. |
| `loading-screen-elements.png` | 800x600 | Loading screen with callouts: ① Background (`ColorParameter`), ② Logo (`SpriteParameter`), ③ Game Name (`LabelParameter`), ④ Loading Icon. |
| `loading-indicator-types.png` | 800x200 | 4 types side-by-side: Spinner, Progress bar, Animated icon, None. Labels below each. |
| `tutorial-screen.png` | 800x600 | Tutorial with callouts: ① Instruction text, ② Hand/tap indicator (`TutorialHandParameter`), ③ Skip button. |
| `tutorial-hand-parameter.png` | 600x400 | TutorialHandParameter composite: Hand sprite + animation preset dropdown. |
| `rich-text-parameter.png` | 800x400 | RichTextParameter composite: Label + entrance animation + exit animation + auto-hide toggle. |

---

## Image Style Guide

### Annotations

Use numbered callouts (①②③④⑤) with legend below:

```
┌─────────────────────────────────────┐
│  ①                                  │
│  ┌──────┐  ┌─────────────────────┐  │
│  │      │  │                     │  │
│  │  ②   │  │         ③          │  │
│  │      │  │                     │  │
│  └──────┘  └─────────────────────┘  │
└─────────────────────────────────────┘

① Parameter sidebar
② Preview panel  
③ Edit controls
```

### Comparison Images

| Type | Format |
|------|--------|
| Good/Bad | ✓ Correct (left) / ✗ Incorrect (right) |
| Before/After | "Before" label (left) / "After" label (right) |
| States | Side-by-side with state names below |

### Technical Specs

| Property | Value |
|----------|-------|
| Max width | 1200px |
| Format | PNG for screenshots, JPG acceptable for photos |
| Background | Light gray (#F5F5F5) or white |
| Annotation color | Red (#E53935) for callout circles/arrows |
| Font | Sans-serif (Inter, Roboto, or system) |

---

## Files Updated

| File | Changes |
|------|---------|
| `docs/SUMMARY.md` | Added "What's Included" page to navigation |
| `docs/README.md` | Updated "What's Included" section with parameter types |
| `docs/reference/whats-included.md` | **NEW** — Comprehensive parameter reference |
| `docs/reference/common-parameters.md` | Aligned with actual parameter types |
| `docs/gameplay/ui-elements.md` | Added parameter type details |
| `docs/gameplay/difficulty.md` | Split UI/Config layers clearly |
| `docs/screens/end-cards.md` | Added EndCardParameter composite details |
| `docs/screens/loading.md` | Added LoadingScreenParameter composite details |

---

## Parameter System Alignment

Documentation now reflects the actual `t1k-cocos-cocos-base-playable-parameter` skill:

### Base Types Documented
- `NumberParameter`, `BooleanParameter`, `ColorParameter`, `TextParameter`
- `ImageParameter`, `AudioParameter`, `RangeParameter`, `CoordinatesParameter`
- `SelectParameter`

### Component Types Documented
- `SpriteParameter` — Images with position, scale, color
- `LabelParameter` — Text with color, size, outline, shadow
- `ButtonParameter` — Sprite + Label combined
- `UINodeParameter` — Base for UI elements

### Composite Types Documented
- `EndCardParameter` — Background + Title + Subtitle + CTA
- `LoadingScreenParameter` — Background + Icon + Game Name
- `TutorialHandParameter` — Hand + Animation preset
- `RichTextParameter` — Label + entrance/exit animations

---

## Next Steps

1. **Provide 32 images** per specifications above
2. **Review updated docs** — Verify accuracy against your dashboard
3. **Add game-specific parameters** — Any parameters unique to specific games?
