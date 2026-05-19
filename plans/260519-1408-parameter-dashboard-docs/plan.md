# Parameter Dashboard Handbook — Documentation Plan

**Created:** 2026-05-19 14:08
**Status:** Complete
**Audience:** Ad Network Clients (non-technical)

## Overview

Create user-friendly GitBook documentation for the Parameter Dashboard, explaining what clients can customize and the pricing model.

## Key Decisions

| Decision | Choice |
|----------|--------|
| Audience | Non-technical ad network clients |
| Tone | Action-oriented, jargon-free |
| Pricing Model | Auto-scanned = FREE, Custom dev = quote |
| Visual Aid | Dashboard screenshots at each section |
| Structure | Use-case based (not technical categories) |

## Phase Summary

| Phase | Description | Status | Effort |
|-------|-------------|--------|--------|
| Phase 1 | Getting Started | Complete | S |
| Phase 2 | Text & Headlines | Complete | S |
| Phase 3 | Images & Visuals | Complete | S |
| Phase 4 | Colors & Branding | Complete | S |
| Phase 5 | Interactive Elements | Complete | S |
| Phase 6 | Game UI Elements | Complete | M |
| Phase 7 | Game Settings | Complete | S |
| Phase 8 | Screens & Views | Complete | M |
| Phase 9 | Custom Development | Complete | S |
| Phase 10 | FAQ & Support | Complete | S |

**Total Effort:** ~3 days

## Content Structure

```
docs/
  handbook/
    SUMMARY.md              # GitBook navigation
    README.md               # Introduction
    getting-started/
      what-is-dashboard.md
      accessing-dashboard.md
      quick-start.md
    text-headlines/
      changing-text.md
      text-styles.md
      multilingual.md
    images-visuals/
      replacing-images.md
      logos-icons.md
      backgrounds.md
    colors-branding/
      brand-colors.md
      ui-colors.md
      gradients-effects.md
    interactive-elements/
      buttons.md
      toggles-switches.md
      sliders.md
    game-ui/
      hp-bars.md
      timers.md
      score-displays.md
      currency.md
    game-settings/
      difficulty.md
      timing-speed.md
      gameplay-values.md
    screens-views/
      loading-screen.md
      tutorial.md
      end-cards.md
    custom-development/
      what-is-custom.md
      request-quote.md
      examples.md
    faq/
      common-questions.md
      troubleshooting.md
      contact.md
```

## Technical Alignment

Maps to `t1k-cocos-cocos-base-playable-parameter` skill:

| Documentation Section | Parameter Type | Layer |
|-----------------------|----------------|-------|
| Text & Headlines | LabelParameter | UI (auto) |
| Images & Visuals | SpriteParameter | UI (auto) |
| Colors & Branding | ColorParameter | UI (auto) |
| Interactive Elements | ButtonParameter, ToggleParameter | UI (auto) |
| Game UI Elements | Custom Composites (HPBar, Timer, etc.) | UI (auto) |
| Game Settings | NumberParameter, BooleanParameter | Config (approval) |
| Screens & Views | EndCardParameter, LoadingScreenParameter | UI (auto) |
| Custom Development | N/A (manual implementation) | Paid |

## Next Steps

1. Create `docs/handbook/` directory structure
2. Write SUMMARY.md (GitBook navigation)
3. Implement each phase sequentially
4. Add screenshot placeholders
5. Review for jargon-free language

## Risk Assessment

| Risk | Likelihood (1-5) | Impact (1-5) | Score | Mitigation |
|------|-----------------|--------------|-------|------------|
| Screenshots unavailable | 3 | 3 | 9 | Use placeholder markup, add actual screenshots later |
| Jargon creep | 2 | 4 | 8 | Peer review each section for plain language |
| Missing dashboard features | 2 | 3 | 6 | Cross-reference with actual dashboard before finalizing |
| Pricing model changes | 1 | 4 | 4 | Document version date, note subject to change |

## Timeline

| Phase | Effort | Dependencies |
|-------|--------|-------------|
| Phase 1: Getting Started | S (1d) | None - foundation |
| Phase 2: Text & Headlines | S (1d) | Phase 1 |
| Phase 3: Images & Visuals | S (1d) | Phase 1 |
| Phase 4: Colors & Branding | S (1d) | Phase 1 |
| Phase 5: Interactive Elements | S (1d) | Phase 1 |
| Phase 6: Game UI Elements | M (3d) | Phases 2-5 (builds on concepts) |
| Phase 7: Game Settings | S (1d) | Phase 6 |
| Phase 8: Screens & Views | M (3d) | Phases 2-5 |
| Phase 9: Custom Development | S (1d) | Phase 1 |
| Phase 10: FAQ & Support | S (1d) | All phases complete |
| **Total** | **~14 days** | Critical path: 1 → 2-5 → 6 → 10 |

**Parallel opportunities:** Phases 2-5 can be written in parallel. Phases 6-8 can overlap.

## Content Principles (from Brainstorm)

| Principle | Implementation |
|-----------|----------------|
| No jargon | "Change text" not "Modify LabelParameter" |
| Action-oriented | "How to replace your logo" not "Image parameters" |
| Visual learning | Dashboard screenshots for each section |
| Clear free/paid | "Everything you see = free" |
| Simple request flow | Contact for custom work |

## References

- Brainstorm report: `plans/reports/brainstorm-260519-1145-parameter-dashboard-docs.md`
- Technical skill: `t1k-cocos-cocos-base-playable-parameter`
- Composite types: `t1k-cocos-cocos-base-playable-parameter-composite`

## Cook Handoff

After plan approval:
```
/t1k:cook plans/260519-1408-parameter-dashboard-docs/
```
