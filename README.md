<div align="center">

# 📱 Apple Details Showcase

### Interactive Multi-Layer Product Showcase Powered by Cutting-Edge Modern CSS & JavaScript

[![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)](https://developer.mozilla.org/en-US/docs/Web/HTML)
[![CSS3](https://img.shields.io/badge/Modern_CSS-1572B6?style=for-the-badge&logo=css3&logoColor=white)](https://developer.mozilla.org/en-US/docs/Web/CSS)
[![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)](https://developer.mozilla.org/en-US/docs/Web/JavaScript)
[![GSAP](https://img.shields.io/badge/GSAP-88CE02?style=for-the-badge&logo=greensock&logoColor=white)](https://gsap.com/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg?style=for-the-badge)](LICENSE)

<br />

<p align="center">
  <b>A sleek, Apple-inspired interactive product feature showcase combining exclusive native disclosures with spring-physics motion and synchronized multi-layered device visual reveals.</b>
</p>

[✨ Live Preview](#-getting-started) • [🎯 Key Features](#-key-features) • [🧠 Under the Hood](#-under-the-hood-modern-web-features) • [📂 Project Structure](#-project-structure) • [🚀 Getting Started](#-getting-started)

</div>

---

## 🌟 Overview

The **Apple Details Showcase** is an experimental demonstration of cutting-edge web platform capabilities. It replicates the high-end, tactile interaction design of Apple product feature pages without relying on bloated libraries or complex height-calculation workarounds.

When a feature item is clicked, the accordion smoothly transitions its dimensions while triggering synchronized 3D perspective shifts, exploded internal views, close-up camera angles, and parallax depth effects on the device canvas.

---

## 🎯 Key Features

- 📑 **Exclusive Native Accordion**: Leverages standard `<details name="feature">` where opening one automatically closes any other disclosure element without custom JS state management.
- 📐 **Zero-Hack Smooth Height Transitions**: Uses `interpolate-size: allow-keywords` and the `::details-content` pseudo-element to animate seamlessly between fixed heights and intrinsic `fit-content`.
- 🪀 **Spring Physics Easing**: Replicates authentic mechanical spring bounces using the CSS `linear(...)` easing function.
- 🎨 **Responsive Multi-Layer Imagery**: Dynamic layering with CSS Container Queries (`cqi` / `cqw`) and `:has()` relational selectors to synchronize product angles with selected features.
- 🌓 **Dynamic Theme Switching**: Supports system, light, and dark modes powered by CSS `light-dark()` with fluid visual morphing via `document.startViewTransition()`.
- 🎛️ **Interactive Dev Controls**: Built-in Draggable [Tweakpane](https://tweakpane.github.io/) panel allowing real-time theme swapping, debug layout outlines, and animation resets.
- ♿ **Accessible by Default**: Fully accessible semantic HTML, keyboard navigable with dynamic `aria-hidden` and `tabindex` state synchronization.

---

## 🧠 Under the Hood: Modern Web Features

| Web Standard | Implementation | What It Solves |
| :--- | :--- | :--- |
| **`interpolate-size`** | `interpolate-size: allow-keywords;` | Solves the decades-old CSS limitation of animating to `height: auto` or `fit-content`. |
| **`::details-content`** | `details::details-content` | Directly targets and animates the internal disclosure container without wrapper hacks. |
| **`linear()` Easing** | `linear(0 0%, 0.4214 6.61%, ...)` | Generates complex multi-stop spring curves natively in CSS without needing external physics engines. |
| **`:has()` Selector** | `section:has(details:nth-of-type(n)[open])` | Enables relational parent-to-child styling to coordinate image states with active accordion items. |
| **Container Queries** | `width: 100cqi; width: 100cqw;` | Sizes image layers fluidly relative to the parent card container rather than the viewport. |
| **View Transitions API** | `document.startViewTransition()` | Creates smooth cross-fades when switching color palettes and themes. |
| **Web Animations API** | `section.getAnimations({ subtree: true })` | Monitors running CSS animations to prevent race conditions during rapid user clicks. |

---

## 📂 Project Structure

```text
Apple-details-showcase/
├── 📄 index.html          # Semantic markup with exclusive details, summary, and action controls
├── 🎨 index.css           # Modern layered CSS (@layer base, demo, images, controls, debug, intro)
├── ⚡ index.js            # GSAP draggable integration, Tweakpane controls, & animation orchestration
├── 🛡️ .gitignore          # Ignores system files and local environments
└── 📖 README.md           # Project documentation and guide
```

---

## 🚀 Getting Started

No heavy build steps or package managers are required. All external dependencies (GSAP & Tweakpane) load via modern ES Modules from CDNs.

### 1️⃣ Clone the Repository

```bash
git clone https://github.com/pabitralenka07/Apple-details-showcase.git
cd Apple-details-showcase
```

### 2️⃣ Run with Any Local Server

Because this project utilizes ES Modules (`<script type="module">`), run it through a local HTTP server:

```bash
# Option A: Using npx serve
npx serve .

# Option B: Using Python 3
python3 -m http.server 8000

# Option C: Using Node.js http-server
npx http-server -p 8000 -c-1
```

### 3️⃣ View in Browser

Open your browser and navigate to:
```text
http://localhost:8000
```

> [!TIP]
> For the best visual experience, use a modern browser that supports CSS `interpolate-size` and `::details-content` (Chrome 129+, Edge 129+, or Safari Technology Preview).

---

## 🕹️ Interactive Controls

- **Click any feature**: Watch the smooth height expansion and phone layer reveal.
- **Next / Previous arrows**: Cycle through features sequentially.
- **Exit button (X)**: Collapse back to the default overview state.
- **Tweakpane Config Panel**:
  - Drag the header to reposition anywhere on screen.
  - Double-click the panel header to snap it back to origin.
  - Toggle **Debug** mode to visualize bounding boxes and layer outlines.
  - Toggle **Theme** (System, Light, Dark) with View Transitions.

---

## 🤝 Contributing

Contributions, issues, and feature requests are welcome!

1. Fork the Project
2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3. Commit your Changes (`git commit -m 'feat: add some AmazingFeature'`)
4. Push to the Branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

---

## 📜 License

Distributed under the MIT License. See `LICENSE` for more information.

---

<div align="center">

Made with ❤️ by [Pabitra Lenka](https://github.com/pabitralenka07)

⭐ If you found this project helpful or inspiring, consider giving it a star!

</div>
