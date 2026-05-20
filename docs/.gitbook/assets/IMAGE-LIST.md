# Image Assets Required

Place all images in this folder (`docs/.gitbook/assets/`).

---

## UI Layer — What's Included (10 images)

| File | Dimensions | Description |
|------|------------|-------------|
| `ui-layer-overview.png` | 1200x600 | Dashboard screenshot showing UI Layer parameters. Show: Sprite, Label, Button in sidebar. Preview panel updating in real-time. |
| `sprite-parameter-anatomy.png` | 800x400 | Sprite element with callouts: ① `spriteFrame` (image), ② `spriteColor` (tint), ③ `position`, ④ `scale`, ⑤ `enable`. Show icon/logo example. |
| `label-parameter-anatomy.png` | 800x400 | Text element with callouts: ① `string`, ② `labelColor`, ③ `fontSize`, ④ `outlineColor`/`outlineWidth`, ⑤ `shadowColor`/`shadowOffset`. |
| `label-outline-examples.png` | 900x200 | "PLAY NOW" text 3x: outlineWidth 0 (none), 2 (thin), 4 (thick). Black outline on white text. Labels below. |
| `button-parameter-anatomy.png` | 800x400 | CTA button with callouts: ① `spriteFrame` (bg), ② `spriteColor`, ③ `labelString`, ④ `labelColor`, ⑤ `labelFontSize`. Green button example. |
| `progressbar-parameter-anatomy.png` | 800x200 | HP bar with callouts: ① Background track, ② Fill bar (green), ③ `progress` value (0.7 = 70%). |
| `slider-parameter-anatomy.png` | 800x200 | Slider with callouts: ① Track, ② Handle/thumb, ③ `direction` indicator. Volume or difficulty slider. |
| `toggle-parameter-anatomy.png` | 600x200 | Two states side-by-side: ① OFF (unchecked), ② ON (checked with checkmark). "Enable Sound" example. |
| `color-parameter-format.png` | 600x200 | Hex format: `#FF5722` (solid orange swatch), `#FF572280` (50% transparent). Show alpha visualization. |
| `animation-presets-overview.png` | 1000x400 | 4-panel grid: ① Entrance (appearing), ② Exit (disappearing), ③ Emphasis (pulsing), ④ Interactive (hand tap). Simple icons. |

---

## Config Layer — What's Included (6 images)

| File | Dimensions | Description |
|------|------------|-------------|
| `config-layer-overview.png` | 1200x600 | Dashboard showing Config Layer. Show: HP, Timer, Difficulty parameters. Preview with HP bar and countdown updating. |
| `number-parameter-dashboard.png` | 600x150 | Dashboard number input. Label "Player HP", input field "100", +/- buttons. Clean UI. |
| `boolean-parameter-dashboard.png` | 600x150 | Dashboard toggle. Label "Show Tutorial", toggle ON (green). Maybe OFF state grayed below. |
| `range-parameter-dashboard.png` | 600x150 | Dashboard slider. Label "Difficulty", slider at 7, min "1" max "10" labels, value "7" displayed. |
| `select-parameter-dashboard.png` | 600x200 | Dashboard dropdown expanded. Label "Difficulty Preset", options: Easy, Medium (selected), Hard. |
| `redirect-parameter-dashboard.png` | 700x250 | Recurring offer parameter. Show: ① `active` toggle (ON/OFF), ② `count` number input (e.g., 3), ③ visual diagram showing "tap 1 → tap 2 → tap 3 = redirect to store". Illustrate the recurring CTA behavior. |

---

## Getting Started (6 images)

| File | Dimensions | Description |
|------|------------|-------------|
| `dashboard-overview.png` | 1200x800 | Full dashboard. Callouts: ① Parameter sidebar, ② Preview panel, ③ Edit controls. |
| `dashboard-workflow.png` | 1000x300 | 4-step flow: Select → Edit → Preview → Save. Arrows connecting. |
| `quick-start-login.png` | 800x500 | Login page at app.playablelabs.ai. Email, password fields, Sign In button. |
| `quick-start-select-parameter.png` | 1000x600 | Dashboard with "CTA Button" selected in sidebar. Cursor visible. |
| `quick-start-edit-save.png` | 1000x600 | Edit panel close-up. Text field edited, preview updating, Save highlighted. |
| `quick-start-before-after.png` | 1200x500 | Side-by-side: Before "Play Now" → After "Download Free". Clear labels. |

---

## Branding (4 images)

| File | Dimensions | Description |
|------|------------|-------------|
| `logo-upload-panel.png` | 800x500 | Logo upload UI. Current thumbnail, Upload/Replace buttons, file size info. |
| `logo-requirements.png` | 1000x400 | Left: ✓ Correct (transparent PNG). Right: ✗ Incorrect (white background). |
| `color-picker.png` | 600x400 | Color picker. Color wheel, selected swatch, hex input `#FF5722`. |
| `color-hex-input.png` | 500x200 | Hex input close-up. `#FF5722` solid, `#FF572280` with alpha. |

---

## Screens (3 images)

| File | Dimensions | Description |
|------|------------|-------------|
| `end-card-overview.png` | 1200x600 | Win screen (left) and Lose screen (right). Clear labels. |
| `loading-screen-elements.png` | 800x600 | Loading screen with callouts: ① Background, ② Logo, ③ Game Name, ④ Loading Icon. |
| `loading-indicator-types.png` | 800x200 | 4 types: Spinner, Progress bar, Animated icon, None. Labels below. |

---

## Total: 29 images

| Section | Count |
|---------|-------|
| UI Layer (What's Included) | 10 |
| Config Layer (What's Included) | 6 |
| Getting Started | 6 |
| Branding | 4 |
| Screens | 3 |
| **Total** | **29** |

---

## Image Specifications

| Property | Value |
|----------|-------|
| Format | PNG (transparency for callouts) |
| Max width | 1200px |
| Background | Light gray (#F5F5F5) or white |
| Annotations | Red (#E53935) circles with white numbers |
| Font | Sans-serif (Inter, Roboto, system) |

### Annotation Style

```
① ② ③ ④ ⑤  ← Circled numbers for callouts
✓ ✗         ← Correct/incorrect comparisons
→            ← Flow diagram arrows
```

### Dashboard Screenshots
- Use actual dashboard UI or high-fidelity mockup
- Light theme preferred
- Highlight active elements with subtle glow/border

### Anatomy Images
- Clean, isolated component on neutral background
- Component large and centered
- Callout lines should not overlap
