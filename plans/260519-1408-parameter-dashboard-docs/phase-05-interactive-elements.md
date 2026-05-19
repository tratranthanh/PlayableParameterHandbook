# Phase 5: Interactive Elements

**Priority:** P1
**Status:** Pending
**Effort:** S (~1 day)

## Overview

Document how users can customize interactive elements like buttons, toggles, sliders, and other clickable/tappable components.

## Technical Alignment

Maps to: `ButtonParameter`, `ToggleParameter`, `SliderParameter` from `t1k-cocos-cocos-base-playable-parameter`

### ButtonParameter Fields

| Dashboard Field | Technical Field | User-Friendly Name |
|-----------------|-----------------|-------------------|
| Button image | `spriteFrame` | "Button Background" |
| Button color | `spriteColor` | "Button Color" |
| Button text | `labelString` | "Button Text" |
| Text color | `labelColor` | "Text Color" |
| Text size | `labelFontSize` | "Text Size" |

## Files to Create

```
docs/handbook/interactive-elements/
  buttons.md
  toggles-switches.md
  sliders.md
```

## Content Outline

### buttons.md
- Customizing CTA buttons
- Button background images
- Button text and styling
- Button colors
- Screenshot: Button editor panel

### toggles-switches.md
- On/Off toggles
- Toggle colors
- Toggle states
- Screenshot: Toggle options

### sliders.md
- Volume/progress sliders
- Slider track colors
- Slider handle customization
- Screenshot: Slider settings

## Screenshot Placeholders

| Screenshot | Description |
|------------|-------------|
| `button-editor.png` | Button customization panel |
| `button-before-after.png` | Button transformation example |
| `toggle-options.png` | Toggle switch settings |
| `slider-customization.png` | Slider settings panel |

## Use Cases

| User Wants To | Solution |
|---------------|----------|
| "Change 'Play Now' button" | Edit CTA button settings |
| "Match button to brand" | Change button color/image |
| "Update button text" | Edit button label |
| "Customize settings toggle" | Modify toggle appearance |

## CTA Button Best Practices

```markdown
### Call-to-Action Tips

Your CTA button is the most important element! Here are best practices:

1. **Clear text** - Use action words like "Play Now", "Download", "Try Free"
2. **Contrasting color** - Make it stand out from the background
3. **Readable size** - Large enough to tap easily on mobile
4. **Brand aligned** - Use your brand's accent color
```

## Success Criteria

- [ ] User can customize CTA buttons
- [ ] User can change button text
- [ ] User understands toggle options
- [ ] User can modify sliders

## FREE Indicator

```markdown
> **FREE** - All interactive element changes are included at no extra cost
```

## Implementation Steps

1. Create `interactive-elements/` directory
2. Write buttons.md
3. Write toggles-switches.md
4. Write sliders.md
5. Add screenshot placeholders
6. Add CTA best practices
7. Add FREE banners
