# Phase 2: Text & Headlines

**Priority:** P1
**Status:** Pending
**Effort:** S (~1 day)

## Overview

Document how users can customize text elements throughout the playable ad, including game titles, instructions, button labels, and tutorial text.

## Technical Alignment

Maps to: `LabelParameter` from `t1k-cocos-cocos-base-playable-parameter`

| Dashboard Field | Technical Field | User-Friendly Name |
|-----------------|-----------------|-------------------|
| Text content | `string` | "Text" |
| Text color | `labelColor` | "Color" |
| Font size | `fontSize` | "Size" |
| Bold | `isBold` | "Bold" |
| Italic | `isItalic` | "Italic" |
| Underline | `isUnderline` | "Underline" |
| Outline | `outlineWidth`, `outlineColor` | "Text Outline" |

## Files to Create

```
docs/handbook/text-headlines/
  changing-text.md
  text-styles.md
  multilingual.md
```

## Content Outline

### changing-text.md
- Finding text elements in the dashboard
- Editing text content
- Character limits (if any)
- Special characters support
- Screenshot: Text editor panel

### text-styles.md
- Changing text color
- Adjusting font size
- Bold, italic, underline
- Adding text outlines
- Screenshot: Style options panel

### multilingual.md
- How to handle different languages
- Text length considerations
- Right-to-left languages note
- Screenshot: Multi-language example

## Screenshot Placeholders

| Screenshot | Description |
|------------|-------------|
| `text-editor-panel.png` | Text editing interface |
| `text-color-picker.png` | Color picker for text |
| `text-styles-panel.png` | Font style options |
| `text-before-after.png` | Before/after example |

## Use Cases

| User Wants To | Solution |
|---------------|----------|
| "Change the game title" | Edit title text element |
| "Make CTA button say 'Download Now'" | Edit button label text |
| "Use my brand font color" | Change text color to brand hex |
| "Make tutorial text bigger" | Increase font size |

## Success Criteria

- [ ] User can find any text element
- [ ] User can edit text content
- [ ] User can change text styling
- [ ] User understands multilingual considerations

## FREE Indicator

Add banner at top of each page:

```markdown
> **FREE** - All text changes are included at no extra cost
```

## Implementation Steps

1. Create `text-headlines/` directory
2. Write changing-text.md
3. Write text-styles.md
4. Write multilingual.md
5. Add screenshot placeholders
6. Add FREE banners
