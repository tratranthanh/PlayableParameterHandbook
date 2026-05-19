# Gameplay

Adjust gameplay elements in your playable ad.

> **Note:** Each playable has different parameters. Below are common examples.

## What's in This Section

| Topic | What You'll Learn |
|-------|-------------------|
| [Game UI Elements](ui-elements.md) | Style HP bars, timers, scores, currency |
| [Difficulty & Balance](difficulty.md) | Adjust challenge level |
| [Timing & Speed](timing.md) | Control game pacing |
| [Gameplay Values](values.md) | Modify points, rewards, thresholds |

## Parameter Types

| Type | Examples |
|------|----------|
| **UI Styling** | HP bar colors, timer style, score display |
| **Simple Config** | Timer duration, HP values, speed multipliers |
| **Visibility** | Show/hide tutorial, UI elements |
| **Animation Presets** | UI entrance/exit animations (speed/delay adjustable) |

## UI Styling vs Game Logic

| UI Styling (adjustable) | Game Logic (requires development) |
|-------------------------|-----------------------------------|
| HP bar colors | HP calculation formulas |
| Timer display style | Timer behavior logic |
| Score appearance | Point calculation systems |
| Animation presets | New game mechanics |

## Animation Presets for Game UI

If the UI component exists in your build:
- Fade In/Out, Scale In/Out for panels
- Bounce, Pulse for feedback
- Typewriter for text reveals

Configurable: preset type, speed, delay, loop.

## Need Something Custom?

AI behavior, spawn patterns, or new mechanics not in your dashboard? See [Custom Development](../help/custom-development.md).
