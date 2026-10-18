<h1 align="center">iLoomX · Live Project Previews</h1>
<p align="center"><b>Four interactive websites and a working web app, each with a real-time 3D scene</b></p>

<p align="center">
  <a href="https://iloomx.com/preview"><img src="https://img.shields.io/badge/Open_live_demos-iloomx.com/preview-8B5CF6?style=for-the-badge&logo=googlechrome&logoColor=white" alt="Live demos"></a>
</p>
<p align="center">
  <img src="https://img.shields.io/badge/three.js-WebGL-000000?style=flat-square&logo=threedotjs&logoColor=white">
  <img src="https://img.shields.io/badge/GSAP-ScrollTrigger-88CE02?style=flat-square&logo=greensock&logoColor=black">
  <img src="https://img.shields.io/badge/HTML_CSS_JS-no_framework-F7DF1E?style=flat-square&logo=javascript&logoColor=black">
  <img src="https://img.shields.io/badge/Responsive-mobile_first-22C55E?style=flat-square">
</p>

These are working sites, not mockups: visitors can book an appointment, order a pizza, shop for linen or run a sprint board. Each one is a single self-contained HTML file with hand-written CSS and JavaScript.

## Projects

| Project | Live | What's inside |
|---|---|---|
| **Studio Éclat**<br>Beauty studio | [Open →](https://iloomx.com/preview/studio-eclat) | Iridescent 3D liquid hero (custom GLSL noise), cursor-following service photos, before/after slider, 4-step booking with calendar |
| **TaskBoard Pro**<br>SaaS product | [Landing](https://iloomx.com/preview/taskboard-pro) · [Login](https://iloomx.com/preview/taskboard-pro/login) · [App](https://iloomx.com/preview/taskboard-pro/app) | WebGL particle waves, scroll-driven 3D mockup, auth flows, and a full dashboard with drag-and-drop kanban, list, calendar, team, reports, ⌘K palette and light/dark themes |
| **La Bella Napoli**<br>Pizzeria | [Open →](https://iloomx.com/preview/la-bella-napoli) | Procedural 3D pizza with ember particles, photo menu with fly-to-cart, delivery checkout with live order tracking, table reservations |
| **Maison Textile**<br>Linen e-commerce | [Open →](https://iloomx.com/preview/maison-textile) | 3D cloth simulation recoloured live, product colour previews, quick view, bag with free-delivery progress, pinned horizontal story, shoppable lookbook |

> TaskBoard Pro demo login: `demo@taskboard.pro` / `demo1234`

## Techniques

- **3D:** three.js with custom vertex shaders (simplex noise displacement and recomputed normals), procedural geometry and canvas textures, PBR materials (iridescence, sheen, clearcoat)
- **Motion:** GSAP and ScrollTrigger for scroll-linked 3D, pinned sections and FLIP animations, all time-based so it stays smooth on slow devices
- **App logic:** vanilla JS state management, HTML5 drag and drop, keyboard shortcuts, localStorage persistence
- **Quality:** responsive down to 360px, `prefers-reduced-motion` support, keyboard focus states, fallbacks when WebGL or images are unavailable

## Files

```
previews/
├── index.html                  # showcase page
├── studio-eclat.html
├── taskboard-pro.html          # landing
├── taskboard-pro-login.html    # auth
├── taskboard-pro-app.html      # dashboard app
├── la-bella-napoli.html
└── maison-textile.html
```

Served in production by a small Laravel route at [iloomx.com/preview](https://iloomx.com/preview).

## Author

Designed and built by **Soltani Ghaith** ([@M3kanoDev](https://github.com/M3kanoDev)) at **[iLoomX](https://iloomx.com)**, part of the [ServerLoom](https://serverloom.com) ecosystem.
Want something like this? → [M3kano@serverloom.com](mailto:M3kano@serverloom.com)

<sub>Brands and businesses in these demos are fictional. Photos: Unsplash.</sub>
