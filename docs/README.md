# Parameter Dashboard Handbook

Customize your playable ad at [app.playablelabs.ai](https://app.playablelabs.ai/).

---

## What Do You Need?

| 🖼️ **Images & Colors** | 🎮 **Gameplay** | 📱 **Screens** |
|------------------------|-----------------|----------------|
| [Add your logo](branding/logos-icons.md) | [Adjust difficulty](gameplay/difficulty.md) | [Edit end card](screens/end-cards.md) |
| [Set brand colors](branding/colors.md) | [Change timers](gameplay/timing.md) | [Customize loading](screens/loading.md) |
| [Style buttons](branding/buttons.md) | [Modify UI elements](gameplay/ui-elements.md) | [Update tutorial](screens/tutorial.md) |

---

## What's Included

**Two-layer system — UI is automatic, Config requires approval.**

### 🎨 UI Layer — Visual Components (Auto)

**Always included. No approval needed.** Changes apply instantly.

| ComponentParameter | Cocos Component | What You Change |
|--------------------|-----------------|-----------------|
| **SpriteComponentParameter** | `cc.Sprite` | `spriteFrame`, `spriteColor`, `position`, `scale`, `contentSize`, `enable` |
| **LabelComponentParameter** | `cc.Label` | `string`, `labelColor`, `fontSize`, `lineHeight`, `isBold`, `isItalic`, `outlineColor`, `outlineWidth`, `shadowColor`, `shadowOffset`, `enable` |
| **ButtonComponentParameter** | `cc.Button` | All Sprite fields + `labelString`, `labelColor`, `labelFontSize`, `labelBold`, `labelOutlineColor`, `labelOutlineWidth` |
| **TransformComponentParameter** | `cc.Node` | `position`, `rotation`, `scale` |
| **UIOpacityComponentParameter** | `cc.UIOpacity` | `opacity` |
| **ProgressBarComponentParameter** | `cc.ProgressBar` | `progress`, `totalLength`, `reverse` |
| **SliderComponentParameter** | `cc.Slider` | `progress`, `direction` |
| **ToggleComponentParameter** | `cc.Toggle` | `isChecked`, `interactable` |

📋 **[Full UI Layer reference →](getting-started/ui-layer.md)**

### ⚙️ Config Layer — Gameplay Values (Approval Required)

**Included if parameter exists in your dashboard.** Affects gameplay balance.

| Category | Parameters |
|----------|------------|
| **Health** | `playerHP`, `enemyHP`, `bossHP` |
| **Damage** | `damage`, `playerDamage`, `enemyDamage` |
| **Timing** | `timerDuration`, `cooldown`, `delay`, `spawnInterval` |
| **Speed** | `speedMultiplier`, `playerSpeed`, `enemySpeed` |
| **Counts** | `spawnCount`, `maxBullets`, `livesCount` |
| **Toggles** | `showTutorial`, `enableSound`, `showHPBar` |

📋 **[Full Config Layer reference →](getting-started/config-layer.md)**

---

## Quick Links

| 📋 [Common Parameters](reference/common-parameters.md) | ❓ [FAQ](help/faq.md) | 🚀 [Quick Start](getting-started/quick-start.md) |
|--------------------------------------------------------|----------------------|--------------------------------------------------|

---

## Need Something More?

Parameters not in your dashboard require development. See [Custom Development](help/custom-development.md).

---

## Get Started

1. **[Quick Start](getting-started/quick-start.md)** — Make your first change
2. **[What's Included — UI Layer](getting-started/ui-layer.md)** — Visual parameters (no cost)
3. **[What's Included — Config Layer](getting-started/config-layer.md)** — Gameplay values
