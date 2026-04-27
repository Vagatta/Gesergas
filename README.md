# Gesergas — Web Astro

Sitio en Astro + Tailwind inspirado en la estructura de [instalacioncalderasgas.es](https://instalacioncalderasgas.es/) (Gesergas, Valladolid). Incluye servicios de instalaciones, Naturgy, fontanería, testimonios y formulario de contacto.

## Stack

- [Astro 4](https://astro.build/)
- [Tailwind CSS 3](https://tailwindcss.com/)
- Plugins: `@tailwindcss/forms`, `@tailwindcss/container-queries`
- Iconos: Material Symbols Outlined
- Tipografía: Manrope + Plus Jakarta Sans

## Estructura

```
src/
  layouts/Layout.astro      # HTML base, fuentes y meta
  components/
    Header.astro
    Hero.astro
    Stats.astro
    HowItWorks.astro
    Services.astro          # Calderas, calefacción, A/A, solares, fontanería, Naturgy
    Differentiators.astro
    Pricing.astro
    Testimonials.astro
    ContactCTA.astro        # Formulario + datos de contacto
    Footer.astro
  pages/
    index.astro             # Composición de la home
public/
  favicon.svg
tailwind.config.mjs         # Tema personalizado (paleta + tokens)
astro.config.mjs
```

## Uso

```bash
npm install
npm run dev      # http://localhost:4321
npm run build
npm run preview
```

## Personalización

- Datos de contacto: `src/components/ContactCTA.astro`, `Footer.astro`, `Header.astro`.
- Servicios y bullets: `src/components/Services.astro`.
- Paleta y tokens: `tailwind.config.mjs`.
