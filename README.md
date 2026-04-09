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
| 👙 **Virtual Try-On** | Dress a model in any garment from a single clothing image |
| 🖼️ **Canvas Expand** | Extend image edges with AI-generated content that blends naturally |
| ✂️ **Background Remove** | Clean cutout or solid-color background replacement |
| 📦 **Product Scene Gen** | Generate lifestyle product shots from plain product images |
| 🎬 **AI Video Generation** | Create cinematic videos from images and text using Kling, Sora 2, Wan AI, Seedance, and more |
| 🎨 **Image Generation** | Generate high-quality images with Midjourney, Seedream, Grok Imagine, Z-Image, and more |
| 🔄 **Photo Transformation** | Face swap, gender swap, age progression, style transfer, and 100+ creative filters |
| 🎥 **Video Enhancement** | Upscale video quality, remove watermarks, remove subtitles, and face swap in videos |

---

## 🚀 Quick start

### 1. Add the skill to your agent

Pick the skill that fits your agent's capabilities and install it:

```bash
npx skills add weshopai/skills@weshop-cli-skill
npx skills add weshopai/skills@weshop-openapi-skill
```

For OpenClaw users:

```bash
clawhub install weshop-cli-skill
clawhub install weshop-openapi-skill
```

Or point your agent directly at the skill directory:

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

For agents that run shell commands via the `weshop` CLI. Requires `weshop-cli` installed (`npm install -g weshop-cli@0.2.1`) and the `WESHOP_API_KEY` environment variable set.

**Image editing (fashion & product)**

| Command | What it does |
|---|---|
| `virtualtryon` | Put a garment onto a generated model with optional model/background references |
| `aimodel` | Replace the model, swap the scene or background while keeping the garment |
| `aiproduct` | Replace or enhance the background around a product |
| `aipose` | Change the human pose while keeping the garment unchanged |
| `expandimage` | Expand the canvas — AI fills the new area to blend naturally |
| `removebg` | Remove the background or replace it with a solid color |
| `flat-lay` | Generate flat-lay product shots |
| `ai-ghost-mannequin-generator` | Ghost mannequin effect for apparel photography |
| `outfit-generator` | Generate outfit combinations |
| `ai-clothes-changer` | Change clothing on a model |

**AI image generation**

| Command | What it does |
|---|---|
| `seedream` | Generate or edit images with Seedream 5.0 by ByteDance (text + up to 14 reference images) |
| `midjourney` | Generate images with Midjourney v6.1, v7, or Niji 6 |
| `grok-imagine` | Generate high-resolution images with xAI Aurora (Grok Imagine) |
| `z-image` | Text-to-image generation with Z-Image by Alibaba |
| `qwen-image-edit` | Edit or generate images with natural language using Qwen (up to 5 reference images) |
| `firered-image-edit` | Edit or generate images with FireRed open-source model (up to 3 reference images) |

**AI video generation**

| Command | What it does |
|---|---|
| `kling` | Generate cinematic videos from images using Kling (v2.1–v3.0, 3s–15s, optional audio) |
| `seedance` | Generate AI videos with Seedance 2.0 by ByteDance (up to 15s, optional audio) |
| `sora-2` | Generate cinematic videos with realistic physics using OpenAI Sora 2 |
| `wan-ai` | Generate AI videos from images and text using Wan AI |
| `grok-imagine-video` | Generate cinematic AI videos with native audio using xAI |
| `ai-bikini-video` | AI video generation for swimwear/fashion scenes |
| `ai-image-animation` | Animate a still image into a short video |

**Video editing & enhancement**

| Command | What it does |
|---|---|
| `ai-video-enhancer` | Upscale and enhance video quality (up to 4K) |
| `video-watermark-remover` | Remove watermarks from videos |
| `replace-face-in-video-online-free` | Replace a face in a video |
| `remove-subtitles-from-video-online-free` | Remove subtitles from a video |
| `ai-text-remover-from-video` | Remove text overlays from a video |
| `logo-remover-from-video` | Remove logos from a video |
| `gemini-watermark-remover` | Remove watermarks using Gemini |
| `remove-text-from-video-online-free` | Remove text from a video |
| `video-upscaler-online-free` | Upscale video resolution |
| `video-resolution-enhancer-online-free` | Enhance video resolution |
| `improve-video-quality-online-free` | General video quality improvement |
| `free-online-video-quality-enhancer` | Free video quality enhancement |
| `free-4k-video-upscaler` | Upscale video to 4K |

**Creative & fun image tools**

| Command | What it does |
|---|---|
| `face-forge` | Face swap / face replacement |
| `ai-face-merge` | Merge two faces together |
| `gender-swap` | Swap gender in a photo |
| `ai-aging` | Age a person in a photo |
| `ai-hairstyle-changer` | Change hairstyle |
| `ai-hair-color-changer` | Change hair color |
| `hair-color-try-on` | Try on a hair color |
| `buzz-cut-ai` | Apply a buzz cut |
| `bald-filter` | Apply a bald filter |
| `bangs-filter` | Add bangs |
| `braces-filter` | Add braces |
| `skin-color-changer` | Change skin tone |
| `ai-selfie` | Generate an AI selfie |
| `ai-photoshoot` | Generate a professional AI photoshoot |
| `ai-poster` | Generate an AI poster |
| `ai-poster-from-images` | Create a poster from reference images |
| `image-to-sketch` | Convert a photo to a sketch |
| `anime-image-converter` | Convert a photo to anime style |
| `ghibli-art-create` | Convert a photo to Ghibli art style |
| `chibi-maker` | Turn a photo into a chibi character |
| `2d-to-3d-image-converter` | Convert a 2D image to 3D |
| `ai-3d-rendering` | Generate a 3D rendering |
| `ps2-filter` | Apply a PS2-era filter |
| `wild-graffiti` | Apply a graffiti art style |
| `ai-spray-paint` | Apply a spray paint effect |
| `image-mixer` | Mix two images together |
| `ai-image-combiner` | Combine multiple images |
| `ai-collage-maker` | Create a collage from images |
| `remove-filter-from-photo` | Remove a filter from a photo |
| `square-face-icon-generator` | Generate a square face icon |
| `mugshot-creator` | Create a mugshot-style photo |

**Character & avatar generators**

| Command | What it does |
|---|---|
| `celeb-ai` | Generate a celebrity-style photo |
| `ai-babe` | Generate a fashion model photo |
| `free-ai-girlfriend-generator` | Generate an AI companion photo |
| `baby-face-generator` | Generate a baby face from two parents |
| `ai-dog` | Generate an AI dog photo |
| `ai-group-photo-generator` | Generate a group photo |
| `ai-action-figure-generators` | Turn a photo into an action figure |
| `sonic-oc` | Generate a Sonic OC |
| `demon-slayer-oc-maker` | Generate a Demon Slayer OC |
| `sprunki-oc-maker` | Generate a Sprunki OC |
| `murder-drones-oc` | Generate a Murder Drones OC |
| `stardew-valley-portrait-maker` | Generate a Stardew Valley portrait |
| `random-animal-generator` | Generate a random animal image |
| `ai-elf` | Generate an elf character |
| `ai-werewolf` | Generate a werewolf character |
| `ai-zombie` | Generate a zombie character |
| `ai-christmas-photo` | Generate a Christmas-themed photo |
| `brat-generator` | Generate a brat-style photo |
| `futuristic-elegance` | Generate a futuristic elegance portrait |
| `pregnant-ai` | Generate a pregnancy photo |
| `fat-ai` | Apply a weight-change filter |

**Swimwear & fashion try-on**

| Command | What it does |
|---|---|
| `bikini-try-on` | Virtual bikini try-on |
| `swimsuit-try-on-haul` | Swimsuit try-on haul |
| `personalized-swimsuit` | Generate a personalized swimsuit photo |
| `custom-bikini` | Generate a custom bikini photo |
| `ai-swimsuit-model` | Generate a swimsuit model photo |
| `ai-bikini-model` | Generate a bikini model photo |
| `ai-bikini-photo-editor` | Edit a bikini photo |
| `photo-to-bikini-ai` | Convert a photo to a bikini photo |

**Other tools**

| Command | What it does |
|---|---|
| `ai-translate` | Translate text in an image |
| `ai-tattoo-generator` | Generate a tattoo design |
| `ai-flag-generator` | Generate a custom flag |
| `ai-landscape-design-free` | Generate a landscape design |
| `ai-room-planner` | Generate a room layout |
| `see-through-clothes-fitler` | See-through clothing filter |
| `clothing-magic-remover` | Remove clothing in a photo |
| `dress-remover-magic-eraser` | Remove a dress in a photo |
| `ai-xray-clothes` | X-ray clothing filter |
| `upload` | Upload a local image and get a reusable URL |
| `status` | Check the status of a run by execution ID |
| `info` | List available preset IDs (scenes, models, background colors) |

### [`weshop-openapi-skill`](./skills/weshop-openapi-skill/)

For agents that call the WeShop OpenAPI directly (HTTP). Covers the core 6 e-commerce and fashion agents: `aimodel`, `aiproduct`, `aipose`, `virtualtryon`, `expandimage`, `removebg`.

---

## 🤝 Compatible agents

Agent Skills are an open standard supported by a growing ecosystem of agent products — including [Claude Code](https://claude.ai/code), [Coworker](https://coworker.ai), [OpenClaw](https://github.com/openclaw/openclaw), and others.

---

## 📄 License

MIT
