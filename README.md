# ✦ Cantis AI — Beyond Imagination

> A production-ready, fully self-contained AI chatbot with stunning psychic/magical UI.

## 🚀 Quick Start

Just open **`index.html`** in any modern browser. No server, no build step, no dependencies to install.

```bash
open index.html   # macOS
# or double-click the file in Finder / Explorer
```

## ✨ Features

| Feature | Detail |
|---|---|
| **3D Animated Intro** | CANTIS text in rotating 3D with neon glow (CSS 3D + Three.js) |
| **Particle Background** | Three.js WebGL particle flow reacting to mouse movement |
| **Click Burst Effects** | Canvas 2D particle burst + ripple ring on every click |
| **Background Music** | Auto-plays atmospheric music with play/pause toggle |
| **Glassmorphism UI** | Frosted glass panels, chat container, settings panel |
| **AI Streaming** | Token-by-token streaming via OpenRouter API |
| **Markdown Rendering** | Full markdown + syntax-highlighted code blocks |
| **Copy Buttons** | Per-code-block and per-message copy buttons |
| **Chat History** | Persists to `localStorage` across sessions |
| **Settings Panel** | Temperature, tokens, reasoning, stream, JSON mode, tools |
| **Regenerate** | Re-generate the last AI response |

## ⚙️ Settings

Access via the gear icon (top-right):

- **Temperature** — Creativity / randomness (0 → 2)
- **Max Tokens** — Response length cap (256 → 8192)
- **Reasoning** — `low / medium / high` effort
- **Stream** — Token-by-token streaming toggle
- **JSON Mode** — Force JSON output format
- **Browser Search / Code Interpreter** — Tool toggles

## 🔑 API

- **Provider**: [OpenRouter](https://openrouter.ai)
- **Endpoint**: `https://openrouter.ai/api/v1/chat/completions`
- **Model**: `openai/gpt-4o-mini`

To change the model, edit `MODEL` in `index.html`:
```js
const MODEL = 'openai/gpt-4o-mini';  // or 'anthropic/claude-3.5-sonnet', etc.
```

## 📂 Structure

```
Cantis-AI/
├── index.html   ← entire app (HTML + CSS + JS, self-contained)
└── README.md
```

## 🎨 Tech Stack

- **Three.js r128** — WebGL 3D particle background
- **Marked.js** — Markdown rendering
- **highlight.js** — Syntax highlighting
- **CSS 3D Transforms** — Intro title animation
- **Canvas 2D** — Click burst particles
- **OpenRouter API** — AI backend (GPT-4o Mini)
