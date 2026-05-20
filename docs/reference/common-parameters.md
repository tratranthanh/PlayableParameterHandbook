# Common Parameters

Parameters vary by playable. Below are parameters found in most builds.

> **Your dashboard shows the actual parameters available for your specific playable.**

---

## Sprite Parameters

Images attached to `cc.Sprite` components.

| Parameter | Common Properties |
|-----------|-------------------|
| Logo | `spriteFrame`, `spriteColor`, `position`, `scale` |
| App Icon | `spriteFrame`, `scale` |
| Background | `spriteFrame`, `spriteColor`, `contentSize` |
| HP Bar Fill | `spriteColor` |
| Loading Icon | `spriteFrame`, `spriteColor` |

---

## Label Parameters

Text attached to `cc.Label` components.

| Parameter | Common Properties |
|-----------|-------------------|
| CTA Text | `string`, `labelColor`, `fontSize`, `outlineColor`, `outlineWidth` |
| Win Title | `string`, `labelColor`, `fontSize`, `outlineColor` |
| Lose Title | `string`, `labelColor`, `fontSize`, `outlineColor` |
| Loading Text | `string`, `labelColor`, `fontSize` |
| Tutorial Text | `string`, `labelColor`, `fontSize` |

---

## Button Parameters

Buttons with `cc.Button` components.

| Parameter | Common Properties |
|-----------|-------------------|
| CTA Button | `spriteFrame`, `spriteColor`, `labelString`, `labelColor`, `labelFontSize` |
| Play Button | `spriteFrame`, `labelString`, `labelColor` |
| Retry Button | `spriteFrame`, `labelString`, `labelColor` |
| Skip Button | `enable`, `labelString`, `labelColor` |

---

## Color Parameters

Standalone `ColorParameter` values.

| Parameter | Format | Example |
|-----------|--------|---------|
| Primary Color | Hex | `#FF5722` |
| Secondary Color | Hex | `#2196F3` |
| HP Bar Color | Hex | `#4CAF50` |
| Timer Color | Hex | `#FFFFFF` |
| Timer Warning | Hex | `#F44336` |

---

## Number Parameters

Gameplay values.

| Parameter | Typical Range |
|-----------|---------------|
| Timer Duration | 15-60 seconds |
| Player HP | 50-200 |
| Enemy HP | 20-100 |
| Damage | 10-50 |
| Speed Multiplier | 0.5-2.0 |
| Spawn Count | 1-10 |

---

## Boolean Parameters

Toggles.

| Parameter | Default |
|-----------|---------|
| Show Tutorial | `true` |
| Show Timer | `true` |
| Show Score | `true` |
| Show HP Bar | `true` |
| Enable Sound | `true` |

---

## Range Parameters

Sliders with min/max.

| Parameter | Min | Max |
|-----------|-----|-----|
| Difficulty | 1 | 10 |
| Volume | 0 | 100 |
| Speed | 0.5 | 2.0 |

---

## Composite Parameters

Pre-built screen bundles.

| Parameter | Components |
|-----------|------------|
| End Card (Win) | Background, Title, Subtitle, CTA Button |
| End Card (Lose) | Background, Title, Subtitle, CTA Button |
| Loading Screen | Background, Icon, Game Name, Logo |
| Tutorial Hand | Hand Sprite, Animation Preset |

---

## Related

- [UI Layer](ui-layer.md) — Full Sprite, Label, Button reference
- [Config Layer](config-layer.md) — Full Number, Boolean, Range reference
- [Composite Parameters](whats-included.md) — Full composite reference
- [File Formats](file-formats.md) — Asset specifications
