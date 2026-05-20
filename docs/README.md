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

## Quick Links

| 📋 [Common Parameters](reference/common-parameters.md) | ❓ [FAQ](help/faq.md) | 🚀 [Quick Start](getting-started/quick-start.md) |
|--------------------------------------------------|----------------------|--------------------------------------------------|

---

## What's Included

**If it's in your dashboard, you can change it — no extra cost.**

Parameters are organized into two layers:

| Layer | What You Change | Examples |
|-------|-----------------|----------|
| **UI Layer** | Visual appearance | Images, text, colors, buttons, opacity, animations |
| **Config Layer** | Gameplay values | HP, damage, timers, speed, counts, toggles |

### UI Layer Parameters
- **Sprite** — Logo, icons, backgrounds, characters (`spriteFrame`, `spriteColor`, `position`, `scale`)
- **Label** — All text (`string`, `labelColor`, `fontSize`, `outline`, `shadow`)
- **Button** — CTA buttons (`spriteFrame`, `labelString`, `labelColor`, `labelFontSize`)
- **Color** — Any color value (hex format: `#FF5722` or with alpha: `#FF572280`)

### Config Layer Parameters
- **Number** — HP, damage, timer duration, speed, counts
- **Boolean** — Show/hide toggles, enable/disable features
- **Range** — Sliders with min/max (difficulty, volume)
- **Select** — Dropdown choices (presets, themes)

### Composite Parameters
- **End Card** — Background + title + subtitle + CTA button
- **Loading Screen** — Background color + icon + game name
- **Tutorial Hand** — Hand sprite + animation preset
- **Rich Text** — Label + entrance/exit animations

📋 **[Full parameter reference →](reference/whats-included.md)**

---

## Need Something More?

Parameters not in your dashboard require development. See [Custom Development](help/custom-development.md).

---

## Get Started

1. **[Quick Start](getting-started/quick-start.md)** — Make your first change
2. **[Common Tasks](getting-started/common-tasks.md)** — Essential customizations checklist
3. **[Common Parameters](reference/common-parameters.md)** — Full reference list
