# Localization Char Extractor

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE.md)
![stability-experimental](https://img.shields.io/badge/stability-experimental-orange.svg)
[![Live Demo](https://img.shields.io/badge/Live%20Demo-GitHub%20Pages-blue?logo=github)](https://llarean.github.io/localization-char-extractor/)

> [!WARNING]
> Work in progress. Use at your own risk.

Browser-based utility for extracting unique characters from localization JSON files. Useful for generating character sets required by custom fonts in game and app localization workflows.

## Preview

![Screenshot](wwwroot/Screenshot.jpg)

## Live Demo

**[https://llarean.github.io/localization-char-extractor/](https://llarean.github.io/localization-char-extractor/)**

## Quick Start

1. Paste or drag-and-drop your localization JSON into the input field
2. Select one or more languages from the auto-detected list
3. Optionally filter by Unicode range and toggle emoji inclusion
4. Click **Extract characters** (or press `Ctrl+Enter`)
5. Fine-tune the result by clicking individual characters to exclude them
6. Choose an output format and copy to clipboard

## Features

- **Multi-language selection** — extract from multiple languages at once and merge into a single deduplicated set
- **Unicode range presets** — filter output to All / Latin / Cyrillic / Greek / Arabic / CJK
- **Emoji filter** — include or exclude emoji characters
- **Interactive character grid** — click any character to exclude it; use **all / none** to select in bulk
- **Output formats** — copy as a plain string (for TextMesh Pro *Custom Characters*) or as `U+XXXX` codes (for BMFont, Hiero)
- **Hover tooltips** — shows the Unicode code point for each character
- **Drag-and-drop** — drop a `.json` file directly onto the input area
- **Persistent input** — JSON is saved to `localStorage` and restored on reload
- **Keyboard shortcut** — `Ctrl+Enter` triggers extraction from anywhere on the page

## Expected JSON Structure

```json
{
  "Localization": {
    "files": [
      {
        "name": "English",
        "content": "{\"KEY_HELLO\": \"Hello\", \"KEY_WORLD\": \"World\"}"
      },
      {
        "name": "Japanese",
        "content": "{\"KEY_HELLO\": \"こんにちは\", \"KEY_WORLD\": \"世界\"}"
      }
    ]
  }
}
```

## Requirements

- A modern browser (Chrome, Firefox, Edge)
- No installation needed — runs entirely in the browser

## Contributing

- **Bug reports**: [Open an issue](https://github.com/LLarean/localization-char-extractor/issues)
- **Feature requests**: Describe your use case in an issue
- **Pull requests**: For bug fixes or improvements

---

<div align="center">

**Made with ❤️ for the localization community**

⭐ If this project helped you, please consider giving it a star!

</div>
