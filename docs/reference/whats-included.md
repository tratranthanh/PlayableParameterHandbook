# Composite Parameters

Composite parameters bundle multiple ComponentParameters into a single configurable unit using `ObjectParameter<T>`. These control entire screens or complex UI elements and are included in your dashboard.

<figure><img src="../.gitbook/assets/composite-overview.png" alt="Composite Parameters Overview"><figcaption>Composites bundle Sprite + Label + Button into screen-level parameters</figcaption></figure>

{% hint style="info" %}
**Architecture Rule:** Composites use flat structure with typed child fields. Never nest `ObjectParameter` inside `ObjectParameter`.
{% endhint %}

---

## EndCardParameter

Controls the entire end card screen (win/lose). Defined in `PlayableParamterTool/parameter/composite/EndCardParameter.ts`.

<figure><img src="../.gitbook/assets/endcard-parameter-anatomy.png" alt="EndCardParameter Anatomy"><figcaption>EndCardParameter: Background (Sprite) + Title (Label) + Subtitle (Label) + CTA (Button)</figcaption></figure>

### Components

| Component | Type | All Properties Included |
|-----------|------|-------------------------|
| Background | `SpriteParameter` | `enable`, `position`, `contentSize`, `scale`, `spriteFrame`, `spriteColor` |
| Title | `LabelParameter` | `enable`, `position`, `string`, `labelColor`, `fontSize`, `lineHeight`, `isBold`, `isItalic`, `outlineColor`, `outlineWidth`, `shadowColor`, `shadowOffset` |
| Subtitle | `LabelParameter` | `enable`, `position`, `string`, `labelColor`, `fontSize` |
| CTA Button | `ButtonParameter` | All SpriteParameter fields + `labelString`, `labelColor`, `labelFontSize`, `labelBold`, `labelOutlineColor`, `labelOutlineWidth` |

### Config Interface

```typescript
interface EndCardConfig {
    background: SpriteParameterValues;
    title: LabelParameterValues;
    subtitle: LabelParameterValues;
    ctaButton: ButtonParameterValues;
}
```

### Example Configuration

| Component | Property | Value |
|-----------|----------|-------|
| Background | `spriteFrame` | `"win-bg.png"` |
| Background | `spriteColor` | `#000000` (darken overlay) |
| Title | `string` | `"You Won!"` |
| Title | `labelColor` | `#FFFFFF` |
| Title | `fontSize` | `72` |
| Title | `outlineWidth` | `4` |
| Subtitle | `string` | `"Play the full game"` |
| Subtitle | `labelColor` | `#CCCCCC` |
| CTA Button | `labelString` | `"Download Now"` |
| CTA Button | `spriteColor` | `#4CAF50` |
| CTA Button | `labelColor` | `#FFFFFF` |

---

## LoadingScreenParameter

Controls the loading screen appearance. Defined in `PlayableParamterTool/parameter/composite/LoadingScreenParameter.ts`.

<figure><img src="../.gitbook/assets/loadingscreen-parameter-anatomy.png" alt="LoadingScreenParameter Anatomy"><figcaption>LoadingScreenParameter: Background (Color) + Icon (Sprite) + Game Name (Label)</figcaption></figure>

### Components

| Component | Type | All Properties Included |
|-----------|------|-------------------------|
| Background | `ColorParameter` | Solid color value `#RRGGBB` |
| Icon | `SpriteParameter` | `enable`, `position`, `contentSize`, `scale`, `spriteFrame`, `spriteColor` |
| Game Name | `LabelParameter` | `enable`, `position`, `string`, `labelColor`, `fontSize`, `lineHeight`, `outlineColor`, `outlineWidth` |

### Config Interface

```typescript
interface LoadingScreenConfig {
    backgroundColor: ColorParameterValues;
    icon: SpriteParameterValues;
    gameName: LabelParameterValues;
}
```

### Example Configuration

| Component | Property | Value |
|-----------|----------|-------|
| Background | color | `#1A1A2E` |
| Icon | `spriteFrame` | `"spinner.png"` |
| Icon | `spriteColor` | `#FFFFFF` |
| Game Name | `string` | `"My Game"` |
| Game Name | `labelColor` | `#FFFFFF` |
| Game Name | `fontSize` | `48` |

---

## TutorialHandParameter

Controls the animated tutorial hand indicator. Defined in `PlayableParamterTool/parameter/composite/TutorialHandParameter.ts`.

<figure><img src="../.gitbook/assets/tutorialhand-parameter-anatomy.png" alt="TutorialHandParameter Anatomy"><figcaption>TutorialHandParameter: Hand (Sprite) + Animation Preset</figcaption></figure>

### Components

| Component | Type | All Properties Included |
|-----------|------|-------------------------|
| Hand | `SpriteParameter` | `enable`, `position`, `contentSize`, `scale`, `spriteFrame`, `spriteColor` |
| Animation | `AnimationPresetParameter` | Preset selection from catalog |

### Config Interface

```typescript
interface TutorialHandConfig {
    sprite: SpriteParameterValues;
    animation: AnimationPresetConfig;
}
```

### Animation Presets

| Category | Presets |
|----------|---------|
| **Interactive** | `tap`, `press`, `swipe`, `drag` |
| **Entrance** | `fadeIn`, `scaleUp`, `slideIn`, `bounceIn`, `pop` |
| **Emphasis** | `pulse`, `shake`, `bounce`, `wiggle`, `glow`, `heartbeat` |

---

## RichTextParameter

Text with entrance and exit animations. Defined in `PlayableParamterTool/parameter/composite/RichTextParameter.ts`.

### Components

| Component | Type | All Properties Included |
|-----------|------|-------------------------|
| Label | `LabelParameter` | `enable`, `position`, `string`, `labelColor`, `fontSize`, `lineHeight`, `isBold`, `isItalic`, `outlineColor`, `outlineWidth`, `shadowColor`, `shadowOffset` |
| Entrance | `AnimationPresetParameter` | Animation when appearing |
| Exit | `AnimationPresetParameter` | Animation when disappearing |
| Auto Hide | `BooleanParameter` | Hide after duration |
| Auto Hide Delay | `NumberParameter` | Display time (seconds) |

### Config Interface

```typescript
interface RichTextConfig {
    label: LabelParameterValues;
    entrance: AnimationPresetConfig;
    exit: AnimationPresetConfig;
    autoHide: boolean;
    autoHideDelay: number;
}
```

### Animation Presets

| Category | Options |
|----------|---------|
| **Entrance** | `fadeIn`, `scaleUp`, `slideInLeft`, `slideInRight`, `slideInTop`, `slideInBottom`, `bounceIn`, `pop` |
| **Exit** | `fadeOut`, `scaleDown`, `slideOutLeft`, `slideOutRight`, `slideOutTop`, `slideOutBottom`, `shrink` |

---

## AnimationPresetParameter

Standalone animation preset selection. Used within composites for entrance, exit, and emphasis animations.

### Available Presets

| Category | Presets |
|----------|---------|
| **Entrance** | `fadeIn`, `scaleUp`, `slideInLeft`, `slideInRight`, `slideInTop`, `slideInBottom`, `bounceIn`, `pop` |
| **Emphasis** | `pulse`, `shake`, `bounce`, `wiggle`, `glow`, `heartbeat` |
| **Exit** | `fadeOut`, `scaleDown`, `slideOutLeft`, `slideOutRight`, `slideOutTop`, `slideOutBottom`, `shrink` |
| **Interactive** | `tap`, `press`, `swipe`, `drag` |

---

## RedirectParameter

Controls store redirect behavior (standalone, not a composite).

### Properties

| Property | Type | Description |
|----------|------|-------------|
| `active` | `BooleanParameter` | Enable redirect |
| `count` | `NumberParameter` | Redirect after N interactions |

---

## NodePreset Catalog

Pre-built presets for common UI patterns. These are auto-detected during Canvas scan and composed from ComponentParameters.

| Preset | Components | Use Case |
|--------|------------|----------|
| **Button** | Node + UITransform + Sprite + Label + Button + UIOpacity | CTA buttons |
| **Image** | Node + UITransform + Sprite + UIOpacity | Backgrounds, icons |
| **Text** | Node + UITransform + Label + UIOpacity | Titles, descriptions |
| **Slider** | Node + UITransform + Sprite + Slider + UIOpacity | Settings sliders |
| **Toggle** | Node + UITransform + Sprite + Toggle + UIOpacity | Checkboxes |
| **CurrencyUI** | Node(root) + Node(icon) + Label(counter) | Currency displays (coins, gems) |
| **HPBar** | Node(root) + Sprite(bg) + Sprite(fill) + Label(text)? | Health/progress bars |
| **Countdown** | Node(root) + Label(prep) + Label(number) | Countdown timers |
| **IconLabel** | Node(root) + Sprite(icon) + Label(text) | Icon + text combos |

### CurrencyUI Preset Example

```typescript
export class CurrencyUIParameter {
    rootNode: UINodeParameter;
    icon: SpriteParameter;
    counter: LabelParameter;
}
```

### HPBar Preset Example

```typescript
export class HPBarUIParameter {
    rootNode: UINodeParameter;
    background: SpriteParameter;
    fill: SpriteParameter;
    text?: LabelParameter;  // optional
}
```

---

## Creating Custom Composites

Custom composites are defined in `scripts/parameter/config/CustomParameter.ts` using flat `ObjectParameter<T>` structure:

```typescript
export class MyScreenParameter extends ObjectParameter<{
  background: SpriteParameter;
  title: LabelParameter;
  button: ButtonParameter;
}> {
  // Flat structure — no nested ObjectParameter
}
```

{% hint style="warning" %}
**Never modify `PlayableParamterTool/`** (submodule) for project-specific types. All custom composites go in `CustomParameter.ts`.
{% endhint %}

Custom composites require development. See [Custom Development](../help/custom-development.md).

---

## Related

- [UI Layer](ui-layer.md) — ComponentParameters (auto-applied)
- [Config Layer](config-layer.md) — Gameplay values (requires approval)
- [End Cards](../screens/end-cards.md) — Using EndCardParameter
- [Loading Screen](../screens/loading.md) — Using LoadingScreenParameter
