# 🖼️ img-toolkit-rust (Staging)

**img-toolkit-rust** is a high-performance image processing library rewritten in Rust (WASM) from the original TypeScript-based [img-toolkit](https://github.com/2YH02/img-toolkit). Leveraging WebAssembly, this version provides faster, more efficient, and reliable image manipulation directly in browsers.

## ✨ Features

- ⚡ **Fast & Efficient**: Powered by Rust and WebAssembly.
- 📸 **Supports JPEG, PNG, WebP** formats.
- 📐 **Resizing** with automatic aspect-ratio handling.
- 🎚️ **Adjust brightness** easily.
- 🔍 **Multiple resampling filters** (Nearest, Triangle, CatmullRom, Gaussian, Lanczos3).

## ⚙️ ResizeOptions

| Option       | Type   | Description                                                                                       |
| ------------ | ------ | ------------------------------------------------------------------------------------------------- |
| `width`      | number | (Optional) Target width in pixels. If omitted, width is auto-adjusted.                            |
| `height`     | number | (Optional) Target height in pixels. If omitted, height is auto-adjusted.                          |
| `quality`    | number | Image quality level ranging from 0.0 (lowest) to 1.0 (highest quality).                           |
| `format`     | string | Output format (`"jpg"`, `"png"`, `"webp"`).                                                       |
| `brightness` | number | (Optional) Brightness level from 0.0 (darkest) to 1.0 (brightest). Defaults to 0.5 if omitted.    |
| `resampling` | number | (Optional) Resampling quality from 0 (fastest) to 10 (highest quality). Defaults to 4 if omitted. |

## 🛠️ Build

```bash
# Build Rust -> WASM
wasm-pack build --target web

# Build TypeScript wrapper
tsc
```

## 🚧 Staging Repository Notice

This repository is a **staging version** rewritten in Rust from the original [img-toolkit](https://github.com/2YH02/img-toolkit) (TypeScript). Once fully stabilized and tested, this will replace the main library.

## 📄 License

MIT
