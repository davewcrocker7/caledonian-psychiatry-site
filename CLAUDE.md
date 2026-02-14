# Caledonian Psychiatry Website

## Project Overview
- **Domain:** caledonianpsychiatry.co.uk
- **Company:** Edinburgh Psych Limited (trading as Caledonian Psychiatry)
- **Business:** Private psychiatric assessment and ongoing care for adults across Scotland (remote delivery)
- **Status:** ~95% complete, production-ready, password-gated (access code: HIS2026)

## Technology Stack
- **Type:** Static HTML/CSS/JavaScript (no backend, no frameworks)
- **Hosting:** GitHub Pages (CNAME configured)
- **Repo:** github.com/davewcrocker7/caledonian-psychiatry-site.git
- **Fonts:** Google Fonts — Cormorant Garamond (display), DM Sans (body)
- **No build tools** — no webpack, npm, or package manager

## Directory Structure
```
caledonian-psychiatry-site/
├── index.html              # Main homepage (1,153 lines)
├── about.html              # About Dr David Crocker (554 lines)
├── privacy.html            # Privacy notice (732 lines)
├── terms.html              # Terms of service (596 lines)
├── complaints.html         # Complaints policy (610 lines)
├── duty-of-candour.html    # Duty of candour statement (577 lines)
├── CNAME                   # GitHub Pages custom domain
├── README.md               # Project readme
└── assets/
    ├── hero.jpg             # Hero image (288K)
    ├── parallax.jpg         # Testimonial background (761K)
    ├── about.jpg            # Services section image (607K)
    ├── contact.jpg          # Contact section placeholder (817K)
    ├── david-headshot.jpg   # Professional headshot (809K)
    ├── david-personal.jpg   # Personal photo (1.2M)
    ├── david-portrait-bw.jpg # B&W portrait (9.1M — needs optimisation)
    ├── north-berwick-map.jpg # Contact section background (233K, zoom 15)
    ├── logo-hero.png        # Hero logo (218K)
    └── logo-mark.png        # Logo mark/favicon (52K)
```

## Design System
- **Colour palette:**
  - Navy: #1a2744 (primary)
  - Sage green: #6e9484 (accent)
  - Cream: #f8f6f1 (background)
  - Rust: #b8886f (secondary accent)
  - Dark grey: #2c2c2c (text)
- **Typography:** Cormorant Garamond (headings), DM Sans (body)
- **Breakpoints:** 968px (tablet), 600px (mobile), 380px (small mobile)

## Page Features
- **Password gate** on all pages (localStorage, code: HIS2026)
- **Sticky navbar** with scroll detection
- **Mobile hamburger menu** with dark overlay
- **Smooth scroll** navigation with fixed-nav offset
- **Fade-in animations** via Intersection Observer
- **Testimonial carousel** (5 quotes, auto-rotates every 5 seconds)
- **Contact form** via Web3Forms (async JS submission)
- **North Berwick map** as low-opacity background in contact section

## Contact Information
- **Email:** admin@caledonianpsychiatry.co.uk
- **Phone:** 07592 142000
- **Address:** The Lighthouse, Heugh Road, North Berwick, EH39 5PX
- **Hours:** Monday–Friday, 08:30–17:30

## Registrations
- **ICO:** ZB532461
- **GMC:** 7411382
- **HIS:** Application in progress

## Fees
| Service | Price | Duration |
|---------|-------|----------|
| ADHD assessment | £725 | 2 x 60 min |
| Autism assessment | £725 | 2 x 60 min |
| Combined ADHD & ASD | £1,200 | 3 x 60 min |
| General mental health | £325 | 60 min |
| Follow-up | £125 | 30 min |
| Prescriptions | £25 | each |

## Web3Forms (Contact Form)
- **Service:** Web3Forms (https://web3forms.com)
- **Access key:** `11211e1d-e6cf-4792-8ceb-fe1995e6b20b`
- **Sends to:** admin@caledonianpsychiatry.co.uk
- **Free tier:** 250 submissions/month
- **Form fields:** Name (required), email (required), phone (optional), message (required)
- **Layout:** Form on left column, contact details + emergency box on right
- **Dashboard:** https://web3forms.com (log in with admin@ email to manage)

## What's Not Yet Built
- Booking system / payment processing
- Analytics (no Google Analytics or similar)
- Image optimisation (especially david-portrait-bw.jpg at 9.1 MB)
- Blog / news section
- Proper favicon and SEO meta tags

## Development Notes
- All CSS is embedded in `<style>` tags within each HTML file (no external stylesheets)
- All JS is inline at bottom of each HTML file
- Styles are duplicated across pages — changes to shared elements (nav, footer, password gate) must be applied to all 6 HTML files
- No templating or includes — each page is fully self-contained
