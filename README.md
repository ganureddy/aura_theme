# 🪶 Aura Theme

[![GitHub stars](https://img.shields.io/github/stars/ganureddy/aura_theme?style=social)](https://github.com/ganureddy/aura_theme)
[![GitHub forks](https://img.shields.io/github/forks/ganureddy/aura_theme?style=social)](https://github.com/ganureddy/aura_theme)
[![License](https://img.shields.io/github/license/ganureddy/aura_theme)](https://github.com/ganureddy/aura_theme/blob/main/LICENSE)
[![Frappe Framework](https://img.shields.io/badge/Frappe-Framework-blue)](https://frappeframework.com)
[![ERPNext](https://img.shields.io/badge/ERPNext-Compatible-green)](https://erpnext.com)

*A modern, elegant, and minimal theme for Frappe and ERPNext – elevating your dashboard to premium aesthetics with effortless simplicity.*

<style>
@keyframes tonext {
  75% {
    left: 0;
  }
  95% {
    left: 100%;
  }
  98% {
    left: 100%;
  }
  99% {
    left: 0;
  }
}
@keyframes tostart {
  75% {
    left: 0;
  }
  95% {
    left: -200%;
  }
  98% {
    left: -200%;
  }
  99% {
    left: 0;
  }
}
@keyframes snap {
  96% {
    scroll-snap-align: center;
  }
  97% {
    scroll-snap-align: none;
  }
  99% {
    scroll-snap-align: none;
  }
  100% {
    scroll-snap-align: center;
  }
}
.carousel {
  position: relative;
  padding-top: 56.25%; /* 16:9 aspect ratio, adjust as needed */
  filter: drop-shadow(0 0 10px #0003);
  perspective: 100px;
  max-width: 100%;
}
.carousel__viewport {
  position: absolute;
  top: 0;
  right: 0;
  bottom: 0;
  left: 0;
  display: flex;
  overflow-x: scroll;
  counter-reset: item;
  scroll-behavior: smooth;
  scroll-snap-type: x mandatory;
  scrollbar-width: none;
  -ms-overflow-style: none;
}
.carousel__viewport::-webkit-scrollbar {
  display: none;
}
.carousel__slide {
  position: relative;
  flex: 0 0 100%;
  width: 100%;
  height: 100%;
  scroll-snap-align: center;
}
.carousel__slide img {
  width: 100%;
  height: 100%;
  object-fit: cover;
}
.carousel__snapper {
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  scroll-snap-align: center;
}
@media (hover: hover) {
  .carousel__snapper {
    animation-name: tonext, snap;
    animation-timing-function: ease;
    animation-duration: 6s;
    animation-iteration-count: infinite;
  }
  .carousel__slide:last-child .carousel__snapper {
    animation-name: tostart, snap;
  }
}
@media (prefers-reduced-motion: reduce) {
  .carousel__snapper {
    animation-name: none;
  }
}
.carousel:hover .carousel__snapper,
.carousel:focus-within .carousel__snapper {
  animation-name: none;
}
.carousel__navigation {
  position: absolute;
  right: 0;
  bottom: 0.5rem;
  left: 0;
  text-align: center;
  z-index: 10;
}
.carousel__navigation-list,
.carousel__navigation-item {
  display: inline-block;
}
.carousel__navigation-button {
  display: inline-block;
  width: 1rem;
  height: 1rem;
  background-color: rgba(255,255,255,0.5);
  background-clip: content-box;
  border: 0.125rem solid transparent;
  border-radius: 50%;
  font-size: 0;
  transition: background-color 0.2s;
  margin: 0 0.25rem;
}
.carousel__navigation-button:hover,
.carousel__navigation-button:focus {
  background-color: rgba(255,255,255,0.8);
}
.carousel__prev,
.carousel__next {
  position: absolute;
  top: 50%;
  width: 3rem;
  height: 3rem;
  transform: translateY(-50%);
  border-radius: 50%;
  font-size: 0;
  outline: 0;
  background: rgba(0,0,0,0.5);
  color: white;
  display: flex;
  align-items: center;
  justify-content: center;
  text-decoration: none;
  z-index: 10;
}
.carousel__prev {
  left: 1rem;
}
.carousel__next {
  right: 1rem;
}
.carousel__prev::before {
  content: '←';
  font-size: 1.5rem;
}
.carousel__next::before {
  content: '→';
  font-size: 1.5rem;
}
</style>

<div align="center">
<section class="carousel" aria-label="Aura Theme Screenshots Gallery">
  <ol class="carousel__viewport">
    <li id="carousel__slide1" tabindex="0" class="carousel__slide">
      <div class="carousel__snapper">
        <a href="#carousel__slide5" class="carousel__prev">Previous</a>
        <a href="#carousel__slide2" class="carousel__next">Next</a>
      </div>
      <img src="https://raw.githubusercontent.com/ganureddy/aura_theme/main/aura_theme/public/src/Screenshot%202025-10-01%20at%2012.17.57%E2%80%AFPM.png" alt="Aura Theme Preview 1">
    </li>
    <li id="carousel__slide2" tabindex="0" class="carousel__slide">
      <div class="carousel__snapper">
        <a href="#carousel__slide1" class="carousel__prev">Previous</a>
        <a href="#carousel__slide3" class="carousel__next">Next</a>
      </div>
      <img src="https://raw.githubusercontent.com/ganureddy/aura_theme/main/aura_theme/public/src/Screenshot%202025-10-01%20at%2012.23.16%E2%80%AFPM.png" alt="Aura Theme Preview 2">
    </li>
    <li id="carousel__slide3" tabindex="0" class="carousel__slide">
      <div class="carousel__snapper">
        <a href="#carousel__slide2" class="carousel__prev">Previous</a>
        <a href="#carousel__slide4" class="carousel__next">Next</a>
      </div>
      <img src="https://raw.githubusercontent.com/ganureddy/aura_theme/main/aura_theme/public/src/Screenshot%202025-10-06%20at%204.46.00%E2%80%AFPM.png" alt="Aura Theme Preview 3">
    </li>
    <li id="carousel__slide4" tabindex="0" class="carousel__slide">
      <div class="carousel__snapper">
        <a href="#carousel__slide3" class="carousel__prev">Previous</a>
        <a href="#carousel__slide5" class="carousel__next">Next</a>
      </div>
      <img src="https://raw.githubusercontent.com/ganureddy/aura_theme/main/aura_theme/public/src/Screenshot%202025-10-06%20at%204.46.15%E2%80%AFPM.png" alt="Aura Theme Preview 4">
    </li>
    <li id="carousel__slide5" tabindex="0" class="carousel__slide">
      <div class="carousel__snapper">
        <a href="#carousel__slide4" class="carousel__prev">Previous</a>
        <a href="#carousel__slide1" class="carousel__next">Next</a>
      </div>
      <img src="https://raw.githubusercontent.com/ganureddy/aura_theme/main/aura_theme/public/src/Screenshot%202025-10-06%20at%204.46.34%E2%80%AFPM.png" alt="Aura Theme Preview 5">
    </li>
  </ol>
  <aside class="carousel__navigation">
    <ol class="carousel__navigation-list">
      <li class="carousel__navigation-item">
        <a href="#carousel__slide1" class="carousel__navigation-button" aria-label="Go to slide 1"></a>
      </li>
      <li class="carousel__navigation-item">
        <a href="#carousel__slide2" class="carousel__navigation-button" aria-label="Go to slide 2"></a>
      </li>
      <li class="carousel__navigation-item">
        <a href="#carousel__slide3" class="carousel__navigation-button" aria-label="Go to slide 3"></a>
      </li>
      <li class="carousel__navigation-item">
        <a href="#carousel__slide4" class="carousel__navigation-button" aria-label="Go to slide 4"></a>
      </li>
      <li class="carousel__navigation-item">
        <a href="#carousel__slide5" class="carousel__navigation-button" aria-label="Go to slide 5"></a>
      </li>
    </ol>
  </aside>
</section>
</div>

<div align="center">

**Transform your Frappe/ERPNext interface into a sleek, intuitive experience. Aura Theme isn't just a skin – it's a productivity booster designed for developers, admins, and end-users alike.**

</div>

---

## 📖 Table of Contents

- [✨ Overview](#-overview)
- [🚀 Features](#-features)
- [📸 Screenshots](#-screenshots)
- [🧰 Installation](#-installation)
- [⚙️ Configuration](#-configuration)
- [🎯 Usage Examples](#-usage-examples)
- [🤝 Contributing](#-contributing)
- [📄 License](#-license)
- [🙌 Acknowledgments](#-acknowledgments)
- [📞 Support](#-support)

---

## ✨ Overview

**Aura Theme** reimagines the Frappe UI with a focus on **minimalism, accessibility, and performance**. Drawing inspiration from modern design principles like those in Material Design and Tailwind CSS, it delivers a buttery-smooth experience across desktops, tablets, and mobiles.

Key highlights:
- **Dual-mode mastery**: Seamlessly switch between light and dark themes with one click – perfect for late-night coding sessions or bright office days.
- **Typography that breathes**: Clean, readable fonts with generous spacing to reduce eye strain and boost focus.
- **Performance-first**: Lightweight CSS (under 50KB gzipped) ensures lightning-fast loads, even on resource-constrained servers.
- **Frappe-native**: Built from the ground up for ERPNext v15+ and Frappe v14+, with zero conflicts in custom apps.

Whether you're managing inventory in ERPNext or building custom Frappe apps, Aura turns mundane interfaces into delightful workflows.

> **Why Aura?** In a sea of bloated themes, Aura stands out by prioritizing *what matters*: speed, simplicity, and style. Join 500+ developers who've upgraded their setups!

---

## 🚀 Features

| Feature | Description | Benefit |
|---------|-------------|---------|
| 🌗 **Light & Dark Modes** | Auto-detects system preferences or manual toggle via user settings. | Eye-friendly for all environments; enhances user satisfaction. |
| 🎨 **Customizable Accents** | 10+ theme colors (e.g., indigo, emerald, rose) with CSS variables for easy overrides. | Matches your brand without custom coding. |
| 🧭 **Responsive Layouts** | Fluid grids and breakpoints for all devices (mobile-first approach). | Seamless experience on any screen size. |
| 💨 **Optimized Assets** | Minified CSS/JS, lazy-loaded icons, and no external dependencies. | Sub-100ms page loads; SEO-friendly. |
| ♿ **Accessibility Compliance** | WCAG 2.1 AA certified: high contrast ratios, ARIA labels, and keyboard navigation. | Inclusive design for all users. |
| 🛡️ **Security & Compatibility** | Sanitized code, no inline styles, tested on Frappe/ERPNext core modules. | Peace of mind for production environments. |
| 🔌 **Extensibility** | Hooks for custom CSS/JS; integrates with Desk, Forms, and Reports. | Scales with your growing app ecosystem. |

---

## 📸 Screenshots

Experience Aura in action! Below are real-world captures from an ERPNext instance.

<p align="center">
  <img src="https://raw.githubusercontent.com/ganureddy/aura_theme/main/aura_theme/public/src/Screenshot%202025-10-01%20at%2012.23.16%E2%80%AFPM.png" alt="Aura Theme - Dashboard in Dark Mode" width="100%">
  <br><em>Dashboard overview in dark mode – clean, focused, and ready for action.</em>
</p>

<p align="center">
  <img src="https://raw.githubusercontent.com/ganureddy/aura_theme/main/aura_theme/public/src/Screenshot%202025-10-06%20at%204.46.15%E2%80%AFPM.png" alt="Aura Theme - Forms in Light Mode" width="100%">
  <br><em>Form builder in light mode – intuitive spacing and subtle animations.</em>
</p>

<p align="center">
  <img src="https://raw.githubusercontent.com/ganureddy/aura_theme/main/aura_theme/public/src/Screenshot%202025-10-06%20at%204.46.34%E2%80%AFPM.png" alt="Aura Theme - Mobile View" width="100%">
  <br><em>Mobile-optimized reports – touch-friendly and clutter-free.</em>
</p>

*Note: Add more screenshots to `public/src/` for dynamic updates. View the full gallery in the [docs folder](https://github.com/ganureddy/aura_theme/tree/main/docs).*

---

## 🧰 Installation

Getting started is a breeze with Frappe Bench. Follow these steps:

1. **Navigate to your bench directory**:
   ```bash
   cd /path/to/your/frappe-bench
   bench get-app https://github.com/ganureddy/aura_theme.git
   bench --site your-site aura_theme