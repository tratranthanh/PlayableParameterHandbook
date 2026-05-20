# Config Layer Parameters

**Config Layer parameters are included if they exist in your dashboard.** These control gameplay values — how the game plays, not how it looks. Config layer changes require approval before implementation.

<figure><img src="../.gitbook/assets/config-layer-overview.png" alt="Config Layer Overview"><figcaption>Config Layer controls gameplay values — HP, timers, speed, toggles</figcaption></figure>

---

## What is the Config Layer?

The Config Layer controls **gameplay values** — health, damage, timing, speed, counts, toggles. Unlike UI Layer (auto-applied), Config Layer parameters affect gameplay balance and require human approval before implementation.

| Category | What It Controls | Examples |
|----------|------------------|----------|
| **Health** | HP values | `playerHP`, `enemyHP`, `bossHP` |
| **Damage** | Attack values | `damage`, `playerDamage`, `enemyDamage` |
| **Timing** | Duration values | `timerDuration`, `cooldown`, `delay`, `spawnInterval` |
| **Speed** | Movement values | `speedMultiplier`, `playerSpeed`, `enemySpeed` |
| **Counts** | Quantities | `spawnCount`, `maxBullets`, `livesCount`, `attemptLimit` |
| **Multipliers** | Scaling values | `scoreMultiplier`, `damageMultiplier` |
| **Toggles** | Feature flags | `showTutorial`, `enableSound`, `showHPBar` |

---

## NumberParameter

Numeric values for gameplay mechanics.

<figure><img src="../.gitbook/assets/number-parameter-dashboard.png" alt="NumberParameter in Dashboard"><figcaption>NumberParameter: number input field with optional min/max/step</figcaption></figure>

### Properties

| Property | Type | Description |
|----------|------|-------------|
| `value` | Number | The numeric value |
| `min` | Number | Minimum allowed (optional) |
| `max` | Number | Maximum allowed (optional) |
| `step` | Number | Increment step (optional) |

### Common Uses

| Category | Parameters |
|----------|------------|
| **Health** | `playerHP`, `enemyHP`, `bossHP` |
| **Damage** | `damage`, `playerDamage`, `enemyDamage` |
| **Timing** | `timerDuration`, `cooldown`, `delay`, `spawnInterval` |
| **Speed** | `speedMultiplier`, `playerSpeed`, `enemySpeed`, `projectileSpeed` |
| **Counts** | `spawnCount`, `maxBullets`, `livesCount`, `attemptLimit` |
| **Multipliers** | `scoreMultiplier`, `damageMultiplier` |

### Example Values

| Parameter | Typical Range | Unit |
|-----------|---------------|------|
| `timerDuration` | 15-60 | seconds |
| `playerHP` | 50-200 | points |
| `damage` | 10-50 | points |
| `speedMultiplier` | 0.5-2.0 | multiplier |
| `spawnCount` | 1-10 | count |

---

## BooleanParameter

True/false toggles for features.

<figure><img src="../.gitbook/assets/boolean-parameter-dashboard.png" alt="BooleanParameter in Dashboard"><figcaption>BooleanParameter: on/off toggle switch</figcaption></figure>

### Properties

| Property | Type | Description |
|----------|------|-------------|
| `value` | Boolean | `true` or `false` |

### Common Uses

| Parameter | Default | What It Controls |
|-----------|---------|------------------|
| `showTutorial` | `true` | Display tutorial overlay |
| `showTimer` | `true` | Display countdown |
| `showScore` | `true` | Display points |
| `showHPBar` | `true` | Display health bar |
| `enableSound` | `true` | Play audio |
| `enableHaptics` | `false` | Vibration feedback |
| `enablePowerUps` | `true` | Power-ups spawn |

---

## RangeParameter

Numeric values with defined min/max bounds. Displayed as sliders in the dashboard.

<figure><img src="../.gitbook/assets/range-parameter-dashboard.png" alt="RangeParameter in Dashboard"><figcaption>RangeParameter: slider with min/max bounds and current value</figcaption></figure>

### Properties

| Property | Type | Description |
|----------|------|-------------|
| `value` | Number | Current value |
| `min` | Number | Minimum value |
| `max` | Number | Maximum value |
| `step` | Number | Increment step |

### Common Uses

| Parameter | Min | Max | Default |
|-----------|-----|-----|---------|
| `difficulty` | 1 | 10 | 5 |
| `volume` | 0 | 100 | 80 |
| `speedMultiplier` | 0.5 | 2.0 | 1.0 |
| `sensitivityX` | 0.1 | 3.0 | 1.0 |

---

## SelectParameter

Dropdown selection from predefined options.

<figure><img src="../.gitbook/assets/select-parameter-dashboard.png" alt="SelectParameter in Dashboard"><figcaption>SelectParameter: dropdown with predefined options (Easy/Medium/Hard)</figcaption></figure>

### Properties

| Property | Type | Description |
|----------|------|-------------|
| `value` | String | Selected option key |
| `options` | Array | Available choices |

### Example

```
options: ["easy", "medium", "hard"]
value: "medium"
```

### Common Uses

| Parameter | Options |
|-----------|---------|
| `difficultyPreset` | Easy, Medium, Hard |
| `theme` | Light, Dark |
| `language` | EN, ES, FR, DE, etc. |

---

## AudioParameter

Audio asset references.

### Properties

| Property | Type | Description |
|----------|------|-------------|
| `audioClip` | Asset | Audio file reference |
| `volume` | Number | Playback volume 0-1 |

### Supported Formats

| Format | Notes |
|--------|-------|
| MP3 | Widely supported, compressed |
| OGG | Good compression, web-friendly |
| WAV | Uncompressed, larger files |

---

## What's Included vs Custom Development

### ✅ Included

If the parameter **exists in your dashboard**, you can change it:

- Adjust timer from 30s to 45s
- Increase player HP from 100 to 150
- Reduce enemy count from 5 to 3
- Toggle tutorial on/off
- Change difficulty preset

### 🔧 Custom Development Required

If the parameter **doesn't exist** in your dashboard:

- New game mechanics
- New AI behaviors
- New spawn patterns
- New win/lose conditions
- Adding parameters that aren't wired

**Rule:** If you don't see it, it doesn't exist in your build yet.

---

## Related

- [UI Layer](ui-layer.md) — Visual parameters (always included)
- [Custom Development](../help/custom-development.md) — Request new features
