# 🌸 Velmori Gifts

<p align="center">
  <img src="images/logo.png" alt="Velmori Gifts Logo" width="130" height="130" style="border-radius: 50%; border: 2.5px solid #c9a84c; box-shadow: 0 10px 30px rgba(0,0,0,0.12);"/>
</p>

<h3 align="center">Because every gift tells a story.</h3>

<p align="center">
  <em>Handcrafted gift hampers, eternal chenille bouquets & bespoke jewellery by Ruchita Tawade.</em>
</p>

<p align="center">
  <a href="https://khushisarda156.github.io/velmori-gifts/">
    <img src="https://img.shields.io/badge/Live_Site-GitHub_Pages-25D366?style=for-the-badge&logo=github&logoColor=white" alt="Live Demo" />
  </a>
  <img src="https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white" alt="HTML5" />
  <img src="https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white" alt="CSS3" />
  <img src="https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black" alt="JavaScript" />
</p>

---

## 🌐 Live Experience

**Live Website:** [https://khushisarda156.github.io/velmori-gifts/](https://khushisarda156.github.io/velmori-gifts/)

---

## ✨ Overview

**Velmori Gifts** is a single-page digital storefront engineered for artisanal luxury gifting. Crafted with love, the website offers a digital unboxing experience centered around an interactive, scroll-scrubbed floral backdrop, drifting blossom petals, and elegant glassmorphic cards.

Designed with vanilla web standards (Zero external runtime dependencies), the site loads instantly with 60fps GPU acceleration across mobile, tablet, and desktop viewports.

---

## ⚡ Engineering & Performance Highlights

* **3-Tier Keyframe Stride Scrubbing**:
  - **Tier 1 (Instant Paint <50ms)**: Preloads and decodes Frame 1 immediately in `<head>`, rendering the complete floral backdrop on the very first paint.
  - **Tier 2 (Keyframe Stride <300ms)**: Fetches an initial skeleton of keyframes across the entire scroll timeline (every 5th frame = 48 frames total). This guarantees 100% scroll scrubbing coverage from top to bottom in under half a second.
  - **Tier 3 (Background Streaming)**: Streams all remaining intermediate frames smoothly in parallel batches without blocking the main UI thread.
* **Nearest-Frame Fallback Interpolation**:
  - If a visitor quickly scrubs before a specific frame finishes downloading, `getClosestLoadedBitmap` instantly projects the nearest available keyframe, completely eliminating blank flashes or dropped frames.
* **GPU-Resident `ImageBitmap` & DPR Capping**:
  - Frames are pre-decoded into GPU-resident `ImageBitmap` primitives to prevent CPU-to-GPU transfer jank.
  - Canvas resolution is capped at `Math.min(devicePixelRatio, 1.5)` to ensure buttery 60fps compositing on Retina and mobile displays.
* **Pure Native Physics**:
  - Smooth passive scroll listener (`{ passive: true }`) synchronized to `requestAnimationFrame`. Zero heavy external scroll libraries or DOM bloat.
* **Floating Petals Engine**:
  - Lightweight canvas animation featuring drifting cherry-blossom petals with subtle natural oscillation and randomized opacity.

---

## 🎨 Luxury Design System

Curated for an artisanal, romantic, and warm editorial aesthetic:

| Token | CSS Variable | Hex Code | Purpose |
| :--- | :--- | :--- | :--- |
| **Cream** | `--cream` | `#fdf8f5` | Base page background & warm ivory canvas fill |
| **Blush** | `--blush` | `#f7ded4` | Soft floral highlights & ambient glow tints |
| **Gold** | `--gold` | `#a57c65` | Luxury borders, section badges & dividers |
| **Rose** | `--rose` | `#b56070` | Headline italic emphasis & review names |
| **Dark Espresso** | `--dark` | `#2c1d1d` | High-contrast WCAG AA display typography |
| **Muted Taupe** | `--dark-muted` | `#574343` | Body copy, product descriptions & metadata |

### Typography
- **Headings & Badges**: `Cinzel` & `Cormorant Garamond` (classic roman & italic serifs).
- **Body & Captions**: `Lato` (clean, accessible geometric sans).

---

## 🛍️ Featured Collections

1. **Birthday Hampers**: Bespoke gift boxes curated with custom accessories, premium chocolates, and artisanal floral toppings.
2. **Apology Hampers**: Thoughtfully assembled "I'm Sorry" keepsake hampers featuring scrunchies, satin bows, and personalized heartfelt tags.
3. **Pipe Cleaner Bouquets**: Handcrafted chenille rose arrangements designed to never wilt or fade.

---

## 📁 Repository Structure

```
velmori-gifts/
├── index.html        # Complete standalone application (HTML, CSS, JS engine)
├── sitemap.xml       # Search engine crawler index
├── robots.txt        # Crawler permission policy
├── build.md          # Technical architectural specification & build guide
├── README.md         # Documentation & project overview
├── images/           # Brand assets & high-resolution product photography
│   ├── logo.png
│   ├── birthday_hamper.jpeg
│   ├── apology_hamper.jpeg
│   └── bouque_pipe_cleaner.jpeg
└── frames/           # 240 compressed JPEG frames for scroll animation
```

---

## 🚀 Local Development

1. **Clone the repository**:
   ```bash
   git clone https://github.com/KhushiSarda156/velmori-gifts.git
   cd velmori-gifts
   ```

2. **Run locally**:
   - Open `index.html` directly in your browser, or launch with any local static server:
   ```bash
   # Using Python 3
   python -m http.server 8000
   
   # Or using Node
   npx serve .
   ```

3. **Visit in browser**:
   Navigate to `http://localhost:8000`.

---

## 💌 Orders & Inquiries

Every gift is personally curated and handcrafted by founder **Ruchita Tawade**.

- **WhatsApp**: [+91 93566 64679](https://wa.me/919356664679?text=Hi%20Ruchita!%20I%20saw%20Velmori%20Gifts%20and%20I'd%20love%20to%20place%20an%20order%20%F0%9F%8E%81)
- **Call**: `+91 93566 64679`

---

## 📄 License

MIT &copy; 2026 Velmori Gifts by Ruchita Tawade. Crafted with love.