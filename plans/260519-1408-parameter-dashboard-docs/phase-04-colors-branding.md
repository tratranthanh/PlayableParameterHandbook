# Phase 4: Colors & Branding

**Priority:** P1
**Status:** Pending
**Effort:** S (~1 day)

## Overview

Document how users can customize colors throughout the playable ad to match their brand identity, including UI colors, backgrounds, and visual effects.

## Technical Alignment

Maps to: `ColorParameter` from `t1k-cocos-cocos-base-playable-parameter`

| Dashboard Field | Technical Field | User-Friendly Name |
|-----------------|-----------------|-------------------|
| Color value | `color` | "Color" |
| Opacity | `alpha` or `UIOpacity` | "Transparency" |

## Files to Create

```
docs/handbook/colors-branding/
  brand-colors.md
  ui-colors.md
  gradients-effects.md
```

## Content Outline

### brand-colors.md
- Why consistent branding matters
- Using your brand color palette
- Color picker tool
- Hex code support
- Screenshot: Color picker panel

### ui-colors.md
- Button colors
- Text colors
- Background colors
- Border colors
- Screenshot: UI color examples

### gradients-effects.md
- Gradient backgrounds (if supported)
- Color overlays
- Transparency/opacity
- Screenshot: Effect examples

## Screenshot Placeholders

| Screenshot | Description |
|------------|-------------|
| `color-picker.png` | Color picker interface |
| `hex-input.png` | Hex code entry |
| `brand-colors-example.png` | Before/after branding |
| `ui-colors-panel.png` | UI color options |

## Use Cases

| User Wants To | Solution |
|---------------|----------|
| "Match my brand colors" | Enter brand hex codes |
| "Change button color" | Edit button background color |
| "Make text match brand" | Change text color |
| "Adjust transparency" | Modify opacity slider |

## Brand Color Guide

Include helpful tips:

```markdown
### Finding Your Brand Colors

Most companies have official brand guidelines with hex codes like:
- Primary: #FF5722
- Secondary: #2196F3
- Accent: #4CAF50

**Tip:** Ask your marketing team for the brand color guide!
```

## Color Accessibility Note

```markdown
### Accessibility Tip

Make sure your text colors have enough contrast against backgrounds.
- Dark text on light backgrounds
- Light text on dark backgrounds

Good contrast helps everyone read your ad clearly!
```

## Success Criteria

- [ ] User can use brand colors
- [ ] User understands color picker
- [ ] User can input hex codes
- [ ] User knows about accessibility

## FREE Indicator

```markdown
> **FREE** - All color changes are included at no extra cost
```

## Implementation Steps

1. Create `colors-branding/` directory
2. Write brand-colors.md
3. Write ui-colors.md
4. Write gradients-effects.md
5. Add screenshot placeholders
6. Add accessibility guidance
7. Add FREE banners
