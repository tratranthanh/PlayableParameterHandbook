# Difficulty & Balance

Adjust how challenging your playable ad is for users.

## Simple vs Complex Difficulty

| Simple (if in dashboard) | Complex (requires quote) |
|--------------------------|--------------------------|
| Timer duration | Enemy AI behavior |
| HP values | Spawn patterns/logic |
| Speed multipliers | Level generation |
| Damage numbers | Win/lose conditions |
| Basic counts | Game flow changes |

**Rule:** Simple numeric values in your dashboard can be changed. Difficulty that requires game logic changes needs development work.

---

## Simple Difficulty Parameters

If these appear in your dashboard, you can adjust them:

| Parameter | What It Does |
|-----------|--------------|
| Timer | Shorter = harder, longer = easier |
| Player HP | Lower = harder, higher = easier |
| Enemy HP | Higher = harder, lower = easier |
| Speed | Faster = harder, slower = easier |
| Damage | Higher = harder/easier depending on source |

---

## Complex Difficulty (Requires Quote)

These require game logic implementation:

| Change | Why It's Complex |
|--------|------------------|
| Smarter enemy AI | Requires behavior code |
| Dynamic spawn patterns | Requires spawn system changes |
| Procedural levels | Requires level generation code |
| New win/lose conditions | Requires game flow changes |
| Adaptive difficulty | Requires player tracking logic |

---

## Difficulty Guidelines for Playable Ads

| Goal | Recommendation |
|------|----------------|
| Show gameplay | Medium difficulty |
| Quick engagement | Easier start |
| Drive downloads | Beatable but engaging |

Most successful playable ads are slightly easier than the full game.

---

## Testing Your Changes

After adjusting difficulty:

1. Play through the entire ad
2. Check if it's completable
3. Verify it's still engaging

---

## Related

* [Timing & Speed](timing.md) — Timer adjustments
* [Gameplay Values](values.md) — Point values
* [Pricing](../help/pricing.md) — What requires a quote
