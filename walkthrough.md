# Sanaya Store — Build Walkthrough ✅

## What Was Built

A full cinematic luxury single-page application for Sanaya Store (Sanaya JSR), Jamshedpur.

---

## File Structure

```
c:\Users\ASLAM\ASHH\
├── index.html              63 KB  ← Master SPA (13 sections)
├── css/
│   └── styles.css          51 KB  ← Full luxury design system
├── js/
│   ├── main.js             15 KB  ← Core interactions
│   ├── particles.js         4 KB  ← Gold dust canvas engine
│   ├── quiz.js              9 KB  ← AI Style Quiz + Ring Calculator
│   └── ticker.js            4 KB  ← Live rates + Toast notifications
└── assets/images/
    ├── hero_necklace.png   625 KB  ← Hero background (AI generated)
    ├── artisan_craft.png   810 KB  ← Brand story section
    ├── luxury_packaging.png 701 KB ← (Available for use)
    ├── high_jewellery.png  818 KB  ← High Jewellery tab
    ├── genz_jewellery.png 1051 KB  ← GenZ Aesthetic tab + Gallery
    └── ocean_jewellery.png 813 KB  ← Ocean & Shell tab + Gallery
```

---

## 13 Sections Built

| # | Section | Key Features |
|---|---------|-------------|
| 1 | **Scroll Progress** | Animated gold gradient bar |
| 2 | **Navigation** | Glass morphism sticky nav, mobile overlay menu |
| 3 | **Cinematic Hero** | SVG mandala, typewriter taglines, gold dust particles, floating orb |
| 4 | **Gold Rate Ticker** | Simulated live 22K/24K/Silver/Platinum/18K rates with live flash |
| 5 | **Brand Story** | Animated counters, split editorial layout with artisan image |
| 6 | **Lookbook Catalog** | 6 tabs, 18 product cards with magnetic 3D tilt, quick-view modal, WhatsApp links |
| 7 | **Craft Timeline** | 5-step horizontal artisan process with floating icons |
| 8 | **Innovation Lab** | Virtual Try-On mockup + 4-step AI Style Quiz |
| 9 | **Unboxing Luxury** | 3D CSS box lid animation, packaging feature list |
| 10 | **GenZ Gallery** | Masonry-style photo grid with hover overlays |
| 11 | **Social Proof** | 3 testimonials, press row, auto social proof toast notifications |
| 12 | **Commission CTA** | Full-width bespoke order section with WhatsApp + email |
| 13 | **Footer** | Newsletter, 4-column links, social icons |

---

## Signature Features

### 🟡 Gold Dust Particles
Canvas engine with 120 particles (50 on mobile). Particles drift upward and are gently attracted to your mouse cursor. Nearby particles draw constellation lines.

### 🎯 Custom Golden Cursor
A dot + ring cursor that smoothly follows mouse with lag (ring lags behind dot for a premium feel). Ring expands on hover over interactive elements.

### 🧲 Magnetic Product Cards
Cards tilt in 3D space relative to mouse position using CSS `perspective`. Cards straighten when mouse leaves.

### 🤖 AI Style Quiz
4-question quiz with tag-based scoring system. Selects your "Jewellery Mood" from 5 archetypes: Grand Bride, Haute Connoisseur, Aesthetic Maven, Artisan Soul, Coastal Dream.

### 📊 Live Gold Ticker
Simulated rates with random drift every 8 seconds. Shows ▲▼ directional change indicators in green/red.

### 🔔 Social Proof Toasts
Auto-triggered purchase notifications starting at 4s, then every 9s. 10 different products with cities across India.

### 📐 Ring Size Calculator
India / US / mm lookup chart for sizes 5–16. Shows result panel with WhatsApp link for unsure customers.

### 📱 Concierge Sidebar
Right-edge floating buttons open a slide-in panel with ring calculator, quick action buttons, and studio address.

---

## Customisation Guide

### Change WhatsApp Number
Replace `919876543210` throughout `index.html` and `quiz.js` with your actual number.

### Change Business Info
- Name: "Sanaya Store" / "Sanaya JSR"
- Location: "Jamshedpur, Jharkhand"
- Email: `hello@sanayastore.com`
- Instagram: `@sanaya.jsr`

### Add More Products
Copy any `<article class="product-card">` block inside a `catalog-grid` div. Update the name, sub-text, price, and WhatsApp message.

### Update Gold Rates (Base)
Edit `BASE_RATES` in `js/ticker.js`:
```js
const BASE_RATES = {
  gold22k: { price: 6480, unit: '/gm', label: '22K Gold' },
  ...
};
```

---

> [!TIP]
> For best visual experience, open in Chrome or Edge. The site works fully offline — just double-click `index.html`.

> [!NOTE]
> The browser preview tool had an installation issue. Simply open `c:\Users\ASLAM\ASHH\index.html` in your browser to see the full experience.
