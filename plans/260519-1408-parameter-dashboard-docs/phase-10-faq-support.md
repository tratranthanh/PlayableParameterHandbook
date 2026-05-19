# Phase 10: FAQ & Support

**Priority:** P2
**Status:** Pending
**Effort:** S (~1 day)

## Overview

Create a comprehensive FAQ section addressing common questions, troubleshooting guides, and support contact information.

## Files to Create

```
docs/handbook/faq/
  common-questions.md
  troubleshooting.md
  contact.md
```

## Content Outline

### common-questions.md

**Pricing Questions:**
- "Is this really free?"
- "What costs extra?"
- "How do I get a quote?"

**Feature Questions:**
- "Can I change [X]?"
- "Why can't I edit some things?"
- "Will my changes go live immediately?"

**Technical Questions:**
- "What image formats are supported?"
- "What's the max file size?"
- "Can I undo changes?"

### troubleshooting.md

**Common Issues:**
- Image not uploading
- Changes not appearing
- Login problems
- Preview not loading

**Solutions format:**
```markdown
### Problem: [Issue]

**Symptoms:** What the user sees

**Solution:**
1. Step one
2. Step two
3. Step three

**Still not working?** Contact support (link)
```

### contact.md

- Support email
- Response time expectations
- What to include in support requests
- Emergency contact (if applicable)

## FAQ Content

```markdown
## Pricing & Costs

### Is customization really free?

**Yes!** Everything you can change in the dashboard is included at no 
extra cost. If you see a setting, you can change it for free.

### What requires a quote?

Only custom development work that isn't available in the dashboard. 
This includes new features, new game mechanics, or special integrations.

### How do quotes work?

1. Tell us what you need
2. We'll assess the work required
3. You receive a quote with timeline
4. You decide if you want to proceed

## Making Changes

### Will my changes go live immediately?

Most visual changes (colors, images, text) apply instantly to your preview.
Some gameplay changes may need a brief review before going live.

### Can I undo my changes?

Yes! The dashboard keeps your original settings. You can:
- Revert individual changes
- Reset to the original version

### Can I test before going live?

Absolutely! Always use the Preview feature to see your changes before 
making them live.

## Technical Questions

### What image formats work?

- **PNG** - Best for logos, icons, and images with transparency
- **JPG/JPEG** - Good for photos and backgrounds

### What's the maximum file size?

Images should be under 2MB. Larger files may slow down loading.

### What screen sizes are supported?

Your playable ad automatically adapts to different screen sizes. 
Design for standard mobile dimensions (1080x1920 portrait or 1920x1080 landscape).
```

## Screenshot Placeholders

| Screenshot | Description |
|------------|-------------|
| `preview-button.png` | How to preview |
| `revert-changes.png` | How to undo |
| `support-form.png` | Support contact form |

## Success Criteria

- [ ] Common questions answered
- [ ] Troubleshooting covers main issues
- [ ] Contact info is clear
- [ ] Tone is helpful and reassuring

## Implementation Steps

1. Create `faq/` directory
2. Write common-questions.md
3. Write troubleshooting.md
4. Write contact.md
5. Add screenshot placeholders
6. Review for completeness
