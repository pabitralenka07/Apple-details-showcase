# Apple Details Showcase

An interactive Apple-style product detail feature showcase built with modern web platform standards. It pairs a native exclusive accordion on the left with synchronized multi-layered device artwork animations on the right (close-up, exploded breakdown, parallax angle, and camera lens details).

## 🚀 Key Features

- **Exclusive Accordion**: Uses HTML5 `<details name="feature">` to natively group disclosures so opening one automatically closes the rest without JavaScript state synchronization.
- **Native Height Animation**: Uses `interpolate-size: allow-keywords` and `::details-content` to smoothly animate between fixed and intrinsic content heights (`fit-content`).
- **CSS Spring Physics**: Uses the modern `linear(...)` easing function for realistic bounce dynamics.
- **Relational Styling with `:has()`**: Dynamically updates phone visual layers based on the active disclosure item.
- **Theme & View Transitions**: Supports light and dark modes with `light-dark()` and smooth visual crossfades via `document.startViewTransition()`.
- **Tweakpane & Draggable**: Interactive runtime configuration panel powered by Tweakpane and GSAP Draggable.

## 🛠️ Tech Stack

- **HTML5**: Native semantic elements (`<details>`, `<summary>`)
- **Modern CSS**: CSS `@layer`, Container Queries (`cqi`/`cqw`), `color-mix()`, `light-dark()`, discrete transitions
- **JavaScript**: GSAP, Tweakpane, Web Animations API

## 💻 Getting Started

You can run this project with any local HTTP static server:

```bash
# Using npx serve
npx serve .

# Or using Python's built-in server
python3 -m http.server 8000
```

Then navigate to `http://localhost:8000` or the port indicated in your terminal.
