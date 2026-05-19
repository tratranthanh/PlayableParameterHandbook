# Phase 9: Custom Development

**Priority:** P2
**Status:** Pending
**Effort:** S (~1 day)

## Overview

Document what custom development means, when it's needed, and how to request a quote for features that require manual implementation.

## Pricing Model Context

| Category | Pricing | Examples |
|----------|---------|----------|
| Auto-scanned UI | FREE | All dashboard-visible changes |
| Auto-detected config | FREE | Difficulty, timing, toggles |
| Custom development | Quote | New features, mechanics, integrations |

## Files to Create

```
docs/handbook/custom-development/
  what-is-custom.md
  request-quote.md
  examples.md
```

## Content Outline

### what-is-custom.md
- What counts as "custom"
- Why some things need development
- Free vs paid comparison
- Screenshot: Conceptual diagram

### request-quote.md
- How to request custom work
- What to include in your request
- Timeline expectations
- Contact information
- Screenshot: Request form (if applicable)

### examples.md
- Common custom requests
- Example: New game mechanic
- Example: SDK integration
- Example: Server-side features
- Example: Custom animations

## Content for what-is-custom.md

```markdown
## What is Custom Development?

Custom development is work that goes beyond the dashboard's built-in 
customization options. It requires our engineering team to write new code.

### The Simple Rule

**If you see it in the dashboard = FREE**
**If it doesn't exist yet = Custom (quote required)**

### Examples

| FREE (Dashboard) | Custom (Quote) |
|------------------|----------------|
| Change button color | Add a new button |
| Edit existing text | Add new text elements |
| Replace existing images | Add new visual effects |
| Adjust timer duration | Add a new timer feature |
| Change HP bar colors | Add new health mechanics |

### Why the Difference?

When you make changes in the dashboard, you're adjusting values that our 
system already knows about. Custom development means creating something 
entirely new, which requires:

- Design planning
- Code development
- Quality testing
- Integration work
```

## Custom Request Template

```markdown
## How to Request Custom Development

1. **Describe what you want**
   - What should happen?
   - When should it appear?
   - How should it look?

2. **Explain why you need it**
   - What goal does it achieve?
   - Why can't dashboard options work?

3. **Share reference examples**
   - Screenshots or videos of similar features
   - Links to ads with this feature

4. **Timeline**
   - When do you need this?
   - Is there flexibility?

**Send your request to:** [contact email/form]
```

## Screenshot Placeholders

| Screenshot | Description |
|------------|-------------|
| `free-vs-custom-diagram.png` | Visual comparison |
| `custom-request-form.png` | Request form (if exists) |
| `custom-example-mechanic.png` | Example: new mechanic |
| `custom-example-effect.png` | Example: new effect |

## Success Criteria

- [ ] User understands free vs custom
- [ ] User knows how to request quotes
- [ ] User has examples for reference
- [ ] Contact process is clear

## Tone Guidance

```markdown
### Important: Keep It Positive

Don't make custom development sound restrictive. Frame it as:
- "Anything is possible!"
- "We can build exactly what you need"
- "The dashboard covers most needs, but we can go further"

NOT:
- "This requires extra payment"
- "Dashboard limitations"
- "Not included"
```

## Implementation Steps

1. Create `custom-development/` directory
2. Write what-is-custom.md
3. Write request-quote.md
4. Write examples.md
5. Add screenshot placeholders
6. Ensure positive framing
