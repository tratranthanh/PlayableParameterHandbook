# All Parameters Reference

Quick lookup for all customizable parameters in the Parameter Dashboard.

## Images & Colors

| Parameter | Type | Location | Example | Limits |
|-----------|------|----------|---------|--------|
| Logo | Image | Images > Logos | 512x512 PNG | 500KB max |
| App Icon | Image | Images > Icons | 256x256 PNG | 300KB max |
| Primary Color | Color | Images > Colors | #FF5722 | Hex format |
| Secondary Color | Color | Images > Colors | #0066CC | Hex format |
| Background Image | Image | Images > Backgrounds | 1920x1080 | 2MB max |
| Button Background | Color | Images > Buttons | #00C853 | Hex format |
| Button Text | Text | Images > Buttons | "Play Now" | 25 chars |
| Headline | Text | Images > Text | "Your Game" | 50 chars |

## Gameplay

| Parameter | Type | Location | Example | Limits |
|-----------|------|----------|---------|--------|
| Difficulty | Number | Gameplay > Difficulty | 5 | 1-10 |
| Timer Duration | Number | Gameplay > Timing | 45 | seconds |
| Player HP | Number | Gameplay > Difficulty | 100 | varies |
| Enemy HP | Number | Gameplay > Difficulty | 50 | varies |
| Movement Speed | Number | Gameplay > Timing | 1.0 | multiplier |
| Point Value | Number | Gameplay > Values | 100 | per action |
| Target Score | Number | Gameplay > Values | 1000 | win threshold |

## Game UI

| Parameter | Type | Location | Example | Limits |
|-----------|------|----------|---------|--------|
| HP Bar Color | Color | Gameplay > UI | #00FF00 | Hex format |
| HP Background | Color | Gameplay > UI | #333333 | Hex format |
| Timer Color | Color | Gameplay > UI | #FFFFFF | Hex format |
| Score Color | Color | Gameplay > UI | #FFD700 | Hex format |
| Currency Icon | Image | Gameplay > UI | 64x64 PNG | 100KB max |

## Screens

| Parameter | Type | Location | Example | Limits |
|-----------|------|----------|---------|--------|
| Loading Background | Color/Image | Screens > Loading | #000000 | 2MB max |
| Loading Text | Text | Screens > Loading | "Loading..." | 30 chars |
| Tutorial Text | Text | Screens > Tutorial | "Tap here!" | 50 chars |
| Win Title | Text | Screens > End Cards | "You Won!" | 30 chars |
| Win Subtitle | Text | Screens > End Cards | "Great job!" | 50 chars |
| Lose Title | Text | Screens > End Cards | "Try Again" | 30 chars |
| CTA Text | Text | Screens > End Cards | "Download Now" | 25 chars |

## Feature Toggles

| Parameter | Type | Location | Default |
|-----------|------|----------|---------|
| Show Tutorial | Boolean | Gameplay > Values | On |
| Sound Effects | Boolean | Gameplay > Values | On |
| Haptics | Boolean | Gameplay > Values | On |
| Power-ups | Boolean | Gameplay > Values | Varies |

## How to Use This Reference

1. **Find the parameter** you want to change
2. **Note the Location** column for where to find it
3. **Check Limits** before preparing your assets
4. **Follow the Example** format for values

## Notes

* All colors use hex format (#RRGGBB)
* Image formats: PNG (transparency) or JPG (photos)
* Character limits are approximate; check dashboard for exact limits
* Number ranges vary by game; dashboard shows actual bounds

## Related

* [File Formats](file-formats.md) - Detailed format specifications
* [Limits & Constraints](limits.md) - Size and character limits
