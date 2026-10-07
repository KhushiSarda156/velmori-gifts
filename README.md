# 🌸 Velmori Gifts

<p align="center">
  <img src="images/logo.png" alt="Velmori Gifts Logo" width="150" height="150" style="border-radius: 50%; border: 3px solid #c9a84c; box-shadow: 0 8px 24px rgba(0,0,0,0.15);"/>
</p>

<h3 align="center">Because every gift tells a story.</h3>

<p align="center">
  <img src="https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white" alt="HTML5" />
  <img src="https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white" alt="CSS3" />
  <img src="https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black" alt="JavaScript" />
  <img src="https://img.shields.io/badge/Netlify-00C8B5?style=for-the-badge&logo=netlify&logoColor=white" alt="Netlify" />
</p>

---

## ✨ Overview

**Velmori Gifts** is a premium, highly-interactive, single-page landing experience designed to showcase custom gift hampers, everlasting pipe-cleaner bouquets, and artisanal jewellery sets handcrafted by Ruchita Tawade. 

The website offers a luxury digital unboxing experience through smooth physics-based scrolling, canvas animations, and a GPU-accelerated scroll-driven background animation.

---

## 🎨 Premium Features

*   **GPU-Accelerated Scroll Animation**: A gorgeous background frame-by-frame animation mapped dynamically to the user's scroll progress, decoded via GPU `ImageBitmap` for 60fps jank-free rendering.
*   **Progressive Asset Loading**: The 240-frame animation load sequence is split dynamically: the first 10 frames load instantly so the user can interact immediately, while the rest are lazy loaded sequentially during browser idle times.
*   **Lenis Smooth Scrolling**: Smooth, momentum-based scrolling that mimics high-end web experiences.
*   **Artisanal Ripple Trail**: A soft blush-gold expanding ripple trail following the cursor, utilizing a high-performance 40-element DOM object pool to keep memory overhead at zero.
*   **Petal Drift Canvas**: An elegant canvas overlay rendering delicate, randomly drifting cherry-blossom petals.
*   **Responsive Luxury Layout**: Tailored layouts for desktop, tablet, and mobile with curated typography and glassmorphism UI components.
*   **Seamless Ordering Integration**: Straightforward, pre-formatted WhatsApp call-to-actions to connect customers directly to the founder for custom commissions.

---

## 🚀 Performance & Google Friendliness (SEO)

We designed this site with modern web standards, making it load lightning-fast and search engine friendly:

*   **Google Font Preconnecting**: Speeds up text rendering times by establishing early connections to font origins.
*   **Resource Lazy Loading**: Product images and testimonials below the fold use native `loading="lazy"` and `decoding="async"` tags.
*   **Perfect Open Graph Metadata**: Comprehensive Open Graph and Twitter Card tags to ensure link sharing on WhatsApp, Telegram, or Facebook displays a beautiful branded preview card.
*   **Canonical Linking**: Prevents search engine indexing conflicts by explicitly setting the canonical tag as the primary address.
*   **Sitemap & Robots**: Full crawler guidance via custom `sitemap.xml` and `robots.txt` configuration files.

---

## 🎨 Design System

Our brand palette reflects warmth, luxury, and hand-curated love.

| Token | CSS Variable | Color Preview | Value | Primary Usage |
| :--- | :--- | :--- | :--- | :--- |
| **Blush** | `--blush` | <img src="https://via.placeholder.com/15/f5d5c8/000000?text=+" width="15" height="15" /> | `#F5D5C8` | Accent backgrounds & subtle highlights |
| **Cream** | `--cream` | <img src="https://via.placeholder.com/15/fdf6f0/000000?text=+" width="15" height="15" /> | `#FDF6F0` | Main section background (warm ivory) |
| **Gold** | `--gold` | <img src="https://via.placeholder.com/15/a57c65/000000?text=+" width="15" height="15" /> | `#A57C65` | Borders, brand badge outlines, labels |
| **Rose** | `--rose` | <img src="https://via.placeholder.com/15/b56070/000000?text=+" width="15" height="15" /> | `#B56070` | Secondary CTA accents & italic texts |
| **Dark** | `--dark` | <img src="https://via.placeholder.com/15/3d2b2b/000000?text=+" width="15" height="15" /> | `#3D2B2B` | Core typography and dark layouts |

---

## 🛠️ Codebase Structure

```
velmori-gifts/
├── index.html        # Main landing page (Structure, Styles, and JS)
├── sitemap.xml       # Google crawler index map
├── robots.txt        # Crawler permissions
├── images/           # Product photography, logo and assets
│   ├── logo.png
│   ├── birthday_hamper.jpeg
│   ├── apology_hamper.jpeg
│   └── bouque_pipe_cleaner.jpeg
└── frames/           # 240 compressed JPEG frames for the scroll-scrub
```

---

## 📦 Getting Started & Customization

### Run Locally

1. **Clone the Repo**:
   ```bash
   git clone https://github.com/khushisarda261099-design/velmori-gifts.git
   ```
2. **Open index.html**:
   Double click `index.html` to open it in any web browser, or serve it via a local environment (like VS Code Live Server).

### Editing Content
- **To update prices or products**: Open `index.html` and search for `<section class="products">`.
- **To change the animation speed or behavior**: Modify the values inside the `<script>` tag at the bottom of `index.html`.

---

## ✉️ Licensing & Contact

- **Founder**: Ruchita Tawade  
- **Contact Number**: `+91 93566 64679`
- **Code License**: MIT. Created with love. Feel free to remix and modify!