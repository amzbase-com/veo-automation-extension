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

[![在 Chrome 应用商店下载](https://img.shields.io/badge/⬇_安装-Chrome_应用商店-success?style=for-the-badge&logo=googlechrome&logoColor=white)](https://chromewebstore.google.com/detail/veo-flow-automation-%E2%80%94-bat/inmkimakahiennggieafocbmfjlmfbhn?hl=zh)
[![官方网站](https://img.shields.io/badge/🌐_官网-访问-blue?style=for-the-badge)](https://github.com/amzbase-com/veo-automation-extension)

# 🎬 VEO Automation —— Google Flow 批量自动化，批量生成 VEO 3 视频与 Nano Banana 图像

[![English](https://img.shields.io/badge/English-blue)](README.md) [![中文](https://img.shields.io/badge/中文-red)](README_zh.md) [![한국어](https://img.shields.io/badge/한국어-orange)](README_ko.md) [![日本語](https://img.shields.io/badge/日本語-purple)](README_ja.md) [![Deutsch](https://img.shields.io/badge/Deutsch-green)](README_de.md) [![Français](https://img.shields.io/badge/Français-yellow)](README_fr.md) [![Русский](https://img.shields.io/badge/Русский-lightgrey)](README_ru.md)

> **VEO Automation** 是一款把 [Google Flow](https://labs.google/fx/tools/flow) 变成「批量生成工作室」的 Chrome 扩展。把上百条 prompt 丢进队列，批量生成 **VEO 3** 视频和 **Nano Banana** 图像，每个结果自动下载到本地——再也不用守着电脑一条一条地点。

**本指南覆盖的关键词：** Google Flow 自动化 · VEO 自动化（VEO automation）· VEO 3 批量生成 · Nano Banana 批量图像生成器 · 批量 AI 视频生成器（bulk AI video generator）· 自动下载 VEO 视频 · Google Flow Chrome 扩展。

---

## 📑 目录

- [为什么选 VEO Automation](#-为什么选-veo-automation)
- [核心功能](#-核心功能)
- [安装方法](#-安装方法)
- [快速上手](#-快速上手)
- [生成模式](#-生成模式)
- [设置项说明](#-设置项说明)
- [技巧与最佳实践](#-技巧与最佳实践)
- [常见问题排查](#-常见问题排查)
- [FAQ](#-faq)
- [隐私与权限](#-隐私与权限)
- [定价](#-定价)

---

## 🚀 为什么选 VEO Automation

Google Flow 很强大，但官方界面只能让你**一次跑一条 prompt**、**一次下载一个文件**。如果你要规模化产出内容——短视频、营销创意、分镜脚本、产品图——这种手动循环就是最大的瓶颈。

VEO Automation 帮你彻底干掉这个瓶颈：

- **粘贴一份列表，然后走开。** 一次丢进几十上百条 prompt，扩展会带重试地按顺序处理，期间你可以去忙别的。
- **VEO 3 视频*和* Nano Banana 图像，一个工具全搞定。** 大多数自动化方案只能跑视频。它能在同一个侧边栏里同时批量跑 Google Flow 的视频模型和 Nano Banana 图像模型。
- **文件自动落盘。** 每个生成好的视频和图像都会被重命名并保存到对应项目的文件夹里——告别右键「另存为」的体力活。

如果你在搜「*Google Flow 批量工具*」「*VEO 3 批量生成器*」，或者想要「*自动下载 Nano Banana 图像*」的办法，那它就是为你量身打造的。

---

## ✨ 核心功能

| 功能 | 作用 |
| --- | --- |
| 🚀 **批量队列** | 把无限条 prompt 加入等待列表，任务自动一条接一条地跑。 |
| 📝 **文生视频（VEO 3）** | 粘贴 prompt，或上传含上百行的 `.txt` 文件，批量产出视频。 |
| 🖼️ **图生视频（VEO 3）** | 用首帧 / 尾帧控制，让静态图片动起来。 |
| 🎨 **文生图（Nano Banana）** | 根据文字描述批量生成图像。 |
| 🔄 **图生图（Nano Banana）** | 规模化地转换或编辑参考图像。 |
| 💾 **自动下载** | 生成完的视频和图像立刻保存到本地，并按项目文件夹归类。 |
| 🔁 **自动重试** | 网络抖动，或 Google 那边「创建失败」？它会自动等待并重试。 |
| 🔗 **片段拼接（concat）** | 把多个 8 秒片段拼成更长的连续视频。 |
| ⚙️ **深度自定义** | 自选模型、宽高比（16:9 / 9:16 / 1:1）、每条 prompt 的产出数量（1–4）、并发数和每条 prompt 间隔。 |
| 🌍 **7 种语言** | English、中文、한국어、日本語、Deutsch、Français、Русский。 |

---

## 📥 安装方法

### Chrome 应用商店（推荐）

1. 打开 Chrome 应用商店里的 [**VEO Automation 扩展页面**](https://chromewebstore.google.com/detail/veo-flow-automation-%E2%80%94-bat/inmkimakahiennggieafocbmfjlmfbhn?hl=zh)。
2. 点击 **添加至 Chrome** → **添加扩展程序**。
3. 固定扩展：点击 Chrome 工具栏的拼图图标，再点 **VEO Automation** 旁边的图钉，下次一键即可打开。

> **兼容性：** Chrome 137+（以及 Edge、Brave 等基于 Chromium 的浏览器）。扩展会以**侧边栏**形式在 Google Flow 旁边打开。

---

## ⚡ 快速上手

1. **打开 Google Flow。** 进入 [labs.google/fx/tools/flow](https://labs.google/fx/tools/flow)，打开（或新建）一个项目。扩展仅在 Flow 项目页面上生效。
2. **打开侧边栏。** 点击 VEO Automation 图标，登录以解锁你的每日额度。
3. **选择模式。** 从下面五种生成模式里挑一个。
4. **添加 prompt。** 直接输入，或上传 `.txt` 文件。
5. **点击「运行」。** 看着队列逐条处理任务、出错自动重试、结果自动下载。

> ℹ️ **关于「调试中」横幅的提醒。** 扩展运行时，Chrome 顶部会出现一条*「……正在被调试」*的提示条。这是必需的：Google Flow 只接受真实可信的用户输入，因此扩展通过 Chrome 官方的调试接口来驱动页面。它不是恶意软件——这是实现可靠自动化的必要代价。批量任务运行期间请不要关闭这条横幅。

---

## 🎛️ 生成模式

### 1. 文生视频 —— VEO 3

直接用文字批量产出视频。

1. 选择 **文生视频**。
2. 在输入框里填写 prompt（每条 prompt 之间用**空行**分隔），**或**点击 **上传 .txt** 导入一份 prompt 列表。
3. 设置时长（单条 8 秒片段，或用 **Concat 拼接**生成更长的连续视频）。
4. 点击 **运行**。

**示例 prompt 列表：**

```
悬崖上一座孤零零的灯塔，黄金时刻的暖光，海浪在下方拍打，缓慢的电影感推镜。

雨中霓虹闪烁的东京小巷，湿漉漉的柏油路上倒映着灯光，蒸汽升腾，手持镜头的晃动感。

航拍镜头滑过秋日森林，树木之间弥漫着清晨低垂的薄雾，暖色调光线。
```

### 2. 图生视频 —— VEO 3

让静帧动起来。

1. 选择 **图生视频**。
2. 点击 **选择图片**（支持多选），可拖动按文件名、日期或自定义顺序排序。
3. 为每张图片写一条 prompt（用空行分隔）。
4. 选好时长，然后 **运行**。

> **小贴士：** 用首帧 + 尾帧来控制运动如何开始和结束。可在「设置」里配置每条 prompt 使用 1–2 张图片。

### 3. 文生图 —— Nano Banana

根据文字描述批量生成图像。

1. 选择 **文生图**。
2. 输入详细的图像 prompt（用空行分隔）。
3. 在「设置」里设定宽高比和图像质量。
4. **运行**——每张图都会按你选的分辨率（1K / 2K / 4K）自动下载。

### 4. 图生图 —— Nano Banana

规模化地编辑或重塑参考图像。

1. 选择 **图生图**。
2. 上传源图像。
3. 写转换 prompt（例如*「同一个角色，赛博朋克装束，夜晚的天台」*）。
4. **运行**，即可基于你的参考图生成变体。

> **按文件名自动匹配角色（可选）：** 把参考图命名为 `dog.png`、`cat.png`、`duck.png`。当某条 prompt 提到*「dog playing with cat」*时，会自动调用 `dog.png` 和 `cat.png`。非常适合在一个系列里保持角色一致性。

### 5. 队列管理

- 在 **Prompt 队列** 里查看所有待处理任务。
- **移除**不再需要的任务，或 **停止**正在运行的批量任务。
- 实时追踪每条 prompt 的进度。

---

## ⚙️ 设置项说明

打开 **设置** 标签页来调整行为。

**常规**
- **默认模式** —— 每次打开面板时自动选中。
- **默认宽高比** —— 16:9、9:16 或 1:1。
- **每条 prompt 产出数** —— 每条 prompt 生成 1–4 个视频/图像。
- **并发 prompt 数** —— 同时跑 1–6 条 prompt。
- **prompt 间隔** —— 每条 prompt 之间等待 0–300 秒，减轻服务器压力。

**模型**
- **视频模型** —— 选择你的 VEO 模型（例如 VEO 3 / VEO 3 Fast）。
- **图像模型** —— 文生图和图生图均使用 Nano Banana。

**下载**
- **视频质量** —— 720p、1080p，或关闭。
- **图像质量** —— 1K、2K、4K，或关闭。
- 文件保存到 Chrome 的「下载」文件夹，每个项目一个子文件夹。

**高级**
- **最大重试次数** —— 失败时重试 1–20 次。
- **默认视频帧** —— 8 秒或 Concat 拼接。
- **每条 prompt 最大图片数** —— 按模式分别设置。
- **语言** —— 在 7 种语言之间切换界面。

---

## 💡 技巧与最佳实践

**写 prompt**
- 把主体、风格、镜头运动和光线写具体。
- 在 Google Flow 上，英文 prompt 往往最稳定。
- 每条 prompt 之间只用一个空行分隔。

**吞吐量 vs. 稳定性**
- 非高峰时段：约 3 条并发 prompt 效果不错。
- 高峰时段：降到 2 条并发，并把间隔提到约 30 秒——能减少「创建失败」的报错。
- 并发越高越快，但越不稳定；按需调到自己舒服的值。

**管理素材**
- 把参考图命名清晰，自动匹配才能正常工作。
- 坚持用 PNG / JPG / GIF，每张最好小于 10 MB。

**可靠性**
- 通宵无人值守的批量任务，记得开着 **自动重试**。
- 间隔越大 = 服务器负载越轻 = 失败越少。

---

## 🔧 常见问题排查

| 现象 | 原因与解决 |
| --- | --- |
| **扩展毫无反应** | 你必须停在 Google Flow 的**项目**页面上。确认扩展已启用，刷新页面，再重新打开面板。 |
| **「无法创建视频」** | Google Flow 暂时过载。别担心——扩展会每隔约 30 秒等待并重试，直到有空闲名额。 |
| **视频/图像下载不了** | 在 Chrome 里：**设置 → 下载内容 → 关闭** *「下载前询问每个文件的保存位置」*。然后在「设置」里重新检查下载质量。 |
| **「策略错误」** | 你的 prompt 或图片触发了 Google 的内容政策。工具会跳过该任务，自动处理下一条。 |
| **生成一直失败** | 检查网络连接，确认 prompt 有效，提高最大重试次数，并查看浏览器控制台找线索。 |
| **页面自己缩小了** | 这是有意为之——工具会调整缩放，以便精确定位按钮。批量任务运行期间请不要手动改缩放。 |
| **「正在被调试」横幅一直在** | 运行期间属于正常现象（见快速上手）。批量任务结束或你手动停止后它就会消失。 |

---

## ❓ FAQ

**VEO Automation 和 Google 有关联吗？**
没有。它是一款独立的第三方工具，用来自动化公开的 Google Flow 网页应用。它不隶属于 Google，也未获其背书或与之有任何关联。

**Nano Banana 是什么？**
Nano Banana 是 Google Flow 里提供的图像模型。VEO Automation 让你在同一个队列里批量生成并自动下载 Nano Banana 图像，和 VEO 3 视频一起跑。

**真的能一次生成上百个视频吗？**
可以。上传一份 prompt 的 `.txt` 文件（或粘贴一长串列表），队列会带自动重试地一条条处理。实际吞吐量取决于 Google Flow 的负载，以及你的并发数 / 间隔设置。

**它适合做竖屏短视频吗？**
适合——把宽高比设为 **9:16** 用于抖音 / Reels / Shorts，**16:9** 用于 YouTube，或 **1:1** 用于方形画面。

**我的文件会保存到哪里？**
保存到你 Chrome 的「下载」文件夹，按项目分到各自的子文件夹里，并自动重命名，方便整理。

**需要 API key 吗？**
不需要。它驱动的是你自己在浏览器里登录的 Google Flow 会话——无需单独的 API key 或开发者账号。

**我的数据会被发往别处吗？**
你的 prompt、图片和视频都在你的浏览器里、在 Google Flow 上处理。扩展只把设置存在本地。详见 [隐私与权限](#-隐私与权限)。

**支持哪些浏览器？**
Chrome 137+ 以及基于 Chromium 的浏览器（Edge、Brave）。需要支持侧边栏。

---

## 🔒 隐私与权限

- **在你的浏览器里运行。** 自动化发生在你自己的 Google Flow 会话中。
- **数据极少。** 设置存在 Chrome 本地存储里。扩展不会出售或抓取你的创作内容。
- **权限范围受限。** 主机访问仅限于 `labs.google/*`（用于自动化 Flow）以及扩展自有的后端（用于登录和额度）。
- **调试器权限** 仅用于向 Google Flow 发送可信的输入事件，这是页面所要求的——见 [快速上手](#-快速上手)。

完整说明：[https://github.com/amzbase-com/veo-automation-extension](https://github.com/amzbase-com/veo-automation-extension)

---

## 💳 定价

VEO Automation 采用 **freemium（免费增值）** 模式：

- **免费版** —— 每天重置的生成额度。适合试用和轻度使用。
- **Pro 版** —— 为跑大批量任务的重度用户提供更高或不限量的额度。

在侧边栏里登录即可查看你当前的额度。在 [https://github.com/amzbase-com/veo-automation-extension](https://github.com/amzbase-com/veo-automation-extension) 管理你的套餐。

---

## 🌐 链接

- **安装：** [Chrome 应用商店](https://chromewebstore.google.com/detail/veo-flow-automation-%E2%80%94-bat/inmkimakahiennggieafocbmfjlmfbhn?hl=zh)
- **官网：** [https://github.com/amzbase-com/veo-automation-extension](https://github.com/amzbase-com/veo-automation-extension)
- **Google Flow：** [labs.google/fx/tools/flow](https://labs.google/fx/tools/flow)

---

_免责声明：VEO Automation 是一个独立项目，**不**隶属于 Google 或 Google Flow 团队，也未获其背书或与之有任何关联。「VEO」「Nano Banana」「Google Flow」和「Google」均为 Google LLC 的商标。使用本工具须遵守 Google 的服务条款。_