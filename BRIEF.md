# Brief de proyecto: MOMART VIP

> Documento de trabajo. Las personas, citas y necesidades son arquetipos de diseño, no transcripciones. No se han realizado todavía entrevistas ni pruebas; por tanto, no se presentan datos de investigación como resultados.

## 1. Problema e hipótesis de investigación (P1 y P2)

En una discoteca concurrida, quien ocupa un reservado puede tener que dejar su mesa para pedir en una barra saturada. En el entorno de ruido y poca luz, las peticiones verbales también pueden llegar incompletas. El personal necesita identificar con rapidez la mesa, el producto y los acompañamientos para preparar y entregar la comanda correctamente.

Estas afirmaciones son hipótesis del proyecto, aún no hallazgos demostrados. Las fichas de Álvaro y Carlos de la sección 3 guían la investigación; sus citas son frases de arquetipo redactadas para el diseño, no citas de personas entrevistadas.

| Participante previsto | Hipótesis que se debe contrastar | Evidencia pendiente |
| --- | --- | --- |
| P1 — cliente de reservado, perfil de Álvaro | Pedir sin abandonar el reservado aporta valor; QR, disponibilidad visible y pago breve son comprensibles en condiciones de cobertura y luz limitadas. | Entrevista consentida y prueba de tarea; registrar conducta, tiempo, errores y observaciones sin datos identificativos. |
| P2 — personal de barra/sala, perfil de Carlos | Una comanda digital vinculada a mesa y con cantidades de acompañamientos reduce ambigüedad y se puede procesar en hora punta. | Entrevista consentida y simulación en tablet; registrar comprensión, errores y tiempo de identificación/preparación. |

**Estado de evidencia:** entrevistas, observación, benchmark y mediciones reales pendientes. El tablero de FigJam es una plantilla y no contiene resultados validados. No se han inventado cifras de espera, ruido, conversión ni errores.

## 2. Solución y alcance del MVP

Aplicación web móvil accesible desde el QR exclusivo de cada reservado, conectada a una cola de comandas para la tablet de barra.

### Dentro del MVP

- Validar el QR e identificar la mesa; permitir reintento y alternativa si falla el QR o la conexión.
- Mostrar una carta inicial de botellas, copas y extras con disponibilidad.
- Configurar hasta ocho refrescos de acompañamiento por botella.
- Resumir la comanda en un carrito asociado a la mesa.
- Facilitar el pago con los métodos disponibles en la pasarela elegida (tarjeta y, si el proveedor y el dispositivo lo permiten, Apple Pay o Bizum).
- Enviar a barra una comanda pagada o validada, con mesa, artículos, cantidades y acompañamientos.
- Mostrar seguimiento con los estados «Recibido en barra», «En preparación» y «En camino a la mesa».
- Conservar la configuración del carrito ante errores de pago, falta de stock o pérdida de conectividad, y ofrecer una acción de recuperación.

### Pospuesto / fuera del MVP

| Funcionalidad | Motivo para posponerla |
| --- | --- |
| Chat directo con el camarero | No es esencial para validar el pedido digital y añade carga de comunicación en hora punta. |
| División de cuenta entre varias personas | Aumenta la complejidad del pago; puede resolverse fuera de la aplicación inicialmente. |
| Historial de pedidos y fidelización | No es necesario para comprobar el valor inmediato del servicio en mesa. |
| Propinas complejas | No son necesarias para validar el recorrido principal y complican el checkout. |

## 3. Fichas de personas

### Persona primaria — Álvaro Benítez

- **Perfil:** 25 años, ingeniero de software, Cádiz; cliente de reservado VIP.
- **Contexto:** iPhone 15; 4G con cobertura irregular; discoteca con ruido elevado y poca luz; sábado, entre las 02:30 y las 05:00.
- **Objetivos:** pedir una botella o hielo en menos de un minuto sin levantarse; disfrutar del reservado y justificar su coste; mantener su estatus sin hacer cola.
- **Frustraciones:** barra general masificada; dificultad para oír al camarero; desconocimiento de marcas disponibles.
- **Cita-arquetipo (no entrevista):** «He pagado 250 € por un reservado para estar cómodo con mis amigos; no quiero perder 20 minutos haciendo cola en la barra ni llevarme empujones para pedir una botella.»
- **Etiquetas:** Cliente VIP · Inmediatez · Móvil-first.

### Persona secundaria — Carlos Navarro

- **Perfil:** 28 años, responsable de barra y apoyo en sala, San Fernando (Cádiz); personal de Momart.
- **Contexto:** tablet táctil TPV o móvil de trabajo; Wi-Fi interna; detrás de la barra, con ritmo frenético y ruido extremo; turno de noche en hora punta.
- **Objetivos:** recibir comandas pagadas o validadas y asociadas a mesa; aumentar la rotación sin colapsar la barra; evitar errores de acompañamientos y quejas.
- **Frustraciones:** clientes VIP reclamando en la barra; notas manuales o peticiones verbales ambiguas por el ruido.
- **Cita-arquetipo (no entrevista):** «En plena hora punta necesito una comanda clara en pantalla que me diga “Mesa 4: 1 Ginebra + 8 Sprite” para prepararlo y servirlo en 2 minutos sin líos.»
- **Etiquetas:** Staff Momart · Gestión de comandas · Pantalla táctil.

## 4. Criterios de éxito y pruebas verificables (RA6-e / RA6-f)

Los siguientes son objetivos de aceptación propuestos, no resultados obtenidos. Antes de evaluar, reclutar al menos cinco participantes por perfil, obtener consentimiento, definir el protocolo y registrar resultados agregados y errores observados.

| Persona y tarea de prueba | Medida | Umbral propuesto |
| --- | --- | --- |
| P1 / Álvaro: desde el QR de prueba, localizar una botella, configurar ocho acompañamientos y confirmar el pedido en un móvil. | Finalización independiente y tiempo desde QR hasta confirmación del pago simulado. | Al menos 4 de 5 participantes completan sin ayuda; mediana inferior a 60 segundos. |
| P1 / Álvaro: repetir la tarea con un fallo simulado de conexión, pago rechazado o producto agotado. | Conservación del carrito y recuperación sin perder acompañamientos. | 5 de 5 conservan la selección; registrar y revisar cada error crítico. |
| P2 / Carlos: localizar una comanda de prueba en tablet e identificar mesa, producto, cantidades y acompañamientos; marcarla como lista. | Exactitud de los campos y tiempo para identificar la información. | 5 de 5 identifican todos los campos sin error en un máximo de 15 segundos. |
| P2 / Carlos: procesar varias comandas de prueba en una simulación de hora punta. | Comandas asociadas a mesa y preparadas con cantidades correctas. | Cero errores críticos de mesa, producto o acompañamientos en la ronda; documentar cualquier incidencia. |

Los resultados se informarán como observaciones del tamaño de muestra indicado, no como garantía de error cero en producción. Revisar los umbrales después del piloto y contrastarlos con línea base real del local.

## 5. Restricciones técnicas y ambientales

- Acceso desde navegador móvil mediante QR; no requiere instalación desde una tienda de aplicaciones.
- Diseñar para cobertura móvil irregular, reintentos y preservación local del carrito durante errores recuperables.
- Presupuesto ambiental inicial del proyecto: carga inicial inferior a **400 KB transferidos** (definir y medir con compresión acordada, caché vacía y una herramienta reproducible). Es un objetivo de diseño por validar, no un límite normativo atribuido a W3C.
- Reducir transferencia y procesamiento: optimizar SVG, limitar recursos de terceros y cargar solo los recursos necesarios para el recorrido inicial. Contrastar las decisiones con las Web Sustainability Guidelines, criterio 2.4.
- Priorizar contraste, legibilidad y controles táctiles en baja iluminación. Evaluar un modo oscuro; no afirmar ahorro energético sin medición en los dispositivos objetivo.
- Confirmar con el local y el proveedor de pagos los métodos admitidos, la operación del TPV, la gestión de stock y los requisitos legales antes de producción.

### Referencias de trabajo

- [FigJam — investigación y definición del MVP](https://www.figma.com/board/NMjzkRlSEGieCYuaP1LJK6/MOMART-VIP-%E2%80%94-Investigaci%C3%B3n-y-MVP)
- [Archivo de diseño en Figma](https://www.figma.com/design/BQfZWsTLEAjWKu432GburA/MOMART-VIP-%E2%80%94-MVP)
