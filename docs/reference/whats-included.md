# What's Included

Every parameter visible in your dashboard is included at no extra cost. This page explains exactly what you can customize.

---

## The Two-Layer System

Your playable ad parameters are organized into two layers:

| Layer | What It Controls | Examples |
|-------|------------------|----------|
| **UI Layer** | Visual appearance | Images, text, colors, button styling, opacity |
| **Config Layer** | Gameplay values | HP, damage, timers, speed, counts, toggles |

**Both layers are included** — if you see the parameter in your dashboard, you can change it.

---

## UI Layer Parameters

Visual components that change how things look.

### Sprite Parameters (Images)

Control any image element in your playable.

| Property | What It Does | Example Value |
|----------|--------------|---------------|
| `spriteFrame` | The image file | Upload PNG/JPG |
| `spriteColor` | Tint overlay color | `#FFFFFF` (white = no tint) |
| `enable` | Show or hide | `true` / `false` |
| `position` | Location on screen | `{x: 0, y: 100}` |
| `scale` | Size multiplier | `{x: 1.0, y: 1.0}` |
| `contentSize` | Explicit dimensions | `{x: 512, y: 512}` |

**Common uses:** Logo, app icon, backgrounds, character sprites, UI icons, currency icons

---

### Label Parameters (Text)

Control any text element in your playable.

| Property | What It Does | Example Value |
|----------|--------------|---------------|
| `string` | The text content | `"Download Now"` |
| `labelColor` | Text color | `#FFFFFF` |
| `fontSize` | Text size | `48` |
| `lineHeight` | Line spacing | `0` (auto) |
| `isBold` | Bold style | `true` / `false` |
| `isItalic` | Italic style | `true` / `false` |
| `isUnderline` | Underline style | `true` / `false` |
| `outlineColor` | Text outline color | `#000000` |
| `outlineWidth` | Outline thickness | `2` (0 = none) |
| `shadowColor` | Drop shadow color | `#000000` |
| `shadowOffset` | Shadow position | `{x: 2, y: -2}` |
| `enable` | Show or hide | `true` / `false` |
| `position` | Location on screen | `{x: 0, y: 200}` |

**Common uses:** Headlines, CTA text, instructions, score labels, timer text, tutorial text

---

### Button Parameters

Buttons combine a sprite background with a text label.

| Property | What It Does | Example Value |
|----------|--------------|---------------|
| `spriteFrame` | Button background image | Upload PNG |
| `spriteColor` | Background tint | `#FF5722` |
| `labelString` | Button text | `"Play Now"` |
| `labelColor` | Text color | `#FFFFFF` |
| `labelFontSize` | Text size | `36` |
| `labelBold` | Bold text | `true` / `false` |
| `labelOutlineColor` | Text outline | `#000000` |
| `labelOutlineWidth` | Outline thickness | `0` |
| `enable` | Show or hide | `true` / `false` |
| `position` | Location on screen | `{x: 0, y: -200}` |
| `scale` | Size multiplier | `{x: 1.0, y: 1.0}` |

**Common uses:** CTA button, play button, retry button, skip button

---

### Color Parameters

Standalone color values for UI elements.

| Format | Example | Notes |
|--------|---------|-------|
| Hex (no alpha) | `#FF5722` | Solid color |
| Hex (with alpha) | `#FF572280` | 50% transparent |

**Common uses:** HP bar fill, timer warning color, score highlight, UI backgrounds

---

## Config Layer Parameters

Gameplay values that change how the game plays.

### Number Parameters

| Property | What It Does | Example Value |
|----------|--------------|---------------|
| Timer duration | Countdown time | `30` (seconds) |
| Player HP | Health points | `100` |
| Enemy HP | Enemy health | `50` |
| Damage value | Attack strength | `25` |
| Speed multiplier | Movement speed | `1.5` |
| Spawn count | Number of enemies | `5` |
| Attempt limit | Max tries | `3` |
| Cooldown | Wait between actions | `2.0` (seconds) |

---

### Boolean Parameters (Toggles)

| Property | What It Does | Values |
|----------|--------------|--------|
| Show tutorial | Display tutorial | `true` / `false` |
| Show timer | Display countdown | `true` / `false` |
| Show score | Display points | `true` / `false` |
| Show HP bar | Display health | `true` / `false` |
| Enable sound | Play audio | `true` / `false` |
| Enable haptics | Vibration feedback | `true` / `false` |

---

### Range Parameters (Sliders)

Numbers with defined minimum and maximum.

| Property | Range | Example |
|----------|-------|---------|
| Difficulty | 1-10 | `5` |
| Volume | 0-100 | `80` |
| Speed | 0.5-2.0 | `1.0` |

---

### Select Parameters (Dropdowns)

Choose from predefined options.

| Property | Options | Example |
|----------|---------|---------|
| Difficulty preset | Easy, Medium, Hard | `Medium` |
| Theme | Light, Dark, Custom | `Dark` |
| Language | EN, ES, FR, etc. | `EN` |

---

## Composite Parameters

Pre-built combinations that control entire screens or complex elements.

### End Card Parameter

Controls the entire win/lose screen.

| Component | What You Can Change |
|-----------|---------------------|
| Background | Image or color |
| Title | Text, color, size, outline |
| Subtitle | Text, color, size |
| CTA Button | Image, text, colors, size |

---

### Loading Screen Parameter

Controls the loading screen appearance.

| Component | What You Can Change |
|-----------|---------------------|
| Background | Solid color |
| Icon | Loading spinner image |
| Game Name | Text, color, size |

---

### Tutorial Hand Parameter

Controls the animated tutorial indicator.

| Component | What You Can Change |
|-----------|---------------------|
| Hand Image | Sprite and color |
| Animation | Preset animation style |

---

### Rich Text Parameter

Text with entrance/exit animations.

| Component | What You Can Change |
|-----------|---------------------|
| Text | Content, color, size, styling |
| Entrance Animation | Fade, slide, scale, etc. |
| Exit Animation | Fade, slide, scale, etc. |
| Auto Hide | Duration before hiding |

---

## Animation Presets

Built-in animation styles you can apply to any compatible element.

| Category | Presets |
|----------|---------|
| **Entrance** | Fade In, Scale Up, Slide In, Bounce In, Pop |
| **Emphasis** | Pulse, Shake, Bounce, Wiggle, Glow |
| **Exit** | Fade Out, Scale Down, Slide Out, Shrink |
| **Interactive** | Tap, Press, Swipe, Drag |

---

## Audio Parameters

Sound customization options.

| Property | What It Does | Format |
|----------|--------------|--------|
| Background Music | Looping audio track | MP3/OGG |
| Sound Effects | One-shot audio clips | MP3/OGG |
| Volume | Audio level | 0-100 |
| Mute | Disable all audio | `true` / `false` |

---

## What's NOT Included

These require [Custom Development](../help/custom-development.md):

| Category | Examples |
|----------|----------|
| **New game mechanics** | New enemy types, new power-ups, new win conditions |
| **New AI behavior** | Smarter enemies, dynamic difficulty, pathfinding |
| **New spawn patterns** | Wave systems, procedural generation |
| **Asset processing** | Generate map from image, new animation frames |
| **New UI systems** | New screen types, new interactions |
| **New parameters** | Adding parameters that don't exist in current build |

**Rule of thumb:** If the parameter isn't in your dashboard, it doesn't exist in your build yet.

---

## Related

- [Common Parameters](common-parameters.md) — Quick reference of typical parameters
- [Custom Development](../help/custom-development.md) — Request new features
- [File Formats](file-formats.md) — Asset specifications
