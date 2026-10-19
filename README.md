<div align="center">

# NEX**ORA**

### A modern, responsive website for a digital design & engineering studio

Dark glass UI · Teal-to-violet palette · 10 responsive pages · No build step

[![Live Demo](https://img.shields.io/badge/Live_Demo-View_Site-45e0c9?style=for-the-badge&logo=githubpages&logoColor=070a14&labelColor=070a14)](https://pashtanahabib.github.io/NEXORA/)
[![HTML5](https://img.shields.io/badge/HTML5-070a14?style=for-the-badge&logo=html5&logoColor=45e0c9)](#-tech-stack)
[![CSS3](https://img.shields.io/badge/CSS3-070a14?style=for-the-badge&logo=css3&logoColor=8b6cf6)](#-tech-stack)
[![Bootstrap 5](https://img.shields.io/badge/Bootstrap_5.3-070a14?style=for-the-badge&logo=bootstrap&logoColor=8b6cf6)](#-bootstrap--javascript)

</div>

---

## 🌐 Live Demo

> **👉 [https://pashtanahabib.github.io/NEXORA/](https://pashtanahabib.github.io/NEXORA/)**

---

## ✨ About

**Nexora** is a complete multi-page agency website template. It pairs a dark, glassmorphism-inspired interface with a restrained teal and violet palette, subtle film-grain backgrounds and confident display typography. It is written in plain HTML and CSS on top of Bootstrap 5, with **no custom JavaScript**. Everything interactive comes from Bootstrap's own components.

## 📄 Pages

| Page | What's inside |
|------|---------------|
| `index.html` | Hero with live-metrics card, case-study carousel, services, about teaser, featured projects, testimonials, pricing preview, FAQ, CTA |
| `services.html` | Detailed service offerings |
| `about.html` | Studio story, values, numbers and skill progress bars |
| `portfolio.html` | Filterable project gallery with detail modals |
| `team.html` | Team member cards |
| `pricing.html` | Pricing plans |
| `blog.html` | Article grid with pagination |
| `blog-details.html` | Single article layout |
| `contact.html` | Contact form and details |
| `404.html` | Custom not-found page |

---

## 🎨 Design & Visual Effects

### Glassmorphism
Translucent surfaces with a soft border and `backdrop-filter: blur()` are used for cards, the stats panel, the navbar and the carousel controls. There are two strengths: `.glass` for normal surfaces and `.glass-strong` for highlighted ones, such as the "Most Popular" pricing card.

### Atmospheric backgrounds
The backgrounds are made only with CSS and one inline SVG, with no image files:
- **Film grain**: a fixed full-page SVG `feTurbulence` noise layer blended with `mix-blend-mode: overlay`. It removes the flat, digital look of plain gradients.
- **Editorial column guides**: hairline vertical lines on hero sections, faded out with a `mask-image` gradient.
- **Soft light washes**: two off-axis radial gradients per hero instead of floating blurred blobs.
- **Textured slide art**: the carousel and the placeholder frames use three CSS textures: diagonal hatching (`repeating-linear-gradient`), a halftone dot grid (`radial-gradient`) and concentric rings (`repeating-radial-gradient`). Each carries one accent glow.

### Animation & motion
| Effect | Where | How |
|--------|-------|-----|
| Staggered fade-up entrance | Hero text, buttons | `@keyframes fadeUp` with 0.12s delay steps |
| Floating panel | Hero metrics card | `@keyframes floatY`, infinite ease-in-out |
| Card lift on hover | Service, pricing and testimonial cards | `transform: translateY(-8px)` plus a violet border glow |
| Button lift and glow | Primary buttons | `translateY(-2px)` plus a colored `box-shadow` |
| Image zoom on hover | Portfolio, blog and team images | `transform: scale(1.05)` with a 0.5-0.6s ease |
| Caption reveal | Portfolio items | Overlay fades in on hover |
| Pill nav hover | Navbar links | Animated background and color |
| Carousel arrows | Case-study slider | Border and fill transition on hover |

### Typography & color
- **Unbounded** for headings and numbers, **Plus Jakarta Sans** for body text
- Gradient text on the logo and stat numbers using `background-clip: text`
- Color tokens defined once as CSS variables (`--accent-1` teal, `--accent-2` violet, `--accent-3` rose)

### Accessibility & polish
- `prefers-reduced-motion` support turns off animations and transitions
- Visible `:focus-visible` outlines on links, buttons and form fields
- An ARIA label on the menu toggle and screen-reader text on the carousel controls
- Custom text selection color
- Lazy-loaded images and smooth in-page scrolling

---

## 🅱️ Bootstrap & JavaScript

### JavaScript
The project has **no custom JavaScript**. The only script is the Bootstrap 5.3 bundle, loaded from a CDN, which powers every interactive element below. This keeps the site light, with nothing to build or maintain.

### Bootstrap components in use
| Component | Where it's used | Attribute |
|-----------|-----------------|-----------|
| **Carousel** | Home page case-study slider, with prev/next arrows, indicators and 5.5s auto-play | `data-bs-ride="carousel"` |
| **Offcanvas** | Mobile navigation drawer on every page | `data-bs-toggle="offcanvas"` |
| **Modal** | Portfolio project detail windows (9 modals) | `data-bs-toggle="modal"` |
| **Tabs** | Portfolio category filter: All, Web Design, UI / UX, Mobile, Branding | `data-bs-toggle="tab"` |
| **Accordion / Collapse** | FAQ sections | `data-bs-toggle="collapse"` |
| **Progress bars** | Skills section on the About page | `.progress` |
| **Pagination** | Blog listing | `.pagination` |
| **Breadcrumb** | Inner page headers | `.breadcrumb` |

### Bootstrap layout & utilities
- **12-column grid** with responsive breakpoints (`col-md-*`, `col-lg-*`) and gutters (`g-4`, `g-5`)
- **Flexbox utilities** (`d-flex`, `justify-content-*`, `align-items-*`, `gap-*`)
- **Responsive display** (`d-none`, `d-lg-flex`, `d-lg-none`) to swap the desktop navbar for the mobile drawer
- Spacing, text and overflow helpers
- **Bootstrap Icons** for all icons
- Native **HTML5 form validation** (`required`, `type="email"`) on the contact form

> **Note:** the contact form and newsletter input are front-end only. To receive messages, connect them to a service such as Formspree or Netlify Forms, or to your own backend.

---

## 🛠️ Tech Stack

- **HTML5**: semantic markup
- **CSS3**: custom properties, glassmorphism, gradients, masks, keyframe animations
- **Bootstrap 5.3.3**: grid and interactive components (via CDN)
- **Bootstrap Icons 1.11.3**
- **Google Fonts**: Unbounded and Plus Jakarta Sans
- **SVG**: bundled illustrations for projects, blog posts and team members

## 📁 Project Structure

```
NEXORA/
├── index.html
├── services.html
├── about.html
├── portfolio.html
├── team.html
├── pricing.html
├── blog.html
├── blog-details.html
├── contact.html
├── 404.html
├── css/
│   └── style.css        # design tokens, components, effects
└── images/
    ├── project-*.svg    # 9 portfolio illustrations
    ├── blog-*.svg       # 6 blog covers
    └── team-*.svg       # 6 team portraits
```

## ⚙️ Getting Started

```bash
git clone https://github.com/PashtanaHabib/NEXORA.git
cd NEXORA
# open index.html in your browser
```

Bootstrap, icons and fonts load from a CDN, so you need an internet connection.

## 🎛️ Customization

All colors, radii and spacing are defined in one place, the `:root` block at the top of `css/style.css`:

```css
:root{
  --bg: #070a14;
  --accent-1: #45e0c9;   /* teal   */
  --accent-2: #8b6cf6;   /* violet */
  --accent-3: #ff6f9d;   /* rose   */
  --radius-md: 16px;
  --container-max: 1200px;
}
```

Change these variables and the whole site follows. To use your own photos, replace the files in `images/` or update the `<img src>` paths in the HTML.

---

<div align="center">

Made with ❤️ by **[Pashtana Habib](https://github.com/PashtanaHabib)**

⭐ If you like this project, give it a star!

</div>
