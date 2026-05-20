# Difficulty & Balance

Adjust how challenging your playable ad is for users.

---

## Two Types of Parameters

| Layer | What It Controls | How to Change |
|-------|------------------|---------------|
| **UI Layer** | How difficulty *looks* (HP bar color, timer style) | Always adjustable |
| **Config Layer** | How difficulty *plays* (HP values, timer duration) | If parameter exists in dashboard |

---

## Config Layer Parameters (Gameplay Values)

If these parameters appear in your dashboard, you can adjust them:

### NumberParameter — Health & Damage

| Parameter | Type | What It Does | Difficulty Impact |
|-----------|------|--------------|-------------------|
| `playerHP` | `NumberParameter` | Player health points | Lower = harder |
| `enemyHP` | `NumberParameter` | Enemy health points | Higher = harder |
| `damage` | `NumberParameter` | Attack damage | Context-dependent |
| `playerDamage` | `NumberParameter` | Damage player deals | Lower = harder |
| `enemyDamage` | `NumberParameter` | Damage enemies deal | Higher = harder |

### NumberParameter — Timing

| Parameter | Type | What It Does | Difficulty Impact |
|-----------|------|--------------|-------------------|
| `timerDuration` | `NumberParameter` | Countdown time (seconds) | Shorter = harder |
| `cooldown` | `NumberParameter` | Wait between actions | Longer = harder |
| `spawnInterval` | `NumberParameter` | Time between spawns | Shorter = harder |
| `delayStart` | `NumberParameter` | Initial delay | Shorter = harder |

### NumberParameter — Speed & Movement

| Parameter | Type | What It Does | Difficulty Impact |
|-----------|------|--------------|-------------------|
| `speedMultiplier` | `NumberParameter` | Overall game speed | Faster = harder |
| `playerSpeed` | `NumberParameter` | Player movement | Lower = harder |
| `enemySpeed` | `NumberParameter` | Enemy movement | Higher = harder |
| `projectileSpeed` | `NumberParameter` | Bullet/object speed | Higher = harder |

### NumberParameter — Counts

| Parameter | Type | What It Does | Difficulty Impact |
|-----------|------|--------------|-------------------|
| `spawnCount` | `NumberParameter` | Enemies per wave | Higher = harder |
| `attemptLimit` | `NumberParameter` | Max retries | Lower = harder |
| `maxBullets` | `NumberParameter` | Ammo capacity | Lower = harder |
| `livesCount` | `NumberParameter` | Player lives | Lower = harder |

### RangeParameter — Sliders

| Parameter | Type | Range | Difficulty Impact |
|-----------|------|-------|-------------------|
| `difficulty` | `RangeParameter` | 1-10 | Higher = harder |
| `difficultyPreset` | `SelectParameter` | Easy/Medium/Hard | Selection-based |

### BooleanParameter — Toggles

| Parameter | Type | What It Does |
|-----------|------|--------------|
| `enablePowerUps` | `BooleanParameter` | Power-ups available |
| `enableTutorial` | `BooleanParameter` | Show tutorial first |
| `enableTimer` | `BooleanParameter` | Use countdown timer |

---

## UI Layer Parameters (Visual Styling)

These control how difficulty-related UI *looks*, not how it *works*:

| Element | Parameter Type | Changeable Properties |
|---------|---------------|----------------------|
| HP Bar | `SpriteParameter` | `spriteColor`, `position`, `scale` |
| Timer Text | `LabelParameter` | `labelColor`, `fontSize`, `outline` |
| Timer Warning | `ColorParameter` | Color when time is low |
| Lives Display | `SpriteParameter` | `spriteFrame`, `spriteColor` |

---

## What's Included vs Custom Development

### ✅ Included (Config Layer — Existing Parameters)

| You Can | Example |
|---------|---------|
| Change timer from 30s to 45s | `timerDuration: 45` |
| Increase player HP from 100 to 150 | `playerHP: 150` |
| Reduce enemy count from 5 to 3 | `spawnCount: 3` |
| Slow down game speed | `speedMultiplier: 0.8` |
| Increase damage dealt | `playerDamage: 30` |

**Requirement:** Parameter must exist in your dashboard.

### 🔧 Custom Development Required

| Request | What's Involved |
|---------|-----------------|
| Smarter enemy AI | Behavior code changes |
| Dynamic difficulty scaling | Player tracking logic |
| New spawn patterns | Spawn system changes |
| Procedural level generation | Level generation code |
| New win/lose conditions | Game flow changes |
| Adaptive difficulty | Real-time adjustment logic |

**Requirement:** [Request a quote](../help/custom-development.md)

---

## Difficulty Guidelines for Playable Ads

| Goal | Recommendation |
|------|----------------|
| Show gameplay | Medium difficulty |
| Quick engagement | Easier start |
| Drive downloads | Beatable but engaging |
| Build frustration (retry-focused) | Slightly harder |

### The Sweet Spot

Most successful playable ads are **slightly easier** than the full game:

| Too Easy | Just Right | Too Hard |
|----------|------------|----------|
| No challenge | Engaging | Frustrating |
| Boring | Achievable | Rage-quit |
| Low replay | "I want more" | Won't retry |

---

## Testing Your Changes

After adjusting difficulty:

1. **Play through completely** — Can you finish?
2. **Time yourself** — Does it fit the ad duration?
3. **Check engagement** — Is it fun or frustrating?
4. **Test failure state** — Does lose screen appear correctly?
5. **Verify values** — Do numbers display correctly in UI?

---

## Related

- [Timing & Speed](timing.md) — Timer adjustments
- [Gameplay Values](values.md) — Scores and multipliers
- [Game UI Elements](ui-elements.md) — HP bar and timer styling
- [Custom Development](../help/custom-development.md) — Request new features
