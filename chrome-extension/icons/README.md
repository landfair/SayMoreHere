# Icons for Say More Here Chrome Extension

To complete the extension setup, you need to create icon images in the following sizes:

- icon16.png (16x16 pixels)
- icon48.png (48x48 pixels)
- icon128.png (128x128 pixels)

## Quick Way to Generate Icons

You can use the included `icon.svg` file and convert it to PNG using one of these methods:

### Option 1: Online SVG to PNG Converter
1. Go to https://svgtopng.com/ or similar service
2. Upload the `icon.svg` file
3. Download PNG versions in sizes: 16x16, 48x48, and 128x128

### Option 2: Using ImageMagick (if installed)
```bash
convert icon.svg -resize 16x16 icon16.png
convert icon.svg -resize 48x48 icon48.png
convert icon.svg -resize 128x128 icon128.png
```

### Option 3: Using Inkscape (if installed)
```bash
inkscape icon.svg -w 16 -h 16 -o icon16.png
inkscape icon.svg -w 48 -h 48 -o icon48.png
inkscape icon.svg -w 128 -h 128 -o icon128.png
```

## Temporary Workaround

For testing purposes, you can temporarily remove the "icons" section from `manifest.json`. Chrome will use a default icon until you add custom ones.
