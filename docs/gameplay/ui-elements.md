# Game UI Elements

Customize UI styling: health bars, timers, scores, currency displays.

> **These are visual (UI Layer) parameters.** Gameplay values (Config Layer) are in [Difficulty & Balance](difficulty.md).

---

## HP Bars

Health bars show player or enemy health status.

### SpriteParameter Properties

| Property | Config Key | Type | Description |
|----------|------------|------|-------------|
| `spriteColor` | Fill color | `ColorParameter` | The health fill color |
| `enable` | Visibility | `BooleanParameter` | Show or hide HP bar |
| `position` | Location | `CoordinatesParameter` | Position on screen |
| `scale` | Size | `CoordinatesParameter` | Size multiplier |

### Common HP Bar Color Properties

| Element | Property | Example |
|---------|----------|---------|
| Health fill | `spriteColor` | `#00FF00` (green) |
| Damage indicator | `indicatorColor` | `#FFFF00` (yellow flash) |
| Empty background | `backgroundColor` | `#333333` (dark gray) |
| Border | `borderColor` | `#000000` (black) |

### HP Bar Anatomy

```
┌────────────────────────────────┐
│ ████████████░░░░░░░░░░░░░░░░░░ │  ← Border
│ ↑ Fill      ↑ Background       │
└────────────────────────────────┘
```

### Color Scheme Examples

| Style | Fill | Background | Border |
|-------|------|------------|--------|
| Classic | `#00C853` | `#424242` | `#000000` |
| Modern | `#00BCD4` | `#263238` | `#FFFFFF` |
| Aggressive | `#F44336` | `#B71C1C` | `#000000` |
| Brand | Your primary | Neutral | Optional |

---

## Timers

Timer displays show countdowns or elapsed time.

### LabelParameter Properties

| Property | Config Key | Type | Description |
|----------|------------|------|-------------|
| `labelColor` | Text color | `ColorParameter` | Timer number color |
| `fontSize` | Text size | `NumberParameter` | Font size in pixels |
| `outlineColor` | Outline | `ColorParameter` | Text outline color |
| `outlineWidth` | Outline size | `NumberParameter` | Outline thickness |
| `enable` | Visibility | `BooleanParameter` | Show or hide timer |

### Timer State Colors

| State | When | Suggested Color |
|-------|------|-----------------|
| Normal | > 10 seconds | `#FFFFFF` (white) |
| Warning | 5-10 seconds | `#FFC107` (yellow) |
| Critical | < 5 seconds | `#F44336` (red) |

> **Note:** Timer state colors may be separate `ColorParameter` entries in your dashboard.

---

## Score Displays

Score counters show points earned during gameplay.

### LabelParameter Properties

| Property | Config Key | Type | Description |
|----------|------------|------|-------------|
| `string` | Format | `TextParameter` | Score prefix (e.g., "Score: ") |
| `labelColor` | Color | `ColorParameter` | Score number color |
| `fontSize` | Size | `NumberParameter` | Font size |
| `enable` | Visibility | `BooleanParameter` | Show or hide score |

### Score Icon (SpriteParameter)

| Property | Config Key | Type | Description |
|----------|------------|------|-------------|
| `spriteFrame` | Icon | `ImageParameter` | Coin or star icon |
| `spriteColor` | Tint | `ColorParameter` | Icon color tint |
| `scale` | Size | `CoordinatesParameter` | Icon size |

---

## Currency Displays

Currency shows in-game money or collectibles.

### Combined Parameters

| Element | Parameter Type | Properties |
|---------|---------------|------------|
| Icon | `SpriteParameter` | `spriteFrame`, `spriteColor`, `scale` |
| Amount | `LabelParameter` | `labelColor`, `fontSize` |
| Background | `SpriteParameter` | `spriteFrame`, `spriteColor` (optional) |

---

## What You CAN Change (UI Layer)

| Element | Changeable Properties |
|---------|----------------------|
| HP Bar | Colors, visibility, position, scale |
| Timer | Text color, font size, outline, visibility |
| Score | Text color, font size, icon, visibility |
| Currency | Icon image, text color, visibility |

---

## What You CANNOT Change Without Development

| Element | Requires Development |
|---------|---------------------|
| HP Bar | Actual HP values, damage calculation |
| Timer | Duration, countdown logic, pause behavior |
| Score | Point values, scoring formula |
| Currency | Starting amount, earn rates |

For gameplay value changes, see:
- [Difficulty & Balance](difficulty.md) — HP, damage, timer duration
- [Gameplay Values](values.md) — Scores, multipliers
- [Custom Development](../help/custom-development.md) — New mechanics

---

## Best Practices

### Color Choices

- **Match your brand** — Use brand colors where appropriate
- **Maintain clarity** — UI must be readable at a glance
- **Use contrast** — Numbers visible against backgrounds
- **Be consistent** — Same style across all UI elements

### Visual Hierarchy

| Priority | Elements | Treatment |
|----------|----------|-----------|
| High | HP, Timer | Most visible, larger |
| Medium | Score, Currency | Visible but secondary |
| Low | Labels, Icons | Subtle, supporting |

---

## Related

- [Difficulty & Balance](difficulty.md) — Change gameplay values
- [Colors](../branding/colors.md) — Brand color application
- [What's Included](../reference/whats-included.md) — Full parameter reference
