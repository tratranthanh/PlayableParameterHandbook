# Reference

Complete parameter reference organized by layer.

---

## Parameter Layers

| Layer | What It Controls | Cost |
|-------|------------------|------|
| **[UI Layer](ui-layer.md)** | Visual appearance (images, text, colors, buttons) | ✅ Always included |
| **[Config Layer](config-layer.md)** | Gameplay values (HP, timers, speed, toggles) | ✅ Included if in dashboard |
| **[Composites](whats-included.md)** | Pre-built screen bundles | ✅ Included if in dashboard |

---

## Quick Reference

### UI Layer Components

| Component | Node Type | Key Properties |
|-----------|-----------|----------------|
| `SpriteParameter` | `cc.Sprite` | `spriteFrame`, `spriteColor`, `position`, `scale` |
| `LabelParameter` | `cc.Label` | `string`, `labelColor`, `fontSize`, `outline`, `shadow` |
| `ButtonParameter` | `cc.Button` | Sprite + `labelString`, `labelColor`, `labelFontSize` |

### Config Layer Types

| Type | Input | Example |
|------|-------|---------|
| `NumberParameter` | Number field | `100` |
| `BooleanParameter` | Toggle | `true` |
| `RangeParameter` | Slider | `0.5` (min-max) |
| `SelectParameter` | Dropdown | `"medium"` |

### Composite Parameters

| Composite | Components |
|-----------|------------|
| `EndCardParameter` | Background + Title + Subtitle + CTA |
| `LoadingScreenParameter` | Background + Icon + Game Name |
| `TutorialHandParameter` | Hand + Animation |

---

## Other References

- **[Common Parameters](common-parameters.md)** — Parameters found in most builds
- **[File Formats](file-formats.md)** — Image and audio specifications
- **[Limits & Constraints](limits.md)** — Size and character limits
