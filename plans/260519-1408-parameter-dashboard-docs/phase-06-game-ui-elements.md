# Phase 6: Game UI Elements

**Priority:** P1
**Status:** Pending
**Effort:** M (~3 days)

## Overview

Document how users can customize game-specific UI elements like HP bars, timers, score displays, and currency indicators.

## Technical Alignment

Maps to: Custom Composites from `t1k-cocos-cocos-base-playable-parameter-composite`

| UI Element | Composite Type | Fields |
|------------|----------------|--------|
| HP Bar | `HPBarUIParameter` | Main color, indicator, background |
| Timer | `LabelParameter` | Color, size, position (string excluded - game-managed) |
| Score | `LabelParameter` | Color, size, position (string excluded - game-managed) |
| Currency | Custom composite | Icon, text color, position |

## Files to Create

```
docs/handbook/game-ui/
  hp-bars.md
  timers.md
  score-displays.md
  currency.md
```

## Content Outline

### hp-bars.md
- What HP bars show
- Changing bar colors
- Main health color
- Damage indicator color
- Background color
- Screenshot: HP bar color options

### timers.md
- Timer display styling
- Timer text color
- Timer text size
- Position adjustments
- Note: Timer numbers are game-controlled
- Screenshot: Timer customization

### score-displays.md
- Score text styling
- Score colors
- Score effects (if available)
- Note: Score numbers are game-controlled
- Screenshot: Score display options

### currency.md
- Currency icon replacement
- Currency text styling
- Coin/gem indicators
- Screenshot: Currency UI options

## Screenshot Placeholders

| Screenshot | Description |
|------------|-------------|
| `hp-bar-colors.png` | HP bar color customization |
| `hp-bar-example.png` | Before/after HP bar |
| `timer-styling.png` | Timer text options |
| `score-display.png` | Score styling panel |
| `currency-ui.png` | Currency indicator options |

## Use Cases

| User Wants To | Solution |
|---------------|----------|
| "Change HP bar to red/green" | Edit HP bar colors |
| "Match timer to brand" | Change timer text color |
| "Style the score display" | Modify score text settings |
| "Use custom coin icon" | Replace currency icon |

## Important Note: Game-Managed Values

```markdown
### Why Can't I Change the Numbers?

Some values like timer countdown, score totals, and HP amounts are 
controlled by the game logic. You can style how they look, but the 
actual numbers are determined by gameplay.

**What you CAN change:**
- Colors
- Sizes
- Fonts
- Positions

**What the game controls:**
- Timer countdown numbers
- Score values
- HP/health amounts
```

## Success Criteria

- [ ] User can customize HP bar colors
- [ ] User understands game-managed values
- [ ] User can style timer/score displays
- [ ] User can customize currency UI

## FREE Indicator

```markdown
> **FREE** - All game UI styling is included at no extra cost
```

## Implementation Steps

1. Create `game-ui/` directory
2. Write hp-bars.md
3. Write timers.md
4. Write score-displays.md
5. Write currency.md
6. Add screenshot placeholders
7. Add game-managed values explanation
8. Add FREE banners
