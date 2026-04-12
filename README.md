[README.md](https://github.com/user-attachments/files/26655382/README.md)
# Markdown → Rich Text Converter

A browser-based tool that converts Markdown into rich formatted text you can paste directly into **Quip**, **Microsoft Word**, **Google Docs**, or any rich text editor — with formatting intact.

![Split-screen editor with live preview](https://img.shields.io/badge/status-live-brightgreen)

## Features

- **Live split-screen preview** — type Markdown on the left, see formatted output on the right
- **Copy Rich Text** — one-click copy that preserves tables, code blocks, headings, and styles when pasted
- **File upload** — drag in any `.md` file
- **Zero setup** — single HTML file, no build tools, no dependencies to install

## Supported Markdown Elements

| Element | Support |
|---------|---------|
| Headings (H1–H6) | ✅ |
| Bold / Italic | ✅ |
| Tables with borders | ✅ |
| Fenced code blocks | ✅ |
| Inline code | ✅ |
| Ordered & unordered lists | ✅ |
| Nested lists | ✅ |
| Blockquotes | ✅ |
| Horizontal rules | ✅ |
| Hyperlinks | ✅ |

## Getting Started

Open `index.html` in any modern browser. That's it.

```bash
git clone https://github.com/<your-username>/markdown-converter.git
open index.html
```

Or visit the live version: `https://<your-username>.github.io/markdown-converter`

## How It Works

- Uses [marked.js](https://github.com/markedjs/marked) (loaded from CDN) for Markdown parsing
- All preview styles are **inline** so they survive copy-paste into Word and Quip
- Tables render with explicit borders and `border-collapse` for paste compatibility
- Clipboard API writes `text/html` with a `document.execCommand` fallback

## License

MIT
