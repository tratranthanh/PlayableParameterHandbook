# Loading Screen

The first thing users see while your playable ad loads.

<figure><img src="../.gitbook/assets/loading-screen-elements.png" alt="Loading Screen Elements"><figcaption>Loading screen components: Background, Logo, Icon, Game Name</figcaption></figure>

---

## LoadingScreenParameter (Composite)

Loading screens use the `LoadingScreenParameter` composite type, which bundles:

| Component | Parameter Type | What You Can Change |
|-----------|---------------|---------------------|
| Background | `ColorParameter` | Solid background color |
| Icon | `SpriteParameter` | `spriteFrame`, `spriteColor` |
| Game Name | `LabelParameter` | `string`, `labelColor`, `fontSize` |
| Logo | `SpriteParameter` | `spriteFrame`, `position`, `scale` |

---

## Background

### ColorParameter

| Property | Type | Description | Example |
|----------|------|-------------|---------|
| Color value | `ColorParameter` | Solid background | `#1A1A2E` |

### Background Tips

| Goal | Approach |
|------|----------|
| Brand alignment | Use brand primary color |
| Dark theme | `#1A1A2E`, `#0D0D0D`, `#121212` |
| Light theme | `#FFFFFF`, `#F5F5F5`, `#FAFAFA` |
| High contrast | Ensure logo/text readable against it |

---

## Loading Icon

### SpriteParameter Properties

| Property | Type | Description | Example |
|----------|------|-------------|---------|
| `spriteFrame` | `ImageParameter` | Spinner/indicator image | Upload PNG |
| `spriteColor` | `ColorParameter` | Icon color tint | `#FFFFFF` |
| `enable` | `BooleanParameter` | Show or hide | `true` |
| `scale` | `CoordinatesParameter` | Size | `{x: 1.0, y: 1.0}` |

<figure><img src="../.gitbook/assets/loading-indicator-types.png" alt="Loading Indicator Types"><figcaption>Options: Spinner, Progress bar, Animated icon, None</figcaption></figure>

### Loading Indicator Types

| Type | Description | When to Use |
|------|-------------|-------------|
| Spinner | Rotating circular icon | Standard, always appropriate |
| Progress bar | Filling horizontal bar | When actual progress is trackable |
| Animated icon | Custom branded animation | Strong brand identity |
| None | Just logo/background | Minimal, fast-loading ads |

---

## Game Name

### LabelParameter Properties

| Property | Type | Description | Example |
|----------|------|-------------|---------|
| `string` | `TextParameter` | Game title text | `"My Game"` |
| `labelColor` | `ColorParameter` | Text color | `#FFFFFF` |
| `fontSize` | `NumberParameter` | Text size | `48` |
| `isBold` | `BooleanParameter` | Bold weight | `true` |
| `enable` | `BooleanParameter` | Show or hide | `true` |

---

## Logo

### SpriteParameter Properties

| Property | Type | Description | Example |
|----------|------|-------------|---------|
| `spriteFrame` | `ImageParameter` | Logo image | Upload PNG (transparent) |
| `spriteColor` | `ColorParameter` | Color tint | `#FFFFFF` (no tint) |
| `position` | `CoordinatesParameter` | Location | `{x: 0, y: 100}` |
| `scale` | `CoordinatesParameter` | Size | `{x: 1.0, y: 1.0}` |
| `enable` | `BooleanParameter` | Show or hide | `true` |

### Logo Tips

| Requirement | Specification |
|-------------|---------------|
| Format | PNG with transparent background |
| Size | 512 x 512 pixels minimum |
| File size | Under 500KB |

---

## Best Practices

### First Impressions

| Element | Recommendation |
|---------|----------------|
| Background | Brand color or simple solid |
| Logo | Centered, appropriately sized |
| Game name | Clear, readable font |
| Loading indicator | Subtle but visible |

### What to Avoid

| Issue | Problem |
|-------|---------|
| Cluttered layout | Overwhelms before gameplay |
| Hard-to-read text | Frustrates users |
| Generic/default look | Misses branding opportunity |
| Mismatched colors | Looks unprofessional |

### Visual Hierarchy

```
┌─────────────────────────────────┐
│                                 │
│           [ LOGO ]              │  ← Primary focus
│                                 │
│          Game Name              │  ← Secondary
│                                 │
│            ◌                    │  ← Loading indicator
│                                 │
└─────────────────────────────────┘
```

---

## Loading Screen Flow

```
User taps ad → Loading screen appears → Assets load → Gameplay starts
                    ↑
              Your branding
              opportunity
```

---

## Configuration Example

| Component | Value |
|-----------|-------|
| Background | `#1A1A2E` (dark blue) |
| Logo | Your brand logo (PNG, transparent) |
| Game Name | `"My Awesome Game"` |
| Game Name Color | `#FFFFFF` (white) |
| Loading Icon | Spinner, `#FFFFFF` tint |

---

## Related

- [Tutorial](tutorial.md) — What users see next
- [End Cards](end-cards.md) — Final screens
- [Logos & Icons](../branding/logos-icons.md) — Logo specifications
- [Colors](../branding/colors.md) — Color consistency
