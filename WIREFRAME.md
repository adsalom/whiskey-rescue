# Whisky Rescue — Wireframe Estructural

> **Documento de validación antes de diseño de alta fidelidad.**
> Pendiente de aprobación por parte del cliente sobre estructura de secciones y jerarquía de contenido.

---

## 1. AGE GATE (Modal de verificación de edad)

- Pantalla completa, bloqueante antes de mostrar cualquier contenido
- Fondo oscuro con textura sutil (madera/oscura)
- Logo centrado (placeholder)
- Texto: "¿Confirmas que tienes legalidad para consumir bebidas alcohólicas en tu país?"
- Botones: **Sí, confirmo** / **No** (redirige o muestra mensaje de despedida)
- Sin opción de recordar — se valida por sesión
- Bilingüe: toggle EN/ES en el propio modal

---

## 2. HEADER / NAVEGACIÓN

- **Posición:** Fija arriba, transparente que se vuelve sólida al hacer scroll
- **Logo:** Izquierda (placeholder hasta brandbook)
- **Nav:** Derecha — Experiencias | Sobre Nosotros | Contacto
- **Idioma:** Toggle EN/ES al final del nav
- **CTA móvil:** Botón hamburguesa con menú overlay

---

## 3. HOME — Hero

- **Sección:** Full viewport height
- **Fondo:** Imagen de atmósfera de whisky (sin hielo, sin copa con hielo — ambiente de bar/madera/destilería)
- **Contenido:**
  - Headline: Nombre de marca + propuesta de valor (ej. "The Art of Whisky, Rescued" / "El arte del whisky, rescatado")
  - Subtítulo breve (1 línea)
  - CTA primario: **"Solicitar una experiencia"** → enlaza a Contacto
  - CTA secundario: "Descubrir nuestras experiencias" → scroll a Experiencias
- **Nota:** No hay tagline definido — dejar espacio para uno, usar solo el nombre como marca

---

## 4. HOME — Introducción a la marca

- **Layout:** Dos columnas (imagen + texto) o centrado
- **Contenido:**
  - 2-3 frases sobre qué es Whisky Rescue
  - Mención del origen (pandemia → barra fija → experiencias)
  - Sin entrar en detalle — la historia completa va en "Sobre Nosotros"

---

## 5. HOME — Ultra Bespoke Experience (Destaque del servicio insignia)

- **Sección:** Separada visualmente del resto (fondo diferente o borde dorado)
- **Layout:** Bloque premium, centrado
- **Contenido:**
  - Título: "Ultra Bespoke Experience"
  - Descripción breve del servicio (exclusividad, a medida, global)
  - Indicación "A cotizar" o "Consulta por este servicio"
  - CTA: "Solicitar información" → Contacto con preselección del tipo
- **Estilo:** Más lujoso que el resto de la página — borde dorado, tipografía más elaborada

---

## 6. HOME — Experiencias (Preview de las 6)

- **Layout:** Grid 2x3 o carrusel (decidir en desarrollo)
- **Cada tarjeta:**
  - Imagen representativa (placeholder)
  - Nombre de la experiencia
  - Descripción 1-2 líneas
  - Rango de precio: "Desde €100 por persona"
  - **NO** se listan los 6 nombres aquí — solo se muestran como preview
  - CTA: "Conocer más" → scroll a sección completa o a Contacto

---

## 7. HOME — Prueba social / Testimonios

- **Layout:** Carrusel o grid de 3 testimonios
- **Formato:** Cita textual + atribución genérica
- **Ejemplos:**
  - "Una experiencia que transformó nuestra reunión de equipo." — *Cliente corporativo, Bogotá*
  - "El nivel de detalle y curaduría es insuperable." — *Anfitrión de evento privado*
  - "Sin duda la mejor degustación de whisky a la que he asistido." — *Asistente, sesión académica*
- **Sin cifras ni nombres reales**

---

## 8. SOBRE NOSOTROS / HISTORIA

- **Layout:** Sección larga con scroll vertical, contenido en bloques
- **Subsecciones:**
  1. **Origen:** Pandemia → cajas de regalo → barra fija en Bogotá → experiencias
  2. **Misión:** Enriquecer vidas descubriendo la cultura del whisky
  3. **Visión:** Ser referente global de experiencias de whisky de alto nivel
  4. **Por qué "Rescue":** Rescatar el arte de tomar whisky, respetar el líquido
  5. **Equipo / Especialistas:** Mención de que trabajan con especialistas reconocidos (sin nombres aún)
- **Estilo:** Storytelling visual, parallax suave o scroll animations

---

## 9. EXPERIENCIAS (Detalle completo)

- **Layout:** Lista vertical con secciones alternas (imagen izquierda/derecha)
- **Cada experiencia:**
  - Nombre
  - Descripción completa (2-3 párrafos)
  - Incluye: "Degustación de expresiones seleccionadas" (usar "expresiones", no "botellas" ni "cata")
  - Rango de precio general: €100–€350 por persona
  - CTA: "Solicitar esta experiencia" → Contacto con preselección
- **Ultra Bespoke Experience:** Sección separada al final, más elaborada, con lenguaje de exclusividad total
- **NO se especifica cuáles son las 6 experiencias** — el cliente debe definirlas

---

## 10. CONTACTO

- **Layout:** Dos columnas (formulario + info de contacto)
- **Formulario:**
  - Nombre completo
  - Email
  - Teléfono / WhatsApp
  - Tipo de experiencia de interés (select: las 6 + Ultra Bespoke + "Otro")
  - Mensaje / Comentarios
  - Botón: "Enviar solicitud"
- **Info de contacto:**
  - Botón directo a WhatsApp: "O escríbenos por WhatsApp"
  - Email de contacto
  - Redes sociales
- **Nota:** No hay reservas automatizadas — el flujo es formulario → seguimiento humano

---

## 11. FOOTER

- **Layout:** 3-4 columnas
- **Columnas:**
  1. Logo + descripción breve
  2. Navegación rápida (links internos)
  3. Redes sociales (Instagram @whiskyrescue, TikTok @whisky.rescue)
  4. Newsletter (captura de email: input + botón "Suscribirme")
- **Bottom bar:**
  - © 2024 Whisky Rescue. Todos los derechos reservados.
  - Enlaces legales: Política de privacidad | Aviso legal | Política de cookies
  - Todos como "Próximamente" o placeholder
  - Verificación de edad: "Este sitio contiene información sobre bebidas alcohólicas. Confirma que tienes la edad legal para acceder."

---

## 12. ANALYTICS PLACEHOLDERS

En el `<head>` y antes del `</body>`, dejar comments con hooks para:
- Google Analytics (GA4) — `G-XXXXXXXXXX`
- Meta Pixel — `XXXXXXXXXX`
- TikTok Pixel — `XXXXXXXXXX`
- Meta Conversions API — token placeholder

---

## 13. BILINGÜISMO

- Toggle EN/ES en header
- Por defecto: inglés
- Cambio de idioma con JavaScript simple (ocultar/mostrar contenido por `data-lang`)
- No se usa framework — es un toggle estático

---

## PREGUNTAS PENDIENTES PARA EL CLIENTE

1. ¿Las 6 experiencias tienen nombre definitivo o provisional?
2. ¿Hay fotografías profesionales disponibles o usamos placeholders de stock?
3. ¿El formulario de contacto tiene destino (email específico)?
4. ¿Se necesita integración con algún CRM o solo email?
5. ¿La verificación de edad es por sesión o se recuerda con cookie?
6. ¿Se permite el uso de cookies para analytics (RGPD)?
7. ¿Hay algún contenido adicional que deba incluirse (prensa, colaboraciones)?
