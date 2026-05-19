# Game UI Elements

Customize UI styling: health bars, timers, scores, currency displays.

> **Note:** These are visual styling parameters. Game logic changes require development.

## HP Bars

Health bars show player or enemy health status.

### Parameters

| Property | What It Does |
|----------|--------------|
| Main Color | The health fill color |
| Indicator Color | Damage flash or secondary color |
| Background Color | The empty bar background |
| Border | Outline around the bar |

### Common Color Schemes

| Style | Main | Indicator | Background |
|-------|------|-----------|------------|
| Classic | Green | Yellow | Dark gray |
| Modern | Teal | White | Black |
| Aggressive | Red | Orange | Dark red |
| Brand | Your primary | Your accent | Neutral |

### HP Bar Anatomy

```
[##########..........] 50% HP
 ^         ^
 |         |
 Fill      Empty (background)
```

## Timers

Timer displays show countdowns or elapsed time.

### Parameters

| Property | What It Does |
|----------|--------------|
| Text Color | Timer number color |
| Background | Container background |
| Warning Color | Color when time is low |
| Font Style | Timer text appearance |

### Timer States

| State | Typical Color |
|-------|---------------|
| Normal | White or brand color |
| Warning | Yellow or orange |
| Critical | Red |

## Score Displays

Score counters show points earned during gameplay.

### Parameters

| Property | What It Does |
|----------|--------------|
| Text Color | Score number color |
| Background | Score container background |
| Icon | Coin or point icon |
| Animation | Pop or glow on score change |

## Currency Displays

Currency shows in-game money or collectibles.

### Parameters

| Property | What It Does |
|----------|--------------|
| Icon | Currency symbol or image |
| Text Color | Amount color |
| Background | Container background |

## Best Practices

### Color Choices

* **Match your brand** - Use brand colors where appropriate
* **Maintain clarity** - UI must be readable at a glance
* **Use contrast** - Numbers visible against backgrounds
* **Be consistent** - Same style across all UI elements

### Visual Hierarchy

* Most important info (HP, time) should be most visible
* Secondary info (score, currency) can be subtler
* Warning states should stand out

## What You Cannot Change

| You CAN change | You CANNOT change |
|----------------|-------------------|
| Bar colors | HP amounts |
| Timer style | Timer duration |
| Score appearance | Point values |
| Currency icon | Currency amounts |

For gameplay values, see [Difficulty & Balance](difficulty.md) and [Gameplay Values](values.md).

## Related

* [Difficulty & Balance](difficulty.md) - Adjust gameplay values
* [Colors & Themes](../branding/colors.md) - Brand color application
