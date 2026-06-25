# 🌿 Freshie — Eat Fresh, At Your Doorstep

A fully responsive e-commerce website for **Freshie**, a Nairobi-based farm-fresh produce delivery brand. Built as a single-file HTML application with vanilla JavaScript — no frameworks, no build tools, no dependencies beyond a Google Fonts import.

---

## 🚀 Live Preview

Open `freshie.html` directly in any modern browser — no server required.

---

## 📁 Project Structure

```
freshie/
├── freshie.html      # Entire application — HTML, CSS & JS in one file
├── README.md         # Project documentation (this file)
└── .gitignore        # Files and folders excluded from version control
```

---

## ✨ Features

### 🛍️ Shop
- **Tabbed product categories** — Fruits, Vegetables, and Smoothies each in their own tab
- **SVG product illustrations** — Hand-drawn vector artwork for every fruit, vegetable, and smoothie cup
- **Smoothie cups** — Each blend rendered as a realistic branded cup with lid, straw, and coloured liquid fill

### 🛒 Cart System
- Add items from any tab with animated button feedback
- Floating cart button with live item count badge
- **Slide-in cart drawer** with full item list
- Quantity controls (increase / decrease per item)
- Per-item removal
- **Free delivery** automatically applied on orders over KES 2,000
- Clear cart with one click

### 💳 Checkout Flow
- Full checkout modal with form validation
- Payment method selector: M-Pesa, Card, or Cash on Delivery
- Kenyan phone number format validation (`07XXXXXXXX`)
- Live order summary with delivery fee calculation
- Order confirmation screen with estimated 2-hour delivery

### 📱 UX & Polish
- Fixed navbar with smooth-scroll navigation
- Active nav link highlights as you scroll through sections
- Mobile-responsive hamburger menu
- Scroll-reveal animations on cards entering the viewport
- Toast notifications for cart actions
- Newsletter sign-up bar (appears after 5 seconds, dismisses per session)
- ESC key closes cart drawer or checkout modal

### 🎨 Brand
| Token | Value |
|---|---|
| Fresh Green | `#22C55E` |
| Dark Green | `#16A34A` |
| Deep Green | `#14532D` |
| Vibrant Orange | `#F97316` |
| Light Cream | `#FFF8E6` |
| Dark Gray | `#333333` |
| Font | Poppins (Google Fonts) |

---

## 🏗️ Sections

| Section | Description |
|---|---|
| **Hero** | Headline, stats, CTA buttons, floating badges |
| **Features Strip** | Fresh Quality · Fast Delivery · Healthy Choices · Nairobi-wide |
| **Shop** | Tabbed: Fruits / Vegetables / Smoothies |
| **How It Works** | 4-step order process |
| **Testimonials** | 3 customer reviews |
| **App Download** | Dual phone mockups, App Store & Play Store CTAs |
| **Footer** | Links, contact details, social icons |

---

## 🛠️ Getting Started

### Run locally

```bash
# Clone the repo
git clone https://github.com/your-username/freshie.git
cd freshie

# Open in browser (macOS)
open freshie.html

# Open in browser (Linux)
xdg-open freshie.html

# Open in browser (Windows)
start freshie.html
```

No package installs, no build step. It just works.

### Deploy to GitHub Pages

1. Push the repo to GitHub
2. Go to **Settings → Pages**
3. Set source to the `main` branch, root folder `/`
4. GitHub Pages will serve `freshie.html` automatically

### Deploy to Netlify / Vercel

Drag and drop the project folder into [netlify.com/drop](https://netlify.com/drop) — live in seconds.

---

## 🧩 Extending the Project

### Adding a new product

In `freshie.html`, find the relevant tab panel (`#tab-fruits`, `#tab-vegetables`, or `#tab-smoothies`) and copy an existing `.product-card` block. Update the SVG illustration, product name, description, price, and `addToCart(this, 'Product Name', price)` values.

Also register the new item in the `PRODUCTS` object in the `<script>` section:

```js
const PRODUCTS = {
  // ...existing items
  'New Product': { price: 200, emoji: '🍑' },
};
```

### Adding a new smoothie

Copy an existing `.smoothie-card-new` block inside `#tab-smoothies`. Swap the liquid fill colour in the SVG (`fill="#YOURCOLOR"`), update the straw colour, and adjust the `addToCart` call.

### Changing prices

Update both the display text (`KES XXX`) in the HTML card and the corresponding price in the `PRODUCTS` object to keep the cart totals accurate.

---

## 📦 Dependencies

| Dependency | Version | Purpose |
|---|---|---|
| [Poppins](https://fonts.google.com/specimen/Poppins) | via Google Fonts CDN | Brand typography |

No npm packages. No frameworks. No bundler.

---

## 🌍 Business Info

| | |
|---|---|
| **Brand** | Freshie Kenya |
| **Tagline** | *Eat fresh, at your doorstep* |
| **Location** | Nairobi, Kenya |
| **Phone** | 0712 345 678 |
| **Website** | www.freshie.co.ke |
| **Instagram** | @eatfreshiefresh |

---

## 📄 License

This project is proprietary to **Freshie Kenya**. All rights reserved.

---

> *Thank you for choosing fresh!* 🌿
