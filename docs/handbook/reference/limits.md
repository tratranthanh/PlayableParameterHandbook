# Limits & Constraints

Reference for character limits, file sizes, and other constraints.

## Text Limits

| Element | Character Limit | Recommendation |
|---------|-----------------|----------------|
| Headlines | 30-50 | Keep under 30 |
| Button labels | 15-25 | Keep under 15 |
| Short instructions | 100 | Keep under 50 |
| Tutorial text | 50 | 3-5 words ideal |
| Win/Lose titles | 30 | Keep punchy |
| Subtitles | 50 | One short sentence |
| Long descriptions | 200+ | Rare use case |

## File Size Limits

| Asset Type | Maximum | Recommended |
|------------|---------|-------------|
| Logo | 500 KB | Under 200 KB |
| Background | 2 MB | Under 1 MB |
| App Icon | 300 KB | Under 100 KB |
| UI Icons | 150 KB | Under 50 KB |
| Currency Icons | 100 KB | Under 30 KB |

## Image Dimensions

| Asset Type | Minimum | Maximum | Recommended |
|------------|---------|---------|-------------|
| Logo | 256x256 | 1024x1024 | 512x512 |
| Background (Portrait) | 720x1280 | 2160x3840 | 1080x1920 |
| Background (Landscape) | 1280x720 | 3840x2160 | 1920x1080 |
| App Icon | 128x128 | 512x512 | 256x256 |
| UI Icons | 32x32 | 256x256 | 64-128 |

## Gameplay Value Ranges

These vary by game. Check your dashboard for exact ranges.

| Value Type | Typical Range | Notes |
|------------|---------------|-------|
| Difficulty | 1-10 | Higher = harder |
| Timer | 15-120 seconds | 30-45 optimal |
| HP values | 1-1000 | Game-dependent |
| Speed multiplier | 0.5-2.0 | 1.0 = normal |
| Point values | 1-10000 | Per action |

## Color Constraints

| Format | Valid | Invalid |
|--------|-------|---------|
| 6-digit hex | #FF5722 | FF5722 (no #) |
| 8-digit hex | #FF572280 | #FF57 (too short) |
| RGB format | Not supported | rgb(255,87,34) |
| Named colors | Not supported | "orange" |

## Supported Languages

Text fields support these character sets:

| Language Group | Examples | Support |
|----------------|----------|---------|
| Latin | English, Spanish, French | Full |
| Cyrillic | Russian, Ukrainian | Full |
| CJK | Chinese, Japanese, Korean | Full |
| Arabic | Arabic, Hebrew | Partial |
| Devanagari | Hindi | Partial |

### Right-to-Left (RTL) Languages

RTL support varies by element. Contact support for RTL requirements.

## Screen Orientations

| Orientation | Supported | Notes |
|-------------|-----------|-------|
| Portrait | Yes | Most common |
| Landscape | Yes | Game-dependent |
| Both | Some games | Responsive layout |

## Performance Considerations

| Factor | Limit | Impact |
|--------|-------|--------|
| Total image size | ~5 MB | Load time |
| Number of images | ~20 | Memory usage |
| Animation frames | Game-dependent | Performance |

## What Happens at Limits?

| Limit Type | Behavior |
|------------|----------|
| Text too long | Warning shown, text truncated |
| File too large | Upload rejected |
| Image too small | Warning shown, may look blurry |
| Invalid color | Reverts to previous value |
| Value out of range | Clamped to nearest valid value |

## Tips for Staying Within Limits

### Text
* Use abbreviations: "Download" → "Get"
* Remove filler words: "Click here to" → just the action
* Use action words: Short verbs work best

### Images
* Compress before uploading
* Use appropriate format (PNG/JPG)
* Crop to exact dimensions needed

### Values
* Start with defaults
* Make incremental changes
* Test after each adjustment

## Related

* [All Parameters](all-parameters.md) - Parameter reference
* [File Formats](file-formats.md) - Format specifications
