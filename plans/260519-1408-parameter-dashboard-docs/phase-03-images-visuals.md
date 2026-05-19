# Phase 3: Images & Visuals

**Priority:** P1
**Status:** Pending
**Effort:** S (~1 day)

## Overview

Document how users can replace images throughout the playable ad, including logos, icons, backgrounds, and character sprites.

## Technical Alignment

Maps to: `SpriteParameter` from `t1k-cocos-cocos-base-playable-parameter`

| Dashboard Field | Technical Field | User-Friendly Name |
|-----------------|-----------------|-------------------|
| Image file | `spriteFrame` | "Image" |
| Visibility | `enable` | "Show/Hide" |
| Image tint | `spriteColor` | "Color Overlay" |
| Size | `contentSize` | "Size" |
| Position | `position` | "Position" |

## Files to Create

```
docs/handbook/images-visuals/
  replacing-images.md
  logos-icons.md
  backgrounds.md
```

## Content Outline

### replacing-images.md
- Finding image elements in the dashboard
- Uploading new images
- Supported file formats (PNG, JPG)
- Image size recommendations
- Screenshot: Image upload interface

### logos-icons.md
- Replacing your brand logo
- Changing app icons
- Icon size requirements
- Transparency support
- Screenshot: Logo replacement example

### backgrounds.md
- Changing background images
- Full-screen backgrounds
- Tiled vs stretched
- Screenshot: Background options

## Screenshot Placeholders

| Screenshot | Description |
|------------|-------------|
| `image-upload-panel.png` | Image upload interface |
| `logo-replacement.png` | Logo before/after |
| `background-options.png` | Background settings |
| `image-formats.png` | Supported formats guide |

## Use Cases

| User Wants To | Solution |
|---------------|----------|
| "Use my company logo" | Replace logo image |
| "Change the background" | Upload new background |
| "Update character images" | Replace sprite images |
| "Hide an element" | Toggle visibility off |

## Image Guidelines

Include technical specs in user-friendly format:

| Element Type | Recommended Size | Format |
|--------------|-----------------|--------|
| Logo | 512x512 px | PNG (transparent) |
| Background | 1920x1080 px | JPG or PNG |
| Icon | 256x256 px | PNG (transparent) |
| Character | Original aspect ratio | PNG (transparent) |

## Success Criteria

- [ ] User can upload new images
- [ ] User understands size requirements
- [ ] User can replace logos/icons
- [ ] User can change backgrounds

## FREE Indicator

```markdown
> **FREE** - All image changes are included at no extra cost
```

## Implementation Steps

1. Create `images-visuals/` directory
2. Write replacing-images.md
3. Write logos-icons.md
4. Write backgrounds.md
5. Add screenshot placeholders
6. Add image spec tables
7. Add FREE banners
