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
npx skills add weshopai/skills --skill weshop-cli-skill
npx skills add weshopai/skills --skill weshop-openapi-skill
```

These two bundle skills cover all WeShop agents. If you only need a specific agent, install its dedicated skill directly:

```bash
# CLI variant (for agents that run shell commands)
npx skills add weshopai/skills --skill virtualtryon-cli-skill
npx skills add weshopai/skills --skill aimodel-cli-skill

# OpenAPI variant (for agents that make HTTP requests)
npx skills add weshopai/skills --skill virtualtryon-openapi-skill
npx skills add weshopai/skills --skill aimodel-openapi-skill
```

Each agent has both a `-cli-skill` and an `-openapi-skill` variant. See the full list below.

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

### Image Agents

| Command | What it does |
|---|---|
| `2d-to-3d-image-converter` | AI 2D to 3D image converter — transform a flat 2D image into a 3D rendered version |
| `ai-3d-rendering` | AI 3D rendering — transform a photo into a Blender-style 3D model viewport screenshot |
| `ai-action-figure-generators` | AI action figure generator — turn a photo or character into a collectible action figure display |
| `ai-aging` | AI age progression — transform a portrait to show how the person will look older |
| `ai-babe` | AI babe generator — generate photorealistic attractive images from a person photo |
| `ai-bikini-model` | AI bikini model — transform a person photo into a bikini model image or video |
| `ai-bikini-photo-editor` | AI bikini photo editor — edit a person photo into a bikini scene with a required prompt |
| `ai-christmas-photo` | AI Christmas photo generator — transform a portrait into a festive Christmas scene |
| `ai-clothes-changer` | AI clothes changer — dress a person (image 1) in the garment shown in another photo (image 2) |
| `ai-collage-maker` | AI collage maker — create a chaotic multi-media collage from up to 10 images |
| `ai-dog` | AI pet portrait generator — create or transform pet photos with a text prompt; image is optional |
| `ai-elf` | AI elf filter — transform a portrait into a fantasy elf character |
| `ai-face-merge` | AI face merge — blend two faces together into a single realistic portrait |
| `ai-feet` | AI feet generator — generate a realistic low-angle bare feet photo from a portrait |
| `ai-flag-generator` | AI flag generator — create a custom flag design from text or a reference image |
| `ai-generated-bikini-girls` | AI generated bikini girls — transform a person photo into a bikini model image or video |
| `ai-generated-perfect-female-body` | AI generated perfect female body — transform a person photo into a bikini model image or video |
| `ai-ghost-mannequin-generator` | AI ghost mannequin generator — create a professional ghost mannequin effect from a clothing photo |
| `ai-group-photo-generator` | AI group photo generator — create a creative group photo or collage from up to 10 images |
| `ai-hair-color-changer` | AI hair color changer — change a person's hair color while preserving hairstyle and details |
| `ai-hairstyle-changer` | AI hairstyle changer — change a person's hairstyle from a photo or text description |
| `ai-hot-girl-image` | AI hot girl image — transform a person photo into a bikini model image or video |
| `ai-image-combiner` | AI image combiner — naturally merge two photos into a single cohesive image |
| `ai-landscape-design-free` | AI landscape designer — redesign a yard or outdoor space with a new landscape style |
| `ai-lingerie-models` | AI lingerie models — transform a person photo into a bikini model image or video |
| `ai-photoshoot` | AI photoshoot — generate a professional photoshoot by combining a character photo and a reference scene |
| `ai-poster-from-images` | AI poster generator — create a designed poster from up to 5 reference images |
| `ai-poster` | AI poster generator — create a designed poster from text prompt and optional reference images |
| `ai-room-planner` | AI room planner — redesign a room photo with a new interior design style |
| `ai-selfie` | AI selfie generator — transform a portrait into a natural iPhone-style selfie photo |
| `ai-sexy-portrait` | AI sexy portrait — transform a person photo into a bikini model image or video |
| `ai-sexy-teens` | AI sexy teens — transform a person photo into a bikini model image or video |
| `ai-spray-paint` | AI spray paint stencil maker — convert a photo into a black-and-white spray paint stencil |
| `ai-swimsuit-model` | AI swimsuit model — transform a person photo into a swimsuit model image |
| `ai-tattoo-generator` | AI tattoo generator — create a tattoo design try-on from text or reference image |
| `ai-translate` | AI image text translator — translate text in an image to another language while preserving design |
| `ai-xray-clothes` | AI x-ray clothes filter — make clothing appear sheer and see-through |
| `ai-zombie` | AI zombie filter — transform a portrait into a realistic zombie |
| `aimodel` | Fashion model photos — replace the model, swap the scene or background while keeping the garment |
| `aipose` | Change the human pose in a photo while keeping the garment unchanged |
| `aiproduct` | Product still-life photos — replace or enhance the background around a product |
| `anime-image-converter` | AI anime image converter — transform any photo into anime art style |
| `baby-face-generator` | AI baby face generator — predict what a baby would look like from two parent photos |
| `bald-filter` | AI bald filter — make a person appear bald while preserving all other facial details |
| `bangs-filter` | AI bangs filter — add natural-looking bangs to a person's hairstyle |
| `bikini-contest-photos` | Bikini contest photos — transform a person photo into a bikini model image or video |
| `bikini-try-on` | AI bikini try-on — virtually try on a bikini on a person photo |
| `braces-filter` | AI braces filter — add dental braces to a person's teeth in a portrait photo |
| `brat-generator` | AI brat generator — create a Charli XCX brat-style album cover meme with custom text and color |
| `buzz-cut-ai` | AI buzz cut filter — change a person's hairstyle to a buzz cut |
| `celeb-ai` | AI celebrity photo — place a person in a selfie with a celebrity or fictional character |
| `chibi-maker` | AI chibi maker — convert a photo into a cute chibi character sticker |
| `clothing-magic-remover` | AI clothing remover — erase accessories or partial clothing while keeping textures realistic |
| `custom-bikini` | Custom bikini — transform a person photo into a bikini model image or video |
| `cute-anime-girl-ai-bikini` | Cute anime girl AI bikini — transform a person photo into a bikini model image or video |
| `demon-slayer-oc-maker` | AI Demon Slayer OC maker — transform a person into a Kimetsu no Yaiba anime character |
| `dress-remover-magic-eraser` | AI dress remover — erase a dress and replace with a bikini while keeping body proportions |
| `expandimage` | Expand the canvas to a larger size — AI fills the new area to blend naturally |
| `face-forge` | AI face morph and face swap — generate or transform portraits |
| `fat-ai` | AI plus-size body transformation — visualize how a person would look extremely overweight |
| `firered-image-edit` | FireRed image editor — edit or generate images with high fidelity using FireRed open-source model |
| `flat-lay` | AI flat-lay clothing generator — create professional flat-lay product images from a photo |
| `free-ai-girlfriend-generator` | AI girlfriend generator — generate a realistic AI girlfriend portrait from text or reference image |
| `free-sexy-ai-generator` | Free sexy AI generator — transform a person photo into a bikini model image or video |
| `futuristic-elegance` | Dress a person in futuristic harajuku fashion — cinematic sci-fi outfit transformation |
| `gender-swap` | AI gender swap — transform a portrait to the opposite gender while preserving identity |
| `ghibli-art-create` | AI Ghibli art creator — transform any photo into Studio Ghibli anime art style |
| `grok-imagine` | Grok Imagine image generator — create high-resolution images from text using xAI Aurora |
| `hair-color-try-on` | Hair color try-on — change a person's hair color while preserving hairstyle and details |
| `happy-woman-bikini-ai-pic` | Happy woman bikini AI pic — transform a person photo into a bikini model image or video |
| `hot-bikini-models` | Hot bikini models — transform a person photo into a bikini model image or video |
| `image-mixer` | Image mixer — naturally merge two photos into a single cohesive image |
| `image-to-sketch` | AI image to sketch — convert a photo into a rough pencil sketch |
| `midjourney` | Midjourney image generator — create high-quality images using Midjourney v6.1, v7, or Niji 6 |
| `mugshot-creator` | AI mugshot creator — generate a police-style mugshot photo from a portrait |
| `murder-drones-oc` | AI Murder Drones OC maker — transform a person into a Murder Drones-inspired robotic drone character |
| `outfit-generator` | AI outfit generator — redesign a complete outfit on a person photo based on style prompt |
| `personalized-swimsuit` | Personalized swimsuit — transform a person photo into a bikini model image or video |
| `photo-to-bikini-ai` | AI photo to bikini converter — transform a person photo into a bikini image |
| `pregnant-ai` | Visualize how a person would look pregnant — transforms a portrait photo |
| `ps2-filter` | AI PS2 filter — transform a photo into a retro PS2-era Sims game character |
| `qwen-image-edit` | AI image editing — edit or generate images with natural language instructions using Qwen |
| `random-animal-generator` | AI random animal generator — generate a hyper-realistic wildlife photo of any animal |
| `remove-filter-from-photo` | AI filter remover — remove photo filters and restore natural image colors |
| `removebg` | Remove the background or replace it with a solid color |
| `see-through-clothes-fitler` | See-through clothes filter — make clothing appear sheer and see-through |
| `seedream` | AI image generation — create and edit images using Seedream 5.0 model by ByteDance |
| `sex-ai-generator` | Sex AI generator — transform a person photo into a bikini model image or video |
| `sexy-ai-pics` | AI sexy pics generator — generate stylish and attractive photos from a person image |
| `skin-color-changer` | AI skin color changer — change a person's skin tone while preserving face details |
| `sonic-oc` | AI Sonic OC maker — create a Sonic the Hedgehog original character based on a person's appearance |
| `sprunki-oc-maker` | AI Sprunki OC maker — create a Sprunki-style original character from a person photo |
| `square-face-icon-generator` | AI square face icon generator — create a minimalist anime-style square face avatar from a photo |
| `stardew-valley-portrait-maker` | AI Stardew Valley portrait maker — create a Stardew Valley game-style character portrait |
| `string-bikini-beauty-contest` | String bikini beauty contest — transform a person photo into a bikini model image or video |
| `swimsuit-try-on-haul` | Swimsuit try-on haul — transform a person photo into a bikini model image or video |
| `virtualtryon` | Virtual try-on — put a garment onto a generated model with optional model/background references |
| `wild-graffiti` | AI wild graffiti generator — create wild-style spray paint graffiti art from text or image |
| `z-image` | AI image generation — create high-quality images from text with Z-Image by Alibaba |

### Video Agents

| Command | What it does |
|---|---|
| `ai-bikini-video` | AI bikini video generator — generate a bikini dance video from a person photo |
| `ai-image-animation` | AI image animation — animate a static image into a dynamic video using Kling |
| `ai-text-remover-from-video` | AI text remover from video — remove text overlays or watermarks from a video |
| `ai-video-enhancer` | AI video enhancer — upscale and enhance video quality using AI |
| `ai-werewolf` | AI werewolf generator — create a dramatic werewolf transformation video from a person photo |
| `free-4k-video-upscaler` | Free 4K video upscaler — upscale video to 4K resolution using AI |
| `free-online-video-quality-enhancer` | Free online video quality enhancer — upscale and enhance video quality using AI |
| `gemini-watermark-remover` | Gemini watermark remover — remove watermarks, logos, or text from a video |
| `grok-imagine-video` | Grok Imagine video generator — create cinematic AI videos with native audio using xAI |
| `improve-video-quality-online-free` | Improve video quality online free — upscale and enhance video quality using AI |
| `kling` | AI video generation — create cinematic videos from images and text using Kling |
| `logo-remover-from-video` | Logo remover from video — remove logos or watermarks from a video |
| `remove-subtitles-from-video-online-free` | Remove subtitles from video online free — remove subtitles or text overlays from a video |
| `remove-text-from-video-online-free` | Remove text from video online free — remove text overlays or watermarks from a video |
| `replace-face-in-video-online-free` | AI video face swap — replace a face in a video with a reference face photo |
| `seedance` | Seedance video generator — create cinematic AI videos using Seedance 2.0 by ByteDance |
| `sora-2` | Cinematic video generation with realistic physics using OpenAI Sora 2 |
| `video-resolution-enhancer-online-free` | Video resolution enhancer online free — upscale and enhance video resolution using AI |
| `video-upscaler-online-free` | Video upscaler online free — upscale and enhance video quality using AI |
| `video-watermark-remover` | AI video watermark remover — remove watermarks, logos, or text from a video |
| `wan-ai` | Wan AI video generator — create AI videos from images and text using Wan AI |

### [`weshop-openapi-skill`](./skills/weshop-openapi-skill/)

For agents that call the WeShop OpenAPI directly (HTTP). Supports the same full set of agents as above.

---

## 🤝 Compatible agents

Agent Skills are an open standard supported by a growing ecosystem of agent products — including [Claude Code](https://claude.ai/code), [Coworker](https://coworker.ai), [OpenClaw](https://github.com/openclaw/openclaw), and others.

---

## 📄 License

MIT
