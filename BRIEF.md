# Brief de proyecto: MOMART VIP

> Documento de trabajo. Las personas, necesidades y criterios de éxito son hipótesis de diseño pendientes de validación con usuarios y personal de sala. No se incluyen cifras de espera, ruido o errores como datos medidos.

## 1. Problema

MOMART VIP plantea resolver la fricción de pedir bebidas y extras desde un reservado de discoteca: el cliente puede tener que abandonar la mesa para acudir a una barra concurrida, y las peticiones verbales en un entorno ruidoso pueden ser ambiguas. El personal necesita recibir comandas legibles, asociadas a una mesa y con acompañamientos claros.

Estas situaciones constituyen el problema de partida del proyecto y deben contrastarse mediante entrevistas y observación. Las citas de las personas son perfiles de trabajo, no transcripciones de entrevistas reales.

## 2. Solución y alcance del MVP

Aplicación web móvil abierta desde el QR exclusivo de cada reservado, conectada a una cola de comandas en una tablet de barra.

### Incluido en el MVP

- Validar el QR e identificar el número de mesa; ofrecer reintento o entrada manual si el QR o la conexión falla.
- Carta inicial de botellas, copas y extras, con disponibilidad visible.
- Configuración de acompañamientos para botella, hasta un máximo de ocho refrescos.
- Carrito con resumen vinculado a la mesa.
- Pago integrado con los métodos que permita la pasarela seleccionada (tarjeta y, si están disponibles, Apple Pay o Bizum).
- Envío de la comanda a la tablet con mesa, productos, cantidades y acompañamientos.
- Seguimiento con estados Recibido en barra, En preparación y En camino a la mesa.
- Recuperación ante producto agotado, error de pago y pérdida de conectividad sin descartar la configuración del carrito.

### Fuera del MVP

| Funcionalidad | Motivo para posponerla |
| --- | --- |
| Chat directo con el camarero | No es esencial para validar el pedido digital y añade carga de comunicación en hora punta. |
| División de cuenta entre varias personas | Aumenta la complejidad del pago; se puede resolver fuera de la aplicación en la primera versión. |
| Historial de pedidos y fidelización | No es necesario para comprobar el valor inmediato del servicio en mesa. |

## 3. Personas de trabajo

- **Principal — Álvaro Benítez**, 25 años, cliente VIP en Cádiz. Busca pedir desde el móvil con rapidez, permanecer con su grupo y conocer la disponibilidad de productos. Contexto y cita pendientes de validar con clientes reales.
- **Secundaria — Carlos “Charly” Navarro**, 28 años, responsable de barra y apoyo en sala. Necesita comandas inequívocas, cobradas o validadas y asociadas a una mesa. Contexto y cita pendientes de validar con personal real.

## 4. Criterios de éxito propuestos

Metas para pruebas de usabilidad, no resultados alcanzados:

- Al menos el 90 % de participantes completa el happy path sin ayuda.
- Tiempo mediano desde la lectura del QR hasta confirmar el pago inferior a 60 segundos.
- Ningún error de mesa, cantidad o acompañamientos en las tareas de prueba; registrar cualquier fallo y su causa.
- Confirmar con el personal que la comanda de tablet se entiende de un vistazo durante un turno simulado.

Definir tamaño de muestra, método de medición y línea base antes de evaluar el MVP.

## 5. Restricciones y consideraciones

- Acceso desde navegador móvil mediante QR; no requiere instalación desde una tienda de aplicaciones.
- Diseñar para conectividad móvil irregular: objetivo inicial de carga menor de 400 KB, optimización de SVG y tolerancia a reintentos. Medir el peso real y ajustar el presupuesto durante la implementación.
- Priorizar legibilidad, contraste y controles táctiles en baja iluminación. Evaluar un modo oscuro como opción de interfaz; no asumir que por sí solo garantiza ahorro energético.
- Confirmar con el local y el proveedor de pagos los métodos, la operación de la tablet, la gestión de stock y los requisitos legales aplicables antes de producción.

## 6. Investigación pendiente

El tablero de FigJam es una plantilla para recoger entrevistas anonimizadas con consentimiento, comparar referentes y agrupar hallazgos. No contiene entrevistas, benchmarks ni conclusiones validadas todavía. Completarlo con evidencias reales antes de presentar los hallazgos como hechos.

- FigJam: [MOMART VIP — Investigación y MVP](https://www.figma.com/board/NMjzkRlSEGieCYuaP1LJK6/MOMART-VIP-%E2%80%94-Investigaci%C3%B3n-y-MVP)
- Archivo de diseño: [MOMART VIP — MVP](https://www.figma.com/design/BQfZWsTLEAjWKu432GburA/MOMART-VIP-%E2%80%94-MVP)
