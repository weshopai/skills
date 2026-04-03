# 🎨 WeShop AI Skills

> **Give your AI agent the power to generate and edit fashion images.**

---

## What is this?

This repository contains **Agent Skills** for [WeShop AI](https://openapi.weshop.ai) — a production-grade image generation and editing platform built for e-commerce and fashion.

Instead of figuring out an API from scratch, your agent loads a skill and immediately knows exactly what to do.

---

## ✨ What can WeShop skills do?

| Capability | What it looks like |
|---|---|
| 👗 **Model Swap** | Replace the model in a product photo while keeping the garment pixel-perfect |
| 🧍 **Pose Change** | Change the model's pose without touching the clothing |
| 🌆 **Scene / Background** | Drop the product into any scene — studio, street, nature, anywhere |
| � **Virtual Try-On** | Dress a modeel in any garment from a single clothing image |
| 🖼️ **Canvas Expand** | Extend image edges with AI-generated content that blends naturally |
| ✂️ **Background Remove** | Clean cutout or solid-color background replacement |
| 📦 **Product Scene Gen** | Generate lifestyle product shots from plain product images |

---

## 🚀 Quick start

### 1. Add the skill to your agent

Pick the skill that fits your agent's capabilities and point it at the skill directory:

```
skills/weshop-cli-skill/     ← if your agent can run shell commands
skills/weshop-openapi-skill/ ← if your agent can make HTTP requests
```

### 2. Get an API key

Sign up at [weshop.ai](https://www.weshop.ai) and grab your API key from the dashboard.

### 3. Ask your agent to do something

```
Take this product photo and generate 4 lifestyle shots with different backgrounds.
```

```
Swap the model in this image with a different fashion model, keep the outfit.
```

```
Do a virtual try-on: put this jacket on the model in the reference photo.
```

That's it. The agent handles the rest.

---

## 📦 Skills in this repo

### [`weshop-cli-skill`](./skills/weshop-cli-skill/)

For agents that run shell commands via the `weshop` CLI. Covers 6 agents plus `upload` and `status` utilities. Requires `weshop-cli` installed (`npm install -g weshop-cli@0.1.0`) and the `WESHOP_API_KEY` environment variable set.

- `aimodel` — fashion model generation & scene editing
- `aiproduct` — product still-life & background editing
- `aipose` — pose change while preserving garment
- `virtualtryon` — virtual try-on composition
- `expandimage` — canvas expansion
- `removeBG` — background removal / replacement

### [`weshop-openapi-skill`](./skills/weshop-openapi-skill/)

For agents that call the WeShop OpenAPI directly (HTTP). Covers the same 6 agents.

---

## 🤝 Compatible agents

Agent Skills are an open standard supported by a growing ecosystem of agent products — including [Claude Code](https://claude.ai/code), [Coworker](https://coworker.ai), [OpenClaw](https://github.com/openclaw/openclaw), and others.

---

## 📄 License

MIT
