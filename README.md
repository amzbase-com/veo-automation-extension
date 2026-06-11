<!--
  LINK STATUS: PARTIAL. The Chrome Web Store listing is LIVE — every "Install"
  link points to it. The official website is NOT live yet, so every bare
  "Website" link still points to THIS GitHub repo as a non-broken placeholder.
  Swap in the real website URL the moment it goes live.

  How links are distinguishable:
    - Install links are the Chrome Web Store URL, ending with  ...?hl=<lang>  (live)
    - Website links are the bare repo URL  ...veo-automation-extension  (no ?hl, placeholder)

  One-shot swap of the website placeholder across all 7 README files (run from repo root):

    sed -i '' \
      -e 's|https://github.com/amzbase-com/veo-automation-extension|YOUR_WEBSITE_URL|g' \
      README*.md
-->

[![Download on Chrome Web Store](https://img.shields.io/badge/⬇_Install-Chrome_Web_Store-success?style=for-the-badge&logo=googlechrome&logoColor=white)](https://chromewebstore.google.com/detail/veo-flow-automation-%E2%80%94-bat/inmkimakahiennggieafocbmfjlmfbhn?hl=en)
[![Website](https://img.shields.io/badge/🌐_Website-Visit-blue?style=for-the-badge)](https://github.com/amzbase-com/veo-automation-extension)

# 🎬 VEO Automation — Batch Google Flow Automation for VEO 3 Video & Nano Banana Images

[![English](https://img.shields.io/badge/English-blue)](README.md) [![中文](https://img.shields.io/badge/中文-red)](README_zh.md) [![한국어](https://img.shields.io/badge/한국어-orange)](README_ko.md) [![日本語](https://img.shields.io/badge/日本語-purple)](README_ja.md) [![Deutsch](https://img.shields.io/badge/Deutsch-green)](README_de.md) [![Français](https://img.shields.io/badge/Français-yellow)](README_fr.md) [![Русский](https://img.shields.io/badge/Русский-lightgrey)](README_ru.md)

> **VEO Automation** is the Chrome extension that turns [Google Flow](https://labs.google/fx/tools/flow) into a batch generation studio. Queue hundreds of prompts, generate **VEO 3** videos and **Nano Banana** images in bulk, and auto-download every result — no more babysitting one prompt at a time.

**Keywords this guide covers:** Google Flow automation · VEO automation · VEO 3 batch generation · Nano Banana batch image generator · bulk AI video generator · auto-download VEO videos · Google Flow Chrome extension.

---

## 📑 Table of Contents

- [Why VEO Automation](#-why-veo-automation)
- [Key Features](#-key-features)
- [Installation](#-installation)
- [Quick Start](#-quick-start)
- [Generation Modes](#-generation-modes)
- [Settings Reference](#-settings-reference)
- [Tips & Best Practices](#-tips--best-practices)
- [Troubleshooting](#-troubleshooting)
- [FAQ](#-faq)
- [Privacy & Permissions](#-privacy--permissions)
- [Pricing](#-pricing)

---

## 🚀 Why VEO Automation

Google Flow is powerful, but the official UI makes you run **one prompt at a time** and download **one file at a time**. If you produce content at scale — short-form video, marketing creative, storyboards, product shots — that manual loop is the bottleneck.

VEO Automation removes it:

- **Paste a list, walk away.** Drop in dozens or hundreds of prompts and the extension processes them sequentially, with retries, while you do something else.
- **VEO 3 video *and* Nano Banana images in one tool.** Most automations only touch video. This one batches both Google Flow video models and the Nano Banana image model from a single side panel.
- **Files land on disk automatically.** Every finished video and image is renamed and saved to a per-project folder — no right-click-save marathon.

If you searched for a *Google Flow batch tool*, *VEO 3 bulk generator*, or a way to *auto-download Nano Banana images*, this is built for exactly that.

---

## ✨ Key Features

| Feature | What it does |
| --- | --- |
| 🚀 **Batch queue** | Add unlimited prompts to a waiting list; tasks run one after another, automatically. |
| 📝 **Text-to-Video (VEO 3)** | Paste prompts or upload a `.txt` file with hundreds of lines to mass-produce videos. |
| 🖼️ **Image-to-Video (VEO 3)** | Animate still images using start-frame / end-frame control. |
| 🎨 **Text-to-Image (Nano Banana)** | Generate images from text descriptions in bulk. |
| 🔄 **Image-to-Image (Nano Banana)** | Transform or edit reference images at scale. |
| 💾 **Auto-download** | Saves finished videos and images to your machine instantly, organized by project folder. |
| 🔁 **Auto-retry** | Network hiccup or "creation failed" on Google's side? It waits and retries automatically. |
| 🔗 **Clip chaining (concat)** | Stitch 8-second segments into longer continuous videos. |
| ⚙️ **Deep customization** | Pick model, aspect ratio (16:9 / 9:16 / 1:1), outputs per prompt (1–4), concurrency, and per-prompt delay. |
| 🌍 **7 languages** | English, 中文, 한국어, 日本語, Deutsch, Français, Русский. |

---

## 📥 Installation

### Chrome Web Store (recommended)

1. Open the [**VEO Automation listing**](https://chromewebstore.google.com/detail/veo-flow-automation-%E2%80%94-bat/inmkimakahiennggieafocbmfjlmfbhn?hl=en) on the Chrome Web Store.
2. Click **Add to Chrome** → **Add extension**.
3. Pin the extension: click the puzzle-piece icon in Chrome's toolbar, then the pin next to **VEO Automation**, so it's one click away next time.

> **Compatibility:** Chrome 137+ (and Chromium-based browsers such as Edge and Brave). The extension opens as a **side panel** beside Google Flow.

---

## ⚡ Quick Start

1. **Open Google Flow.** Go to [labs.google/fx/tools/flow](https://labs.google/fx/tools/flow) and open (or create) a project. The extension only activates on Flow project pages.
2. **Open the side panel.** Click the VEO Automation icon. Sign in to unlock your daily quota.
3. **Pick a mode.** Choose one of the five generation modes (below).
4. **Add your prompts.** Type them, or upload a `.txt` file.
5. **Click Run.** Watch the queue process each task, retry on errors, and auto-download results.

> ℹ️ **Heads-up about the "debugging" banner.** While the extension runs, Chrome shows a *"… is being debugged"* bar at the top. This is required: Google Flow only accepts genuine, trusted user input, so the extension drives the page through Chrome's official debugging interface. It is not malware — it's the cost of reliable automation. Don't close the banner while a batch is running.

---

## 🎛️ Generation Modes

### 1. Text-to-Video — VEO 3

Mass-produce videos straight from text.

1. Select **Text-to-Video**.
2. Enter prompts in the box (separate each prompt with a **blank line**) **or** click **Upload .txt** to import a prompt list.
3. Set duration (single 8s clip, or **Concat** for longer chained videos).
4. Click **Run**.

**Example prompt list:**

```
A lone lighthouse on a cliff at golden hour, waves crashing below, slow cinematic dolly-in.

A neon-lit Tokyo alley in the rain, reflections on wet asphalt, steam rising, handheld feel.

Aerial shot gliding over autumn forest, low morning fog between the trees, warm light.
```

### 2. Image-to-Video — VEO 3

Bring still frames to life.

1. Select **Image-to-Video**.
2. Click **Select images** (multi-select supported) and drag to reorder by name, date, or custom order.
3. Write a prompt per image (blank-line separated).
4. Choose duration, then **Run**.

> **Tip:** Use a start frame + end frame to control how the motion begins and ends. Configure 1–2 images per prompt in Settings.

### 3. Text-to-Image — Nano Banana

Generate images from descriptions, in bulk.

1. Select **Text-to-Image**.
2. Enter detailed image prompts (blank-line separated).
3. Set aspect ratio and image quality in Settings.
4. **Run** — every image auto-downloads at your chosen resolution (1K / 2K / 4K).

### 4. Image-to-Image — Nano Banana

Edit or restyle reference images at scale.

1. Select **Image-to-Image**.
2. Upload source images.
3. Write transformation prompts (e.g. *"same character, cyberpunk outfit, rooftop at night"*).
4. **Run** to generate variations based on your references.

> **Auto-match characters by filename (optional):** name your references `dog.png`, `cat.png`, `duck.png`. A prompt that mentions *"dog playing with cat"* automatically pulls in `dog.png` and `cat.png`. Perfect for keeping characters consistent across a series.

### 5. Queue Management

- See every pending task in the **Prompt Queue**.
- **Remove** tasks you no longer need, or **Stop** a running batch.
- Track real-time progress per prompt.

---

## ⚙️ Settings Reference

Open the **Settings** tab to tune behavior.

**General**
- **Default mode** — auto-selected each time you open the panel.
- **Default aspect ratio** — 16:9, 9:16, or 1:1.
- **Outputs per prompt** — 1–4 videos/images per prompt.
- **Concurrent prompts** — run 1–6 prompts at the same time.
- **Prompt delay** — wait 0–300s between prompts to ease server load.

**Models**
- **Video model** — choose your VEO model (e.g. VEO 3 / VEO 3 Fast).
- **Image model** — Nano Banana for text-to-image and image-to-image.

**Download**
- **Video quality** — 720p, 1080p, or off.
- **Image quality** — 1K, 2K, 4K, or off.
- Files save to Chrome's Downloads folder, one subfolder per project.

**Advanced**
- **Max retries** — 1–20 attempts on failure.
- **Default video frame** — 8s or Concat.
- **Max images per prompt** — set per mode.
- **Language** — switch the UI among 7 languages.

---

## 💡 Tips & Best Practices

**Writing prompts**
- Be specific about subject, style, camera motion, and lighting.
- English prompts tend to be the most reliable on Google Flow.
- Separate prompts with a single blank line.

**Throughput vs. stability**
- Off-peak: ~3 concurrent prompts works well.
- Peak hours: drop to 2 and raise the delay to ~30s — fewer "creation failed" errors.
- More concurrency = faster but less stable; tune to taste.

**Managing assets**
- Name reference images clearly so auto-matching works.
- Stick to PNG / JPG / GIF, ideally under 10 MB each.

**Reliability**
- Leave **Auto-retry** on for unattended overnight batches.
- Higher delay = lighter server load = fewer failures.

---

## 🔧 Troubleshooting

| Symptom | Cause & fix |
| --- | --- |
| **Extension does nothing** | You must be on a Google Flow **project** page. Confirm the extension is enabled, refresh, and reopen the panel. |
| **"Cannot create video"** | Google Flow is temporarily overloaded. Don't worry — the extension waits and retries every ~30s until a slot frees up. |
| **Videos/images won't download** | In Chrome: **Settings → Downloads → turn off** *"Ask where to save each file before downloading."* Then recheck the download quality in Settings. |
| **"Policy error"** | Your prompt or image tripped Google's content policy. The tool skips that task and moves to the next automatically. |
| **Generation keeps failing** | Check your connection, verify prompts are valid, raise Max retries, and review the browser console for clues. |
| **The page zoomed out by itself** | Intentional — the tool adjusts zoom so it can locate buttons precisely. Don't change zoom manually while a batch runs. |
| **"Being debugged" banner won't go away** | Expected while running (see Quick Start). It disappears when the batch finishes or you stop it. |

---

## ❓ FAQ

**Is VEO Automation affiliated with Google?**
No. It's an independent third-party tool that automates the public Google Flow web app. It is not affiliated with, endorsed by, or connected to Google.

**What is Nano Banana?**
Nano Banana is the image model available through Google Flow. VEO Automation lets you batch-generate and auto-download Nano Banana images alongside your VEO 3 videos — from the same queue.

**Can I really generate hundreds of videos at once?**
Yes. Upload a `.txt` file of prompts (or paste a long list) and the queue processes them one by one with automatic retries. Practical throughput depends on Google Flow's load and your concurrency/delay settings.

**Does it work for short-form vertical video?**
Yes — set the aspect ratio to **9:16** for TikTok / Reels / Shorts, **16:9** for YouTube, or **1:1** for square.

**Where do my files go?**
To your Chrome Downloads folder, organized into one subfolder per project, renamed automatically so they're easy to sort.

**Do I need an API key?**
No. It drives your own logged-in Google Flow session in the browser — no separate API key or developer account required.

**Is my data sent anywhere?**
Your prompts, images, and videos are processed in your browser on Google Flow. The extension stores settings locally. See [Privacy & Permissions](#-privacy--permissions).

**Which browsers are supported?**
Chrome 137+ and Chromium-based browsers (Edge, Brave). A side panel is required.

---

## 🔒 Privacy & Permissions

- **Runs in your browser.** Automation happens on your own Google Flow session.
- **Minimal data.** Settings are stored in Chrome local storage. The extension doesn't sell or harvest your creative content.
- **Scoped permissions.** Host access is limited to `labs.google/*` (to automate Flow) and the extension's own backend (for sign-in and quota).
- **The debugger permission** is used solely to send trusted input events to Google Flow, which the page requires — see [Quick Start](#-quick-start).

Full details: [https://github.com/amzbase-com/veo-automation-extension](https://github.com/amzbase-com/veo-automation-extension)

---

## 💳 Pricing

VEO Automation is **freemium**:

- **Free** — a daily generation quota that resets every day. Great for trying it out and light use.
- **Pro** — higher or unlimited quota for power users running large batches.

Sign in inside the side panel to see your current quota. Manage your plan at [https://github.com/amzbase-com/veo-automation-extension](https://github.com/amzbase-com/veo-automation-extension).

---

## 🌐 Links

- **Install:** [Chrome Web Store](https://chromewebstore.google.com/detail/veo-flow-automation-%E2%80%94-bat/inmkimakahiennggieafocbmfjlmfbhn?hl=en)
- **Website:** [https://github.com/amzbase-com/veo-automation-extension](https://github.com/amzbase-com/veo-automation-extension)
- **Google Flow:** [labs.google/fx/tools/flow](https://labs.google/fx/tools/flow)

---

_Disclaimer: VEO Automation is an independent project and is **not** affiliated with, endorsed by, or connected to Google or the Google Flow team. "VEO", "Nano Banana", "Google Flow", and "Google" are trademarks of Google LLC. Use of this tool is subject to Google's terms of service._