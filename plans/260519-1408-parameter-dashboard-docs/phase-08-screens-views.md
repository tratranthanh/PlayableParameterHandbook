# Phase 8: Screens & Views

**Priority:** P1
**Status:** Pending
**Effort:** M (~3 days)

## Overview

Document how users can customize full screen experiences like loading screens, tutorial overlays, and end cards (win/lose screens).

## Technical Alignment

Maps to: Composite parameters from `t1k-cocos-cocos-base-playable-parameter`

| Screen | Composite Type | Components |
|--------|----------------|------------|
| Loading Screen | `LoadingScreenParameter` | Background color, icon, game name |
| Tutorial | `TutorialHandParameter`, `RichTextParameter` | Hand sprite, tutorial text |
| End Card (Win) | `EndCardParameter` | Background, title, subtitle, CTA button |
| End Card (Lose) | `EndCardParameter` | Background, title, subtitle, CTA button |

## Files to Create

```
docs/handbook/screens-views/
  loading-screen.md
  tutorial.md
  end-cards.md
```

## Content Outline

### loading-screen.md
- Loading screen purpose
- Background color
- Loading icon/animation
- Game name text
- Screenshot: Loading screen editor

### tutorial.md
- Tutorial overlay
- Tutorial text styling
- Hand/pointer icon
- Animation settings
- Screenshot: Tutorial customization

### end-cards.md
- Win screen customization
- Lose screen customization
- Background images
- Title and subtitle text
- CTA button (most important!)
- Screenshot: End card editor

## Screenshot Placeholders

| Screenshot | Description |
|------------|-------------|
| `loading-screen-editor.png` | Loading screen settings |
| `loading-before-after.png` | Loading screen transformation |
| `tutorial-editor.png` | Tutorial customization |
| `tutorial-hand.png` | Hand/pointer options |
| `endcard-win.png` | Win screen editor |
| `endcard-lose.png` | Lose screen editor |
| `endcard-cta.png` | CTA button focus |

## Use Cases

| User Wants To | Solution |
|---------------|----------|
| "Brand the loading screen" | Change colors, icon, name |
| "Customize tutorial" | Edit tutorial text and hand |
| "Update win screen" | Modify end card settings |
| "Change CTA on end card" | Edit end card button |

## End Card Best Practices

```markdown
### Making Effective End Cards

End cards are your final chance to convert players! Tips:

**Win Screen:**
- Celebrate the achievement
- Strong CTA: "Keep Playing!" or "Download Now!"
- Bright, positive colors

**Lose Screen:**
- Encourage retry or download
- CTA: "Try Again!" or "Get the Full Game!"
- Don't be too negative

**Both:**
- Clear, readable text
- Prominent CTA button
- Brand-aligned design
```

## Success Criteria

- [ ] User can customize loading screen
- [ ] User can edit tutorial elements
- [ ] User can customize both end cards
- [ ] User understands CTA importance

## FREE Indicator

```markdown
> **FREE** - All screen customizations are included at no extra cost
```

## Implementation Steps

1. Create `screens-views/` directory
2. Write loading-screen.md
3. Write tutorial.md
4. Write end-cards.md
5. Add screenshot placeholders
6. Add end card best practices
7. Add FREE banners
