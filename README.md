# Fibrix Broadband - Website

Official website for **[fibrixllp.org](https://fibrixllp.org)** - Fibrix Broadband, a broadband internet, IPTV, and networking hardware provider based in Joynagar Mojilpur, South 24 Parganas, West Bengal.

**Fibrix Broadband** is the brand name of **Fibrix LLP** (LLP ID: ACT-8822).

## Pages

| Page | File | Description |
|------|------|-------------|
| Home | `index.html` | Hero, services, broadband plans (4 duration tabs), OTT platforms, IPTV packages, hardware catalog, CTA |
| About Us | `about.html` | Company info, team, mission ("Internet for All"), vision, values |
| Contact Us | `contact.html` | Contact form (Google Form integration) & company details |
| Privacy Policy | `privacy-policy.html` | Data collection, usage, and privacy practices |
| Terms & Conditions | `terms.html` | Service terms for broadband & hardware |
| Refund Policy | `refund-policy.html` | Refund & cancellation for services & hardware |

## Broadband Plans

Plans are available in **Monthly**, **Quarterly (90 days)**, **Half-Yearly (180 days)**, and **Yearly (365 days)** durations with tabbed UI.

### Monthly Plans

| Plan | Speed | Price (incl. GST) |
|------|-------|--------------------|
| Connect 40 | 40 Mbps | ₹330/mo |
| Family 60 | 60 Mbps | ₹430/mo |
| Power 80 (Most Popular) | 80 Mbps | ₹530/mo |
| Turbo 100 | 100 Mbps | ₹600/mo |
| OTT + 30 | 30 Mbps | ₹550/mo |
| OTT + 60 | 60 Mbps | ₹650/mo |
| OTT + 80 | 80 Mbps | ₹750/mo |
| OTT + 100 | 100 Mbps | ₹820/mo |

Additional quarterly, half-yearly, and yearly pricing available on the website.

## IPTV Packages

| Package | Channels | Price (incl. GST) |
|---------|----------|--------------------|
| HD | 49 | ₹90/mo |
| HD+ | 56 | ₹120/mo |
| ACE HD | 74 | ₹150/mo |
| AXEL HD (Popular) | 95 | ₹200/mo |

Each package is available in 4 regional variants: Hindi, Marathi, Gujarati & Bangla. Channel lists are grouped by category (Entertainment, Movies, Kids, Sports, Infotainment, News, etc.) with expandable dropdowns. Channel data sourced from `iptvchannel.csv`.

### Channel Search

A search bar above the IPTV cards lets users find any channel and see which packs include it. Typing a channel name (min 2 chars) displays a results table with ✓/✗ availability across all 4 packages, helping users decide which pack to choose.

## OTT Platforms

Included with select broadband plans:

- **Premium OTT Pack** — 29 platforms
- **Prime Plus OTT Pack** — 27 platforms

## Networking Hardware

Listed as a catalog (no e-commerce): Routers & Switches, ONU/ONT Devices, GPON/EPON OLT, Fiber Optic Cables, Patch Cords & Connectors, Set-Top Boxes.

## Logos

- **Header / Favicon:** `Fibrix Logo Style 1.png`
- **Footer:** `Fibrix Logo Style 2.png`

## Contact Form

The contact form submits to a Google Form via `fetch` (no-cors POST). Entry IDs:

| Website Field | Google Form Entry ID |
|---------------|----------------------|
| First Name | `entry.1423676904` |
| Last Name | `entry.1657985535` |
| Email Address | `entry.291522330` |
| Phone Number | `entry.350177398` |
| Subject | `entry.1065936945` |
| Message | `entry.1467988090` |

## Payment Portal

Bill payments are handled externally at **[pay.fibrixllp.org](https://pay.fibrixllp.org/customer_portal)**.

## UI Features

- **Collapsible header** — hides on scroll down, shows on scroll up (all pages, all screen sizes)
- **Navigation** — Home, IPTV, OTT, About Us, Contact Us, Pay Bill (IPTV & OTT link to homepage anchors from other pages)
- **Plan duration tabs** — pill-style Monthly / Quarterly / Half-Yearly / Yearly switcher
- **OTT platform tabs** — Premium / Prime Plus toggle with text-only grid
- **IPTV expandable cards** — "View Channel List" button reveals categorised channel grid per package
- **IPTV channel search** — real-time search bar to look up any channel across all 4 packs with ✓/✗ availability table
- **Hardware list cards** — numbered cards with red accent border, no images
- **WhatsApp integration** — floating chat button on all pages
- **Mobile-first responsive** — hamburger nav, stacked grids, optimised touch targets

## Hosting & Deployment

Hosted on **GitHub Pages** with a custom domain.

- **Repository:** `shourjo-h/fibrixllp.github.io`
- **Branch:** `main`
- **Custom domain:** `fibrixllp.org`
- **CNAME file:** included

### DNS Configuration

**A Records** (for fibrixllp.org):
```
185.199.108.153
185.199.109.153
185.199.110.153
185.199.111.153
```

**CNAME** (for www):
```
www -> shourjo-h.github.io
```

## SEO

- `robots.txt` — allows all crawlers, points to sitemap
- `sitemap.xml` — all 6 pages with priorities
- Open Graph meta tags on all pages for social sharing previews

## Customisation

- **Broadband plans & pricing:** Edit plan cards in `index.html` (inside `.plan-tab-content` divs)
- **IPTV packages:** Edit IPTV cards in `index.html` (inside `#iptv` section); update `iptvchannel.csv` for reference
- **Brand color:** `#c11111` — edit CSS variables in `css/style.css`
- **Contact form:** Update Google Form entry IDs in `contact.html` if form fields change

## Tech Stack

- Pure HTML5 + CSS3 + vanilla JavaScript
- Google Fonts (Inter, weights 400–800)
- GitHub Pages hosting
- Google Forms backend for contact form

## Team

- **Papia Banerjee** — Partner
- **Jibesh Mahato** — Partner
