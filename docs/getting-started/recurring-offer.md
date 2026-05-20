# Recurring Offer (Redirect Parameter)

**The recurring offer triggers a store redirect during gameplay** — not just at the end card. It can be wired to any kind of trigger: UI taps, gameplay events, level completion, custom interactions.

<figure><img src="../.gitbook/assets/redirect-parameter-dashboard.png" alt="RedirectParameter Recurring Offer"><figcaption>RedirectParameter: enable recurring redirects, trigger after N interactions</figcaption></figure>

---

## Why Recurring Offers Matter

Ad networks reward playables that drive store visits **during** gameplay, not just at the end. The recurring offer captures users who don't reach the end card — typically 40-60% of impressions.

| Strategy | Store Visits | Conversion |
|----------|--------------|------------|
| End card only | ~30-40% of users | Lower |
| Recurring + End card | ~70-90% of users | Higher |

---

## RedirectParameter

Standalone parameter — not part of UI or Config layer specifically. It can be triggered by any parameter type.

### Properties

| Property | Type | Description |
|----------|------|-------------|
| `active` | BooleanParameter | Enable/disable the recurring redirect |
| `count` | NumberParameter | Number of interactions before redirecting (e.g., 3 = redirect on 3rd trigger) |

---

## What Can Trigger It

The recurring offer can hook into **any kind of parameter or event**:

| Trigger Type | Example |
|--------------|---------|
| **UI taps** | Tap any button → counts toward redirect |
| **Gameplay events** | Defeat enemy, complete level, collect item |
| **Time-based** | Every 10 seconds of gameplay |
| **Custom interactions** | Drag, swipe, drop, match |
| **Complex parameters** | After N successful actions |

---

## Common Configurations

| Use Case | Active | Count | Behavior |
|----------|--------|-------|----------|
| **Aggressive** | `true` | `1` | Redirect on every interaction |
| **Balanced (recommended)** | `true` | `3` | Redirect every 3 interactions |
| **Light touch** | `true` | `5` | Redirect every 5 interactions |
| **End card only** | `false` | — | Disable recurring (CTA at end only) |

---

## Implementation Note

The redirect parameter is **included in every build by default**. The trigger logic (what counts as an "interaction") is defined per-playable based on its game type:

- **Match-3:** Each match counts
- **Shooter:** Each shot fired
- **Puzzle:** Each piece placed
- **Runner:** Each obstacle passed

Custom trigger logic requires development. See [Custom Development](../help/custom-development.md).

---

## Related

- [UI Layer](ui-layer.md) — Visual parameters
- [Config Layer](config-layer.md) — Gameplay values
- [End Cards](../screens/end-cards.md) — End card CTA configuration
- [Custom Development](../help/custom-development.md) — Custom trigger logic
