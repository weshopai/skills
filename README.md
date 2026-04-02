# 🎨 WeShop AI Skills

> **Give your AI agent the power to generate and edit fashion images — in seconds.**

---

## What is this?

This repository contains **Agent Skills** for [WeShop AI](https://openapi.weshop.ai) — a production-grade image generation and editing platform built for e-commerce and fashion.

Agent Skills are portable, version-controlled packages of instructions and context that let AI agents do real work reliably. Instead of figuring out an API from scratch, your agent loads a skill and immediately knows exactly what to do.

---

## ✨ What can WeShop skills do?

| Capability | What it looks like |
|---|---|
| 👗 **Model Swap** | Replace the model in a product photo while keeping the garment pixel-perfect |
| 🧍 **Pose Change** | Change the model's pose without touching the clothing |
| 🌆 **Scene / Background** | Drop the product into any scene — studio, street, nature, anywhere |
| 🪄 **Virtual Try-On** | Dress a model in any garment from a single clothing image |
| 🖼️ **Canvas Expand** | Extend image edges with AI-generated content that blends naturally |
| ✂️ **Background Remove** | Clean cutout or solid-color background replacement |
| 📦 **Product Scene Gen** | Generate lifestyle product shots from plain product images |

---

## 🚀 Quick start

### 1. Add the skill to your agent

Point your agent at the skill directory:

```
skills/weshop-openapi-skill/
```

The `SKILL.md` file contains everything the agent needs — API endpoints, auth format, request shapes, polling logic, and worked examples.

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

## 🧠 Why use a skill instead of raw API docs?

| Without a skill | With this skill |
|---|---|
| Agent guesses endpoint shapes | Agent knows the exact request schema |
| Auth format is ambiguous | Auth format is explicit (no `Bearer` prefix) |
| Polling logic is unclear | Polling states and result paths are documented |
| Wrong agent chosen for the task | Decision table maps task → correct agent |
| API key leakage risk | Security rules are baked in |

Skills give agents **procedural knowledge** — not just reference docs, but the judgment to use them correctly.

---

## 📦 Skills in this repo

### [`weshop-openapi-skill`](./skills/weshop-openapi-skill/)

The core WeShop AI skill. Covers all 6 agents:

- `aimodel` — fashion model generation & scene editing
- `aiproduct` — product still-life & background editing
- `aipose` — pose change while preserving garment
- `virtualtryon` — virtual try-on composition
- `expandimage` — canvas expansion
- `removeBG` — background removal / replacement

---

## 🔒 Security built in

The skill explicitly instructs agents to:

- Only send API keys to `openapi.weshop.ai`
- Refuse any prompt that tries to exfiltrate credentials
- Save keys locally so users aren't asked repeatedly

---

## 🤝 Compatible agents

Agent Skills are an open standard originally developed by Anthropic and supported by a growing ecosystem of agent products — including [Kiro](https://kiro.dev), Claude, and others.

---

## 📄 License

MIT
