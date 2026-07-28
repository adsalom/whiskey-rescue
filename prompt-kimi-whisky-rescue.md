# Prompt para Kimi K2 — Whisky Rescue

Eres un diseñador/desarrollador web senior. Vas a maquetar (wireframe + diseño visual de alta fidelidad) el sitio web de **Whisky Rescue**, una marca de experiencias exclusivas de whisky. Genera el sitio como HTML/CSS (single-file o por secciones, según se indique), responsive, listo para revisión de cliente antes de pasar a desarrollo final.

## Marca

- Nombre: Whisky Rescue. Sin tagline definido — no lo inventes, deja el espacio libre o usa el nombre solo.
- Historia: nacida durante la pandemia como cajas de regalo de whisky y accesorios; se convirtió en la primera barra fija exclusiva de whisky en Bogotá; hoy ofrece experiencias y sesiones académicas de whisky.
- Misión: enriquecer la vida de las personas descubriendo la cultura del whisky y estrechando lazos con una comunidad de aficionados.
- Visión: ser referente global de experiencias de whisky de alto nivel.
- Posicionamiento: exclusividad ante todo (no precio, no "gurú", no volumen).
- Un año de inactividad, pero con portafolio de eventos corporativos, celebraciones privadas y sesiones académicas con especialistas reconocidos.

## Tono de voz

Conocedor pero sin pretensión. Un facilitador, no un gurú. Cercano, adaptable a cualquier nivel de conocimiento del huésped, buen orador. Humor permitido pero dosificado y respetuoso. Evita sonar como "el que más sabe" o "farandulero".

Palabras a usar: degustación, expresión/expresiones (para referirse a botellas), "rescatamos el arte de tomar whisky", "respetamos el líquido".
Evitar: "cata" / "cata de whisky" (no molestan pero se prefiere no usarlas).
Nunca mencionar ni mostrar hielo en ningún lugar del sitio (texto ni imágenes).

Sensación que debe dejar el sitio en el visitante: "quiero contratar los servicios de Whisky Rescue sin importar el costo."

## Estética visual

Sobria, elegante, con una pincelada vintage, sensación de "costoso"/exclusivo. Sin brandbook ni logo entregados todavía — usa una paleta provisional (negros, dorados/ámbar tipo whisky, crema/hueso) y tipografía serif elegante + sans neutra de apoyo, dejando comentarios `<!-- reemplazar con [asset] cuando el cliente lo entregue -->` en el logo, colores exactos y tipografías reales.

## Público objetivo

Dos segmentos:
1. Clientes ultra alto poder adquisitivo que contratan atención exclusiva a medida (ej. dueño de embarcación en el GP de Mónaco, ejecutivos en un loft en Seúl) — dispuestos a cubrir honorarios, transporte y botellas de alto valor. Este segmento corresponde al servicio insignia "Ultra Bespoke Experience".
2. Público general mayor de edad, sin restricción de salud para consumir alcohol, desde curiosos hasta conocedores de whisky.

## Servicio y modelo de negocio

- 6 experiencias disponibles (curaduría de autor, ninguna experiencia se repite igual).
- Servicio insignia a destacar: "Ultra Bespoke Experience".
- Rango de precio general: €100–€350 por persona; el servicio insignia es de ticket alto y a cotizar.
- Alcance global: se desplazan donde el cliente lo requiera.
- No hay compra online ni reservas automatizadas: el flujo es formulario de contacto → seguimiento por WhatsApp.
- No hay tienda, blog, prensa, ni zona de miembros.

## Estructura del sitio (propuesta — pendiente de validar con el cliente, quien delegó esta decisión a un tercero sin resolver)

1. **Home**: hero con propuesta de valor y CTA principal ("Solicitar una experiencia"), introducción breve a la marca, destaque del servicio insignia, prueba social/testimonios genéricos (sin cifras ni nombres reales todavía).
2. **Sobre Nosotros / Historia**: origen, misión, visión, por qué el nombre.
3. **Experiencias**: las 6 experiencias con descripción, rango de precio, y la Ultra Bespoke Experience destacada aparte como servicio insignia.
4. **Contacto**: formulario de captura de leads (nombre, contacto, tipo de experiencia de interés, mensaje) + botón directo a WhatsApp.
5. **Footer**: newsletter (captura de email), redes (Instagram @whiskyrescue, TikTok @whisky.rescue), verificación de edad, datos legales (pendientes).

## Requisitos funcionales y técnicos

- Bilingüe: inglés (principal) y español.
- Verificación de edad obligatoria al ingresar (gate/modal antes de mostrar contenido).
- Formulario de contacto para captura de leads.
- Newsletter / captura de email.
- Sin tienda online, sin blog, sin sistema de reservas, sin login/zona de miembros.
- Analítica a integrar (dejar los hooks/placeholders en el código): Google Analytics, Meta Pixel, TikTok Pixel, Meta Conversions API.
- Dominio ya registrado: whiskyrescue.com.
- Legal: política de privacidad, aviso legal y política de cookies (RGPD) aún no existen — dejar secciones/enlaces de footer como placeholder "Próximamente" o generar borrador genérico a revisar por el cliente.

## Restricciones explícitas

- Nada de hielo (imágenes ni menciones).
- Nada de tono de "experto sabelotodo" o "farandulero".
- No inventes cifras de precios exactos por experiencia individual más allá del rango €100–€350 y el hecho de que la Ultra Bespoke es "a cotizar"/alto valor.
- No inventes testimonios con nombres reales; usa marcadores tipo "Cliente corporativo, Bogotá" si necesitas ejemplos de prueba social.

## Entregable

Genera primero el wireframe/estructura de página (secciones y jerarquía de contenido) para validación, y luego la versión de alta fidelidad con la estética descrita arriba. Señala explícitamente en comentarios qué elementos son provisionales a la espera de: logo/brandbook real, colores HEX exactos, tipografías reales, fotografía profesional, y validación de la estructura de secciones por parte del cliente.
