# Common Parameters

Parameters vary by playable. Below are parameters found in most builds.

> **Your dashboard shows the actual parameters available for your specific playable.**

---

## Sprite Parameters (Images)

| Parameter | Type | Properties You Can Change |
|-----------|------|---------------------------|
| Logo | `SpriteParameter` | `spriteFrame`, `spriteColor`, `enable`, `position`, `scale` |
| App Icon | `SpriteParameter` | `spriteFrame`, `spriteColor`, `scale` |
| Background | `SpriteParameter` | `spriteFrame`, `spriteColor`, `contentSize` |
| Character | `SpriteParameter` | `spriteFrame`, `spriteColor`, `position`, `scale` |
| Currency Icon | `SpriteParameter` | `spriteFrame`, `spriteColor`, `scale` |
| HP Bar Fill | `SpriteParameter` | `spriteColor` (change color only) |

### Sprite Property Reference

| Property | Type | Description | Example |
|----------|------|-------------|---------|
| `spriteFrame` | Image | The image file | Upload PNG/JPG |
| `spriteColor` | Color | Tint overlay | `#FFFFFF` |
| `enable` | Boolean | Visibility | `true` |
| `position` | Coordinates | Location | `{x: 0, y: 100}` |
| `scale` | Coordinates | Size multiplier | `{x: 1.0, y: 1.0}` |
| `contentSize` | Coordinates | Fixed dimensions | `{x: 512, y: 512}` |

---

## Label Parameters (Text)

| Parameter | Type | Properties You Can Change |
|-----------|------|---------------------------|
| CTA Text | `LabelParameter` | `string`, `labelColor`, `fontSize`, `isBold`, `outline`, `shadow` |
| Win Title | `LabelParameter` | `string`, `labelColor`, `fontSize`, `outline` |
| Lose Title | `LabelParameter` | `string`, `labelColor`, `fontSize`, `outline` |
| Loading Text | `LabelParameter` | `string`, `labelColor`, `fontSize` |
| Tutorial Text | `LabelParameter` | `string`, `labelColor`, `fontSize` |
| Score Label | `LabelParameter` | `string`, `labelColor`, `fontSize` |
| Timer Label | `LabelParameter` | `labelColor`, `fontSize` |

### Label Property Reference

| Property | Type | Description | Example |
|----------|------|-------------|---------|
| `string` | Text | The text content | `"Download Now"` |
| `labelColor` | Color | Text color | `#FFFFFF` |
| `fontSize` | Number | Text size in pixels | `48` |
| `lineHeight` | Number | Line spacing | `0` (auto) |
| `isBold` | Boolean | Bold weight | `true` |
| `isItalic` | Boolean | Italic style | `false` |
| `isUnderline` | Boolean | Underline | `false` |
| `outlineColor` | Color | Outline color | `#000000` |
| `outlineWidth` | Number | Outline thickness | `2` |
| `shadowColor` | Color | Shadow color | `#000000` |
| `shadowOffset` | Coordinates | Shadow position | `{x: 2, y: -2}` |

---

## Button Parameters

| Parameter | Type | Properties You Can Change |
|-----------|------|---------------------------|
| CTA Button | `ButtonParameter` | `spriteFrame`, `spriteColor`, `labelString`, `labelColor`, `labelFontSize`, `position`, `scale` |
| Play Button | `ButtonParameter` | `spriteFrame`, `spriteColor`, `labelString`, `labelColor` |
| Retry Button | `ButtonParameter` | `spriteFrame`, `labelString`, `labelColor` |
| Skip Button | `ButtonParameter` | `enable`, `labelString`, `labelColor` |

### Button Property Reference

| Property | Type | Description | Example |
|----------|------|-------------|---------|
| `spriteFrame` | Image | Button background | Upload PNG |
| `spriteColor` | Color | Background tint | `#FF5722` |
| `labelString` | Text | Button text | `"Play Now"` |
| `labelColor` | Color | Text color | `#FFFFFF` |
| `labelFontSize` | Number | Text size | `36` |
| `labelBold` | Boolean | Bold text | `true` |
| `labelOutlineColor` | Color | Text outline | `#000000` |
| `labelOutlineWidth` | Number | Outline thickness | `0` |

---

## Color Parameters

| Parameter | Type | Description |
|-----------|------|-------------|
| Primary Color | `ColorParameter` | Main brand color |
| Secondary Color | `ColorParameter` | Supporting color |
| Accent Color | `ColorParameter` | Highlight color |
| HP Bar Color | `ColorParameter` | Health fill color |
| HP Bar Background | `ColorParameter` | Empty bar color |
| Timer Color | `ColorParameter` | Timer text color |
| Timer Warning | `ColorParameter` | Low time color |
| Score Color | `ColorParameter` | Score text color |

### Color Format

| Format | Example | Usage |
|--------|---------|-------|
| Hex (solid) | `#FF5722` | Standard colors |
| Hex (alpha) | `#FF572280` | Semi-transparent (80 = 50% alpha) |

---

## Number Parameters (Gameplay)

| Parameter | Type | Description | Typical Range |
|-----------|------|-------------|---------------|
| Timer Duration | `NumberParameter` | Countdown seconds | 10-60 |
| Player HP | `NumberParameter` | Player health | 50-200 |
| Enemy HP | `NumberParameter` | Enemy health | 20-100 |
| Damage | `NumberParameter` | Attack damage | 10-50 |
| Speed | `NumberParameter` | Movement speed | 0.5-2.0 |
| Spawn Count | `NumberParameter` | Enemies per wave | 1-10 |
| Attempt Limit | `NumberParameter` | Max retries | 1-5 |
| Cooldown | `NumberParameter` | Wait time (seconds) | 0.5-5.0 |

---

## Boolean Parameters (Toggles)

| Parameter | Type | Default | Description |
|-----------|------|---------|-------------|
| Show Tutorial | `BooleanParameter` | `true` | Display tutorial overlay |
| Show Timer | `BooleanParameter` | `true` | Display countdown |
| Show Score | `BooleanParameter` | `true` | Display points |
| Show HP Bar | `BooleanParameter` | `true` | Display health bar |
| Enable Sound | `BooleanParameter` | `true` | Play audio |
| Enable Haptics | `BooleanParameter` | `false` | Vibration feedback |

---

## Range Parameters (Sliders)

| Parameter | Type | Min | Max | Description |
|-----------|------|-----|-----|-------------|
| Difficulty | `RangeParameter` | 1 | 10 | Overall difficulty |
| Volume | `RangeParameter` | 0 | 100 | Audio volume % |
| Speed Multiplier | `RangeParameter` | 0.5 | 2.0 | Game speed |

---

## Composite Parameters

### EndCardParameter

Controls entire end card screen.

| Component | Parameter Type | Key Properties |
|-----------|---------------|----------------|
| Background | `SpriteParameter` | `spriteFrame`, `spriteColor` |
| Title | `LabelParameter` | `string`, `labelColor`, `fontSize`, `outline` |
| Subtitle | `LabelParameter` | `string`, `labelColor`, `fontSize` |
| CTA Button | `ButtonParameter` | `spriteFrame`, `labelString`, `labelColor` |

### LoadingScreenParameter

Controls loading screen appearance.

| Component | Parameter Type | Key Properties |
|-----------|---------------|----------------|
| Background | `ColorParameter` | Color value |
| Icon | `SpriteParameter` | `spriteFrame`, `spriteColor` |
| Game Name | `LabelParameter` | `string`, `labelColor`, `fontSize` |

### TutorialHandParameter

Controls tutorial hand indicator.

| Component | Parameter Type | Key Properties |
|-----------|---------------|----------------|
| Hand | `SpriteParameter` | `spriteFrame`, `spriteColor` |
| Animation | `AnimationPreset` | Preset selection |

---

## Animation Presets

Available on compatible elements (RichText, Tutorial Hand).

| Category | Options |
|----------|---------|
| Entrance | `fadeIn`, `scaleUp`, `slideIn`, `bounceIn`, `pop` |
| Emphasis | `pulse`, `shake`, `bounce`, `wiggle`, `glow` |
| Exit | `fadeOut`, `scaleDown`, `slideOut`, `shrink` |
| Interactive | `tap`, `press`, `swipe`, `drag` |

---

## Your Playable May Have More

Each game has unique parameters based on its mechanics:

| Genre | Additional Parameters |
|-------|----------------------|
| Puzzle | Grid size, match count, piece colors, combo multiplier |
| Action | Weapon damage, fire rate, ammo count, reload time |
| Idle | Click multiplier, auto-income rate, upgrade costs |
| Simulation | Resource caps, unlock thresholds, time scales |

**Check your dashboard for the complete list.**

---

## Related

- [What's Included](whats-included.md) — Full parameter type reference
- [File Formats](file-formats.md) — Asset specifications
- [Limits & Constraints](limits.md) — Size and character limits
