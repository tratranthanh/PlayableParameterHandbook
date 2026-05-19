# Phase 1: Getting Started

**Priority:** P0 (Foundation)
**Status:** Pending
**Effort:** S (~1 day)

## Overview

Create the introduction and onboarding section that helps users understand what the Parameter Dashboard is and how to access it.

## Context Links

- Brainstorm: `plans/reports/brainstorm-260519-1145-parameter-dashboard-docs.md`

## Requirements

### Functional
- Explain what the Parameter Dashboard is in plain language
- Provide login/access instructions
- Include a "Quick Start" for first-time users
- Establish the "free vs paid" concept early

### Non-Functional
- Zero technical jargon
- Under 500 words per page
- Mobile-friendly reading

## Files to Create

```
docs/handbook/
  README.md
  SUMMARY.md
  getting-started/
    what-is-dashboard.md
    accessing-dashboard.md
    quick-start.md
```

## Content Outline

### README.md (Introduction)
- Welcome message
- What this handbook covers
- Who this is for
- Quick navigation to common tasks

### SUMMARY.md (GitBook Navigation)
- Full table of contents with nested structure

### what-is-dashboard.md
- Plain language explanation
- Screenshot: Dashboard overview
- Key concept: "If you see it in the dashboard, you can change it for free"

### accessing-dashboard.md
- How to get login credentials
- URL/link to dashboard
- Screenshot: Login screen

### quick-start.md
- 3-step guide: "Your First Change"
- Step 1: Find a text element
- Step 2: Edit the text
- Step 3: Preview your change
- Screenshot: Before/after comparison

## Screenshot Placeholders

| Screenshot | Description | Location |
|------------|-------------|----------|
| `dashboard-overview.png` | Full dashboard view | what-is-dashboard.md |
| `login-screen.png` | Login page | accessing-dashboard.md |
| `first-change-before.png` | Element before editing | quick-start.md |
| `first-change-after.png` | Element after editing | quick-start.md |

## Success Criteria

- [ ] User understands what the dashboard does
- [ ] User can log in and access dashboard
- [ ] User completes their first change
- [ ] Free/paid concept is clear

## Implementation Steps

1. Create `docs/handbook/` directory structure
2. Write SUMMARY.md with full navigation
3. Write README.md introduction
4. Write what-is-dashboard.md
5. Write accessing-dashboard.md
6. Write quick-start.md
7. Add screenshot placeholder markup

## Content Tone Guidelines

| Instead of | Write |
|------------|-------|
| "LabelParameter" | "text element" |
| "SpriteParameter" | "image" |
| "Configure properties" | "Make changes" |
| "Deploy changes" | "Save your changes" |
| "UI components" | "things you see on screen" |
