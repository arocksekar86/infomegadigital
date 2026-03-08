# Infomega Digital Technologies - Static Website

A pixel-perfect static website for **Infomega Digital Technologies**, a full-service digital marketing and ecommerce agency. Generated from a WordPress (Astra + Elementor) backup using Playwright browser automation to capture the fully rendered pages.

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
├── css/                # All stylesheets (Astra theme, Elementor, plugins)
├── js/                 # All scripts (jQuery, Elementor, Swiper, WPForms, etc.)
├── assets/
│   ├── images/         # All images (logos, service graphics, client logos, testimonials)
│   └── fonts/          # Icon fonts (Elementor icons, Font Awesome)
├── .github/
│   └── workflows/
│       └── deploy.yml  # GitHub Pages deployment
└── README.md
```

## Features

- **Pixel-Perfect**: Captured from live WordPress using Playwright headless browser
- **SEO Optimized**: Semantic HTML5, meta tags, proper heading hierarchy
- **Fully Responsive**: Mobile, tablet, and desktop layouts via Astra & Elementor CSS
- **Interactive**: Elementor carousels, testimonial sliders, WhatsApp chat widget
- **All Assets Local**: Images, fonts, CSS, and JS served locally (no external dependencies except Google Fonts)
- **Clean Structure**: Organized into `css/`, `js/`, and `assets/` folders

## Tech Stack

- **HTML5** - Captured from WordPress Elementor rendering
- **CSS3** - Astra theme + Elementor styles + plugin styles
- **JavaScript** - jQuery, Elementor frontend, Swiper, WPForms, testimonial slider
- **Google Fonts** - Loaded from Google CDN

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

## Deployment

Automatically deployed to GitHub Pages via GitHub Actions on push to `master`.

## Source Data

This static site was generated from a WordPress backup containing:
- **Database**: MariaDB SQL dump (`u342552640_U3Z7B.sql`)
- **Files**: WordPress installation in `public_html/` (Astra theme + Elementor page builder)
- **Theme**: Astra 3.9.2 with Elementor 3.7.8
- **Method**: Playwright headless browser crawl of locally hosted WordPress instance

The original WordPress files are preserved in the `public_html/` directory alongside this static site.
