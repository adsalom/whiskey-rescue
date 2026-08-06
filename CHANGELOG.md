# Whisky Rescue — Registro de Cambios

> Documento de seguimiento del proyecto. Cada cambio relevante se registra aquí con fecha, descripción y estado.

---

## Estado Actual

| Elemento | Estado |
|----------|--------|
| Landing page (HTML/CSS/JS) | Remodelada con identidad oficial |
| Bilingüismo EN/ES | Implementado |
| Age Gate | Implementado (con logo oficial) |
| Identidad visual (paleta brand guide) | Aplicada (#B69759 · #593930 · #5C5C5B · #1D1D1B) |
| Tipografías oficiales | Centaur MT + Guild of Professional Actors (local) + Barlow |
| Logos oficiales | Integrados (age gate, header, footer, favicon, marca de agua) |
| Fotografías del cliente | Integradas y optimizadas (verificadas sin hielo) |
| Experiencias de autor | Cuatro experiencias oficiales integradas; dos adicionales pendientes de definición |
| Formulario de contacto | Placeholder (pendiente integración + email destino) |
| WhatsApp oficial | Integrado: `wa.me/34649158386` |
| Dominio personalizado | Pendiente |
| Analytics (GA4, Meta, TikTok) | Placeholders configurados |
| Textos legales (privacidad/cookies/aviso) | Enlaces "Próximamente" |
| Deploy Cloudflare Pages | Activo |

---

## Registro

### 2026-08-05 — Integración de experiencias oficiales y Ultra Bespoke

**Tipo:** Contenido / Desarrollo
**Estado:** Completado parcialmente (pendientes dos experiencias adicionales)

- Integradas en la landing las cuatro experiencias definidas en `WR experiencias de autor.docx`: **Un momento, un whisky a la vez**, **The Genesis Experience**, **The Circle** y **The Fusion Series W&W**.
- Retirados los nombres provisionales I–VI que no tenían respaldo documental.
- Actualizado `Ultra Bespoke Experience` con el alcance global, máximo de tres expresiones, honorarios del especialista de `€2.500`, transporte, hospedaje y acuerdo de confidencialidad, según `WR Ultra bespoke.docx` y ambos brochures.
- Integrados el teléfono `+34 649 158 386`, el enlace de WhatsApp y `whiskyrescuebog@gmail.com` desde el brochure oficial.
- Alineados el hero, la introducción y el tono del sitio con el manifiesto oficial.
- El brief declara seis experiencias, pero los documentos específicos entregados solo definen cuatro; las dos restantes quedan pendientes para no inventar contenido.

### 2026-07-29 — Remodelación con identidad oficial de marca

**Tipo:** Diseño / Desarrollo  
**Estado:** Completado

Material del cliente recibido (carpeta `Identidad`): brand guide oficial, 6 logos PNG, fuente Centaur MT, 13 fotografías de degustaciones + 2 fotos del equipo, documento de estrategia KOM.

**Identidad aplicada (brand guide):**
- Paleta oficial: `#B69759` (dorado), `#593930` (marrón), `#5C5C5B` (gris), `#1D1D1B` (negro)
- Sistema tipográfico por roles:
  - **Guild of Professional Actors** (fuente del logotipo, licencia uso libre): titular del hero y títulos Ultra Bespoke — solo textos verificados sin acentos (la fuente no incluye charset español)
  - **Centaur MT** (archivo del cliente, woff2 33 KB): serif editorial para títulos de sección, citas, numerales romanos y precios
  - **Barlow** (Google Fonts, línea gráfica KOM): sans funcional para cuerpo, navegación, etiquetas, botones y formularios
- Logo oficial apilado en age gate, header y footer (`logo-stacked.png`: el PNG original del cliente con el lienzo transparente vacío recortado — el arte no se tocó). Favicons actualizados a ícono blanco sobre fondo color negro de la marca (`#1D1D1B`) para alta visibilidad. (Anteriormente: ícono dorado sobre fondo crema)
- Título de la pestaña (`<title>`) acortado a "Whisky Rescue - Experiences" para evitar truncamiento en el navegador.
- Eliminada la marca de agua con el ícono del logo en el fondo del age gate para evitar la percepción de "logo sobre logo".
- Ícono-estrella como marca de agua en secciones (recurso permitido por la guía)
- Fotografías reales optimizadas (15 imágenes, ~2 MB total, JPEG progresivo) — todas verificadas sin hielo (restricción explícita del cliente)
- Fotos del equipo incluidas sin nombres (decisión del cliente)

**Correcciones sobre la versión anterior:**
- Bug `lang-se` → `lang-es` (el título de Experiencias nunca se mostraba en español)
- "Tailored Curaduría" → "Tailored Curation" (spanglish en texto EN)
- Precios por experiencia unificados al rango oficial €100–€350/persona (la versión anterior asignaba precios escalonados no aprobados)
- Opciones del select de experiencias ahora sí son bilingües (data-en/data-es + swap en `setLang`)
- Alertas de formularios bilingües
- Año del footer dinámico
- `prefers-reduced-motion` respetado
- Meta OG, JSON-LD de organización y preload de fuentes añadidos

**Assets generados:**
```
assets/
├── fonts/   centaur-mt-regular.woff2 · guild-of-professional-actors.woff2
├── logos/   logo-stacked.png (original recortado de márgenes) · logo-gold.png
│            logo-white.png · icon-gold.png · icon-dark.png · favicon-64.png · favicon-512.png
└── img/     15 fotografías optimizadas (hero, experiencias, historia, equipo)
```

---

### 2025-07-28 — Deploy inicial a Cloudflare Pages

**Tipo:** Infraestructura  
**Estado:** Completado

- Repositorio creado en GitHub: `adsalom/whiskey-rescue`
- Proyecto desplegado en Cloudflare Pages
- URL de producción: https://whiskey-rescue.pages.dev
- URL de preview: https://d8cef994.whiskey-rescue.pages.dev
- Rama `main` configurada como producción

---

### 2025-07-28 — Estructura inicial de la landing page

**Tipo:** Desarrollo  
**Estado:** Completado

- Age Gate con verificación de edad (modal bilingüe)
- Header fijo con efecto scroll y menú móvil
- Hero section con CTAs
- Sección de introducción a la marca
- Ultra Bespoke Experience (sección premium)
- Preview de experiencias (grid)
- Testimonios / prueba social
- Sección Sobre Nosotros / Historia
- Detalle de experiencias (6 + Ultra Bespoke)
- Formulario de contacto (placeholder)
- Footer con newsletter y redes sociales
- Scroll animations con IntersectionObserver
- Smooth scroll para anchors

---

## Pendientes del Cliente

> Estos elementos están esperando respuesta o aprobación del cliente.

1. Definición de las dos experiencias adicionales mencionadas en el brief
2. Email de destino del formulario
3. Integración con CRM o solo email
4. IDs reales de analytics (GA4, Meta Pixel, TikTok Pixel, Meta CAPI)
5. Textos legales: política de privacidad, aviso legal, política de cookies (RGPD)
6. Testimonios reales (hoy: genéricos sin nombres)
7. Tagline / propuesta de valor definitiva
8. Dominio personalizado (whiskyrescue.com ya registrado)

**Resueltos el 2026-07-29:** brandbook (paleta + tipografías), logos, fotografías reales, verificación de edad por sesión.

---

## Notas de Desarrollo

### Stack actual
- HTML5 + CSS3 + JavaScript vanilla
- Google Fonts (Barlow)
- Sin frameworks — diseño estático
- CSS custom properties para theming
- Deploy: Cloudflare Pages

### Estructura de archivos
```
whiskey-rescue/
├── index.html              # Landing page completa
├── WIREFRAME.md            # Documento de estructura
├── prompt-kimi-whisky-rescue.md  # Prompt de referencia
├── whiskey-rescue-brief.pdf      # Brief del proyecto
├── .gitignore
├── CHANGELOG.md            # Este documento
├── node_modules/           # Wrangler (dev dependency)
└── package.json            # Configuración npm
```

---

## Enlaces Relevantes

| Recurso | URL |
|---------|-----|
| Producción | https://whiskey-rescue.pages.dev |
| GitHub | https://github.com/adsalom/whiskey-rescue |
| Dashboard Cloudflare | https://dash.cloudflare.com |
