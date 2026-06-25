# Hause · Arquitectura + Construcción — Sitio web

Sitio estático (HTML + CSS + JS, sin build) construido a partir del brochure y el sitemap definido.

## Estructura
- `index.html` — el sitio completo (una sola página con las secciones del sitemap: Inicio, Verticales, Nosotros, Servicios + Inversiones, Proceso, Proyectos y Contacto).
- `img/` — imágenes del brochure, optimizadas para web y clasificadas por vertical (`res-*`, `com-*`, `corp-*`).

## Cómo verlo / publicarlo
- **Local:** abrí `index.html` en el navegador (mantené la carpeta `img/` al lado).
- **Producción:** subí toda la carpeta a cualquier hosting estático (Vercel, Netlify, Cloudflare Pages o un hosting común vía FTP) y apuntá `hause.com.py` ahí.

## Qué editar
Todo lo configurable está al inicio del `<script>` en `index.html`:
- `HAUSE.whatsapp` — número de WhatsApp (formato internacional sin +).
- `HAUSE.email` — correo de contacto.
- `HAUSE.crmEndpoint` — opcional: webhook para guardar las consultas del formulario (igual funciona mandando al WhatsApp).
- `PROJECTS` — agregá, quitá o renombrá obras del portafolio. El filtro y el lightbox se actualizan solos.

## Sobre las imágenes
Son las del brochure (renders y fotos de obra). Para mejor calidad, conviene reemplazarlas por fotos en alta de cada obra terminada, manteniendo los mismos nombres de archivo en `img/`.

## Sitemap → secciones
Esta es la versión de una sola página. Si más adelante querés URLs separadas (`/nosotros`, `/proyectos`, etc.), la estructura ya está seccionada y se divide fácil.
