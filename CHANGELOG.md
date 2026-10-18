# Changelog

Registro de las solicitudes, resultados y decisiones de diseño relevantes del proyecto. Las citas de las personas y los objetivos de usabilidad son arquetipos/umbrales propuestos hasta validarlos con participantes reales.

## [Fecha no registrada, antes de 2026-10-16] — Estructuración inicial del diseño en Figma

- **Herramientas:** Figma y asistente IA.
- **Qué se pidió:** Crear el contenido del MVP MOMART VIP en las páginas de personas, User Flow, Sitemap, wireframes móvil y wireframes PC.
- **Qué devolvió:** Se estructuraron las dos personas (cliente VIP y personal de barra), el flujo QR-carta-pedido-pago-entrega, la arquitectura de información y las pantallas móvil y de gestión de barra.
- **Qué se conservó:** La propuesta de pedidos a mesa desde un QR exclusivo por reservado y la diferenciación del servicio VIP frente a la barra general.
- **Qué se cambió y por qué:** Se tradujeron las necesidades del cliente y del personal en pantallas y pasos operativos que sirvieran de base para revisar el MVP. Las citas de persona se consideran frases de arquetipo, no transcripciones.

## [2026-10-16] — Auditoría de rúbrica, casos límite y alcance

- **Herramientas:** Figma, FigJam, GitHub y asistente IA.
- **Qué se pidió:** Contrastar el diseño con la rúbrica, corregir los wireframes, añadir casos límite y preparar materiales de investigación, alcance y documentación.
- **Qué devolvió:** Se amplió el User Flow con recuperación ante QR/conectividad fallida, falta de stock y pago denegado; se revisaron los wireframes móviles; se creó en FigJam una plantilla para entrevistas, benchmark, mapa de afinidad y matriz Dentro/Fuera; y se creó el repositorio público con BRIEF.md y CHANGELOG.md.
- **Qué se conservó:** El flujo principal de pedido para reservados por QR, las personas de cliente VIP y personal de barra, y las tres situaciones de recuperación priorizadas.
- **Qué se cambió y por qué:** Se añadieron las pantallas 1.0 QR, 4.0 Carrito y 5.0 Pago para cubrir el recorrido del Sitemap/User Flow. Se pasó a escala de grises estricta para ajustarse a la consigna de wireframes. Los valores de espera, ruido y error mencionados durante la auditoría no se reportan como mediciones.
- **Pendiente:** El FigJam es una plantilla visual; entrevistas, benchmark y hallazgos siguen pendientes. No se inventaron resultados ni consentimientos.

## [2026-10-18] — README y definición del brief

- **Herramientas:** GitHub y asistente IA.
- **Qué se pidió:** Presentar brevemente el proyecto en README.md y enlazar directamente al brief; auditar los cinco apartados requeridos del brief.
- **Qué devolvió:** README.md describe la aplicación y enlaza con el archivo relativo BRIEF.md. Se ampliaron las fichas de Álvaro Benítez y Carlos Navarro y se formularon tareas y umbrales verificables separados para P1 y P2.
- **Qué se conservó:** El enlace relativo al brief y la distinción explícita entre hipótesis de diseño y evidencia observada.
- **Qué se cambió y por qué:** Se añadió un presupuesto inicial de transferencia inferior a 400 KB, indicado como objetivo del proyecto que debe medirse, no como requisito normativo de W3C; se detallaron los perfiles y pruebas para hacer los criterios observables.
- **Pendiente:** Las entrevistas reales con P1/P2 y sus datos no están disponibles; no se presentan como realizadas ni se fabrican citas o resultados.

## [2026-10-18] — Configuración del prototipo móvil

- **Herramientas:** Figma y asistente IA.
- **Qué se pidió:** Evitar que Play abriera una lámina con varias pantallas y configurar un flujo móvil reproducible desde la pantalla QR.
- **Qué devolvió:** Se prepararon seis frames raíz, el inicio «Flujo Principal MVP», dispositivo iPhone 15 y las conexiones QR → Carta → Configurador → Carrito → Pago → Tracking. Las alternativas Apple Pay, Google Pay y confirmación de pago se conectaron a Tracking con transición Instantánea.
- **Qué se conservó:** La lámina original como referencia y la disposición visual de las pantallas reconstruidas como frames independientes.
- **Qué se cambió y por qué:** Las seis pantallas se separaron de la lámina estática para que cada una fuera un destino de navegación y pudiera configurarse como inicio de flujo.
- **Pendiente de validación:** Los frames miden 420 × 850, mientras el preset iPhone 15 es 393 × 852; falta comprobar si el escalado o encuadre afecta la presentación. La vista previa quedó cargando/negra durante la comprobación, por lo que no se afirma que el recorrido completo se haya validado en Presentación.

## [2026-10-18] — Auditoría de entrega y correcciones documentales

- **Herramientas:** GitHub, Figma, FigJam y asistente IA.
- **Qué se pidió:** Verificar BRIEF.md, README.md, CHANGELOG.md y el formato de enlaces externos; corregir directamente las carencias detectadas.
- **Qué devolvió:** Se actualizó BRIEF.md con el estado real de evidencia P1/P2, fichas completas, pruebas de aceptación por perfil y restricciones técnicas/ambientales. Este changelog se completó para registrar las intervenciones de diseño, prototipo y documentación. Se confirmó que README.md enlaza a un archivo existente mediante ./BRIEF.md.
- **Qué se conservó:** La transparencia sobre investigación no realizada, las rutas actuales de Figma (figma.com/design/ para el archivo y figma.com/board/ para FigJam) y el enlace relativo del README.
- **Qué se cambió y por qué:** Se sustituyeron criterios generales por tareas medibles para Álvaro y Carlos, se etiquetaron las citas como arquetipos y se mantuvo el objetivo inferior a 400 KB como presupuesto a validar. Se registraron la configuración del prototipo y las limitaciones de su vista previa/dimensiones para no declarar una validación inexistente.
- **Pendiente:** Realizar entrevistas consentidas, recoger y sintetizar evidencias reales, y volver a probar el prototipo en Presentación.

### Entregables

- [Diseño MOMART VIP en Figma](https://www.figma.com/design/BQfZWsTLEAjWKu432GburA/MOMART-VIP-%E2%80%94-MVP)
- [Tablero de investigación y MVP en FigJam](https://www.figma.com/board/NMjzkRlSEGieCYuaP1LJK6/MOMART-VIP-%E2%80%94-Investigaci%C3%B3n-y-MVP)
- [Repositorio momart-vip-mvp](https://github.com/gromerosanchez/momart-vip-mvp)
