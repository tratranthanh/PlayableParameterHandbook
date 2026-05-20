# End Cards

End cards are the final screens users see — your best chance to convert.

<figure><img src="../.gitbook/assets/end-card-overview.png" alt="End Card Overview"><figcaption>Win screen (left) and Lose screen (right)</figcaption></figure>

---

## End Card Types

| Type | When It Appears | Typical Tone |
|------|-----------------|--------------|
| Win Screen | User succeeds | Celebratory, positive |
| Lose Screen | User fails | Encouraging, retry-focused |
| Time's Up | Timer runs out | Urgency, "almost had it" |

---

## EndCardParameter (Composite)

End cards use the `EndCardParameter` composite type, which bundles:

<figure><img src="../.gitbook/assets/end-card-elements.png" alt="End Card Elements"><figcaption>Customizable elements: Background, Title, Subtitle, CTA Button</figcaption></figure>

| Component | Parameter Type | What You Can Change |
|-----------|---------------|---------------------|
| Background | `SpriteParameter` | `spriteFrame`, `spriteColor` |
| Title | `LabelParameter` | `string`, `labelColor`, `fontSize`, `outline`, `shadow` |
| Subtitle | `LabelParameter` | `string`, `labelColor`, `fontSize` |
| CTA Button | `ButtonParameter` | `spriteFrame`, `spriteColor`, `labelString`, `labelColor`, `labelFontSize` |

---

## Background

### SpriteParameter Properties

| Property | Type | Description | Example |
|----------|------|-------------|---------|
| `spriteFrame` | `ImageParameter` | Background image | Upload PNG/JPG |
| `spriteColor` | `ColorParameter` | Color overlay/tint | `#000000` for darkening |

### Background Options

| Approach | When to Use |
|----------|-------------|
| Full image | Custom artwork, screenshots |
| Solid color | Clean, minimal look |
| Color + tint | Darken image for text readability |

---

## Title

### LabelParameter Properties

| Property | Type | Description | Example |
|----------|------|-------------|---------|
| `string` | `TextParameter` | Headline text | `"You Won!"` |
| `labelColor` | `ColorParameter` | Text color | `#FFFFFF` |
| `fontSize` | `NumberParameter` | Text size | `72` |
| `isBold` | `BooleanParameter` | Bold weight | `true` |
| `outlineColor` | `ColorParameter` | Outline color | `#000000` |
| `outlineWidth` | `NumberParameter` | Outline thickness | `4` |
| `shadowColor` | `ColorParameter` | Shadow color | `#000000` |
| `shadowOffset` | `CoordinatesParameter` | Shadow position | `{x: 3, y: -3}` |

### Title Examples

| Screen | Suggested Text | Tone |
|--------|---------------|------|
| Win | "You Won!", "Victory!", "Nice!" | Celebratory |
| Lose | "Try Again", "So Close!", "Almost!" | Encouraging |
| Time's Up | "Time's Up!", "Out of Time" | Urgent |

---

## Subtitle

### LabelParameter Properties

| Property | Type | Description | Example |
|----------|------|-------------|---------|
| `string` | `TextParameter` | Secondary text | `"Play the full game"` |
| `labelColor` | `ColorParameter` | Text color | `#CCCCCC` |
| `fontSize` | `NumberParameter` | Text size | `36` |

### Subtitle Examples

| Screen | Suggested Text |
|--------|---------------|
| Win | "Keep the fun going", "More levels await" |
| Lose | "Want to try again?", "The full game has more" |

---

## CTA Button

The Call-to-Action button converts viewers into downloads.

<figure><img src="../.gitbook/assets/end-card-cta.png" alt="CTA Button Customization"><figcaption>Customize CTA text, color, and style</figcaption></figure>

### ButtonParameter Properties

| Property | Type | Description | Example |
|----------|------|-------------|---------|
| `spriteFrame` | `ImageParameter` | Button background | Upload PNG |
| `spriteColor` | `ColorParameter` | Background color/tint | `#FF5722` |
| `labelString` | `TextParameter` | Button text | `"Download Now"` |
| `labelColor` | `ColorParameter` | Text color | `#FFFFFF` |
| `labelFontSize` | `NumberParameter` | Text size | `42` |
| `labelBold` | `BooleanParameter` | Bold text | `true` |
| `labelOutlineColor` | `ColorParameter` | Text outline | `#000000` |
| `labelOutlineWidth` | `NumberParameter` | Outline thickness | `2` |

### CTA Text Examples

| Good (Action-oriented) | Weak (Generic) |
|------------------------|----------------|
| "Download Now" | "Click Here" |
| "Play Free" | "Continue" |
| "Get the App" | "OK" |
| "Try It!" | "Submit" |

### CTA Color Tips

| Goal | Approach |
|------|----------|
| Maximum visibility | Bright accent color, contrasts with background |
| Brand alignment | Use brand primary or accent color |
| Text readability | High contrast between `labelColor` and `spriteColor` |

---

## Win Screen Configuration

| Element | Recommendation |
|---------|----------------|
| Title | Celebrate: "You Won!", "Victory!" |
| Subtitle | "Keep the fun going", "More levels await" |
| CTA | "Download Now", "Play More" |
| Background | Bright, positive colors or celebration imagery |

---

## Lose Screen Configuration

| Element | Recommendation |
|---------|----------------|
| Title | Encouraging: "Try Again", "So Close!" |
| Subtitle | "Want to try again?", "The full game has more" |
| CTA | "Get Full Game", "Try Again" |
| Background | Softer colors, retry-focused imagery |

---

## Testing End Cards

1. **Play to win** — Verify win screen displays correctly
2. **Play to lose** — Verify lose screen displays correctly  
3. **Tap CTA** — Confirm redirect works
4. **Check mobile** — Ensure buttons are tappable (min 44x44px)
5. **Check text** — Verify all text fits and is readable

---

## Related

- [Buttons](../branding/buttons.md) — Button styling details
- [Loading Screen](loading.md) — First screen users see
- [What's Included](../reference/whats-included.md) — Full parameter reference
