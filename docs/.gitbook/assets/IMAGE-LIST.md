# Image Assets Required

Place all images in this folder (`docs/.gitbook/assets/`).

---

## Getting Started (6 images)

| File | Description |
|------|-------------|
| `dashboard-overview.png` | Full dashboard interface. Show: ① Parameter sidebar (left), ② Preview panel (center), ③ Edit controls (right). Use numbered callouts. |
| `dashboard-workflow.png` | Horizontal 4-step flow diagram: Select → Edit → Preview → Save. Arrows connecting each. |
| `quick-start-login.png` | Login page screenshot. Show email field, password field, "Sign In" button. URL bar showing app.playablelabs.ai. |
| `quick-start-select-parameter.png` | Dashboard with parameter highlighted in sidebar. Show cursor selecting "CTA Button" or similar. |
| `quick-start-edit-save.png` | Edit panel close-up. Show text field being edited, live preview updating, Save button highlighted. |
| `quick-start-before-after.png` | Side-by-side comparison. Left: "Before" with original button. Right: "After" with changed button. Clear labels. |

---

## Branding (4 images)

| File | Description |
|------|-------------|
| `logo-upload-panel.png` | Logo upload interface. Show current logo thumbnail, Upload/Replace buttons, file size/format info. |
| `logo-requirements.png` | Good vs bad comparison. Left: ✓ Correct (transparent PNG). Right: ✗ Incorrect (white background box). |
| `color-picker.png` | Color picker interface. Show color wheel/gradient, selected swatch, hex input field showing `#FF5722`. |
| `color-hex-input.png` | Close-up of hex input. Show format examples: `#FF5722` (solid), `#FF572280` (with alpha). |

---

## UI Layer Reference (6 images)

| File | Description |
|------|-------------|
| `ui-layer-overview.png` | Diagram showing UI Layer components: Sprite, Label, Button nodes on a game screen. Callouts pointing to each. |
| `sprite-parameter-anatomy.png` | Single sprite with callouts: ① `spriteFrame` (the image), ② `spriteColor` (tint), ③ `position`, ④ `scale`. |
| `label-parameter-anatomy.png` | Single label with callouts: ① `string` (text), ② `labelColor`, ③ `fontSize`, ④ `outline`, ⑤ `shadow`. |
| `label-outline-examples.png` | Same text shown 3 times with different outline widths: 0 (none), 2 (thin), 4 (thick). Labels below each. |
| `button-parameter-anatomy.png` | Button with callouts: ① `spriteFrame` (background), ② `spriteColor`, ③ `labelString`, ④ `labelColor`, ⑤ `labelFontSize`. |
| `color-parameter-format.png` | Color format diagram. Show: `#RRGGBB` breakdown with example `#FF5722`, plus `#RRGGBBAA` with alpha example. |

---

## Config Layer Reference (1 image)

| File | Description |
|------|-------------|
| `config-layer-overview.png` | Diagram showing Config Layer types: Number (slider), Boolean (toggle), Range (slider with min/max), Select (dropdown). |

---

## Composite Parameters Reference (4 images)

| File | Description |
|------|-------------|
| `composite-overview.png` | Diagram showing how composites bundle components. Show: Sprite + Label + Button = EndCardParameter. |
| `endcard-parameter-anatomy.png` | End card screen with callouts: ① Background (Sprite), ② Title (Label), ③ Subtitle (Label), ④ CTA Button (Button). |
| `loadingscreen-parameter-anatomy.png` | Loading screen with callouts: ① Background (Color), ② Logo (Sprite), ③ Game Name (Label), ④ Loading Icon (Sprite). |
| `tutorialhand-parameter-anatomy.png` | Tutorial hand with callouts: ① Hand (Sprite), ② Animation preset indicator (tap/swipe/drag). |

---

## Screens (5 images)

| File | Description |
|------|-------------|
| `end-card-overview.png` | Win screen (left) and Lose screen (right) side-by-side. Clear "Win" / "Lose" labels. |
| `end-card-elements.png` | Single end card with numbered callouts: ① Background, ② Title, ③ Subtitle, ④ CTA Button. |
| `end-card-cta.png` | CTA button close-up with property controls visible: text input, color pickers for background and text. |
| `loading-screen-elements.png` | Loading screen with callouts: ① Background, ② Logo, ③ Game Name, ④ Loading Icon. |
| `loading-indicator-types.png` | 4 loading indicators side-by-side: Spinner, Progress bar, Animated icon, None. Labels below each. |

---

## Total: 26 images

| Section | Count |
|---------|-------|
| Getting Started | 6 |
| Branding | 4 |
| UI Layer Reference | 6 |
| Config Layer Reference | 1 |
| Composite Parameters | 4 |
| Screens | 5 |
| **Total** | **26** |

---

## Image Specifications

| Property | Value |
|----------|-------|
| Format | PNG |
| Max width | 1200px |
| Background | Light gray (#F5F5F5) or white |
| Annotations | Red (#E53935) circles/arrows with white numbers |
| Labels | Sans-serif font (Inter, Roboto, system) |

### Annotation Style

```
① ② ③ ④ ⑤  ← Use circled numbers for callouts
✓ ✗         ← Use for correct/incorrect comparisons
→            ← Use arrows for flow diagrams
```
