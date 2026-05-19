# Phase 7: Game Settings

**Priority:** P2
**Status:** Pending
**Effort:** S (~1 day)

## Overview

Document how users can adjust gameplay values like difficulty, timing, and speed settings. These are Config Layer parameters that may require approval.

## Technical Alignment

Maps to: Config Layer from `t1k-cocos-cocos-base-playable-parameter`

| Setting Type | Technical Type | Example |
|--------------|----------------|---------|
| Difficulty | `NumberParameter` | Enemy HP, damage values |
| Timing | `NumberParameter` | Timer duration, delays |
| Speed | `NumberParameter` | Movement speed, animation speed |
| Flags | `BooleanParameter` | Enable/disable features |

**Note:** Config layer parameters may require approval before changes take effect.

## Files to Create

```
docs/handbook/game-settings/
  difficulty.md
  timing-speed.md
  gameplay-values.md
```

## Content Outline

### difficulty.md
- What affects difficulty
- Adjusting challenge level
- Enemy stats (if available)
- Player advantages
- Screenshot: Difficulty settings

### timing-speed.md
- Timer durations
- Animation speeds
- Transition timings
- Screenshot: Timing settings

### gameplay-values.md
- Point values
- Combo multipliers
- Reward amounts
- Feature toggles
- Screenshot: Gameplay config

## Screenshot Placeholders

| Screenshot | Description |
|------------|-------------|
| `difficulty-settings.png` | Difficulty adjustment panel |
| `timing-options.png` | Timer/speed settings |
| `gameplay-config.png` | Gameplay values panel |
| `toggle-features.png` | Feature toggles |

## Use Cases

| User Wants To | Solution |
|---------------|----------|
| "Make game easier" | Adjust difficulty values |
| "Shorten the timer" | Change timer duration |
| "Speed up animations" | Modify animation speed |
| "Disable a feature" | Toggle feature off |

## Config Layer Approval Note

```markdown
### Why Do Some Changes Need Approval?

Game settings affect how the game plays, not just how it looks. 
To ensure the best player experience, some changes may need review 
before they go live.

**Visual changes (instant):**
- Colors, images, text styling

**Gameplay changes (may need review):**
- Difficulty adjustments
- Timer durations
- Speed modifications

You'll see a note on any setting that requires approval.
```

## Success Criteria

- [ ] User understands difficulty options
- [ ] User can adjust timing/speed
- [ ] User knows about approval process
- [ ] User can toggle features

## FREE Indicator

```markdown
> **FREE** - All game settings adjustments are included at no extra cost
> 
> *Note: Some gameplay changes may require brief review before going live*
```

## Implementation Steps

1. Create `game-settings/` directory
2. Write difficulty.md
3. Write timing-speed.md
4. Write gameplay-values.md
5. Add screenshot placeholders
6. Add approval process explanation
7. Add FREE banners with review note
