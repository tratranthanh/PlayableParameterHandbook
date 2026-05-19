# File Formats

Supported file formats for images, logos, and other assets.

## Image Formats

| Format | Extension | Best For | Transparency |
|--------|-----------|----------|--------------|
| PNG | .png | Logos, icons, graphics | Yes |
| JPEG | .jpg, .jpeg | Photos, backgrounds | No |

### When to Use PNG

* Logos and brand marks
* Icons and UI elements
* Graphics with text
* Images needing transparent backgrounds
* Clean edges and sharp lines

### When to Use JPEG

* Photographic backgrounds
* Product photos
* Lifestyle imagery
* Large full-screen images (smaller file size)

## Size Guidelines

### Logos

| Type | Size | Format | Max File Size |
|------|------|--------|---------------|
| Main Logo | 512 x 512 px | PNG | 500 KB |
| App Icon | 256 x 256 px | PNG | 300 KB |
| Small Icon | 128 x 128 px | PNG | 150 KB |

### Backgrounds

| Orientation | Size | Format | Max File Size |
|-------------|------|--------|---------------|
| Portrait | 1080 x 1920 px | JPG/PNG | 2 MB |
| Landscape | 1920 x 1080 px | JPG/PNG | 2 MB |
| Square | 1080 x 1080 px | JPG/PNG | 2 MB |

### UI Elements

| Type | Size | Format | Max File Size |
|------|------|--------|---------------|
| Currency Icon | 64 x 64 px | PNG | 100 KB |
| Button Image | 256 x 128 px | PNG | 200 KB |
| Custom Icons | 128 x 128 px | PNG | 150 KB |

## Color Formats

| Format | Example | Usage |
|--------|---------|-------|
| Hex (6-digit) | #FF5722 | Standard colors |
| Hex (8-digit) | #FF572280 | Colors with transparency |

### Hex Color Breakdown

```
#FF5722
  ^^ Red (FF = 255)
    ^^ Green (57 = 87)
      ^^ Blue (22 = 34)

#FF572280
        ^^ Alpha/Opacity (80 = 50%)
```

## Preparing Images

### Removing Backgrounds

For logos and icons with transparent backgrounds:

1. Open in image editor (Photoshop, GIMP, Figma)
2. Remove background
3. Export as PNG-24
4. Verify transparency in preview

### Optimizing File Size

If your image is too large:

| Action | Reduction |
|--------|-----------|
| Reduce dimensions | ~75% smaller |
| Increase JPG compression | ~50% smaller |
| Use PNG-8 for simple graphics | ~60% smaller |
| Use online compression tool | ~30-50% smaller |

### Color Profile

* Use sRGB color profile
* Don't use CMYK (for print)
* Avoid embedded color profiles for smaller files

## Troubleshooting

| Issue | Cause | Solution |
|-------|-------|----------|
| White box around logo | Not PNG or transparency lost | Re-export as PNG-24 |
| Colors look wrong | Wrong color profile | Convert to sRGB |
| Image pixelated | Resolution too low | Use larger source |
| File won't upload | Too large | Compress or reduce size |
| Wrong dimensions | Aspect ratio mismatch | Crop to correct ratio |

## Tools for Image Preparation

### Free Online Tools

* TinyPNG - Compress PNG/JPG
* Remove.bg - Remove backgrounds
* Canva - Design and export
* GIMP - Full image editing

### Design Software

* Adobe Photoshop
* Figma
* Sketch
* Affinity Designer

## Related

* [All Parameters](all-parameters.md) - Parameter reference
* [Limits & Constraints](limits.md) - Size limits
