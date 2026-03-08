# Infomega Digital Technologies - Static Website

A lightweight static website for **Infomega Digital Technologies**, a full-service digital marketing and ecommerce agency. Converted from a WordPress (Astra + Elementor) backup into clean HTML/CSS/JS.

## Pages

| Page | File | Description |
|------|------|-------------|
| Home | `index.html` | Hero section, services overview, about us, clients, why choose us, testimonials, CTA |
| Services | `services.html` | 11 detailed service cards (SEO, Content Marketing, PPC, Social Media, etc.) |
| About | `about.html` | Company intro, core values, mission/vision, client testimonials |
| Contact | `contact.html` | Contact form, email, social links, quote request CTA |

## Project Structure

```
static-site/
├── index.html          # Homepage
├── services.html       # Services page
├── about.html          # About page
├── contact.html        # Contact page
├── css/
│   └── style.css       # All styles (responsive, mobile-first)
├── js/
│   └── main.js         # Navigation, animations, testimonial slider, form handling
├── assets/
│   ├── logo.svg        # White logo (for dark backgrounds / header)
│   └── logo-black.svg  # Dark logo (for light backgrounds)
└── README.md
```

## Features

- **SEO Optimized**: Semantic HTML5, meta tags, Open Graph, canonical URLs, proper heading hierarchy
- **Fully Responsive**: Mobile, tablet, and desktop layouts
- **No Dependencies**: Pure HTML/CSS/JS - no frameworks or build tools required
- **Performance**: Lightweight (~50KB total), no jQuery, minimal external resources
- **Accessible**: ARIA labels, keyboard navigation, semantic elements
- **Smooth Animations**: Intersection Observer scroll animations with graceful degradation
- **Testimonials Slider**: Auto-playing carousel with touch swipe support
- **Contact Form**: Client-side form with validation and success message

## Tech Stack

- **HTML5** - Semantic markup
- **CSS3** - Custom properties, Grid, Flexbox, media queries
- **Vanilla JavaScript** - No libraries or frameworks
- **Google Fonts** - Roboto, Roboto Slab

## How to Run

Simply open `index.html` in a browser, or serve with any static file server:

```bash
# Python
python -m http.server 8080

# Node.js
npx serve .

# PHP
php -S localhost:8080
```

## Color Palette

| Variable | Color | Usage |
|----------|-------|-------|
| `--primary` | `#01aef0` | Brand blue, buttons, links, accents |
| `--secondary` | `#1a1a2e` | Dark backgrounds, header, footer |
| `--accent` | `#61CE70` | Green highlights |
| `--text` | `#555` | Body text |
| `--heading` | `#1a1a2e` | Headings |

## Source Data

This static site was generated from a WordPress backup containing:
- **Database**: MariaDB SQL dump (`u342552640_U3Z7B.sql`)
- **Files**: WordPress installation in `public_html/` (Astra theme + Elementor page builder)
- **Theme**: Astra 3.9.2 with Elementor 3.7.8

The original WordPress files are preserved in the `public_html/` directory alongside this static site.
