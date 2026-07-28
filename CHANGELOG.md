# Whisky Rescue — Registro de Cambios

> Documento de seguimiento del proyecto. Cada cambio relevante se registra aquí con fecha, descripción y estado.

---

## Estado Actual

| Elemento | Estado |
|----------|--------|
| Landing page (HTML/CSS/JS) | En desarrollo |
| Bilingüismo EN/ES | Implementado |
| Age Gate | Implementado |
| Formulario de contacto | Placeholder (pendiente integración) |
| Contenido final (copy) | Pendiente del cliente |
| Fotografías / assets visuales | Pendientes (usando placeholders) |
| Dominio personalizado | Pendiente |
| Analytics (GA4, Meta, TikTok) | Placeholders configurados |
| Deploy Cloudflare Pages | Activo |

---

## Registro

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

1. Nombre definitivo o provisional de las 6 experiencias
2. Fotografías profesionales o uso de stock
3. Destino del formulario de contacto (email específico)
4. Integración con CRM o solo email
5. Verificación de edad: por sesión o con cookie
6. Uso de cookies para analytics (RGPD)
7. Contenido adicional (prensa, colaboraciones)
8. Tagline / propuesta de valor definitiva
9. Brandbook con tipografías y colores exactos
10. Dominio personalizado

---

## Notas de Desarrollo

### Stack actual
- HTML5 + CSS3 + JavaScript vanilla
- Google Fonts (Playfair Display + Inter)
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
