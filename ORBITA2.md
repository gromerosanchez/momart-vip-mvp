# Órbita 2: sistema visual de MOMART VIP

> **Estado de la entrega:** se aplicaron cambios directamente al archivo de Figma mediante MCP y se verificó su persistencia por lectura del documento. Los wireframes, mockups y componentes incluyen contenido editable y estructuras iniciales de Auto Layout; no constituyen una entrega visual completamente validada. Los assets de producto/imágenes siguen siendo placeholders. El contraste del estado Default del botón primario se corrigió a 5,94:1 en Claro y 11,47:1 en Oscuro; falta auditar otros estados y combinaciones. En `05 — Mockups` se verificó la retícula `Grid / Mobile (4 cols - 16px gutter - 16px margin)` aplicada a seis pantallas móviles y el prototipo navegable de seis pasos. El punto inicial sigue apareciendo como `Flow 1`: el nombre del punto de flujo es de solo lectura en la API MCP disponible. No se completaron mockups móviles de alta fidelidad.

## Enlaces

| Qué | Enlace |
|---|---|
| Archivo de Figma (versión "Entrega Órbita 2") | https://www.figma.com/design/BQfZWsTLEAjWKu432GburA/MOMART-VIP-%E2%80%94-MVP |
| Prototipo móvil en mockups | https://www.figma.com/proto/BQfZWsTLEAjWKu432GburA/MOMART-VIP-%E2%80%94-MVP?node-id=189-2&starting-point-node-id=189%3A2&scaling=scale-down |
| Proyecto de Google Stitch (solo si lo has usado) | No se ha utilizado Google Stitch |

## Dónde está cada cosa en Figma

| Entregable | Página y sección del archivo |
|---|---|
| Inventario de decisiones | Página `04 — Wireframes`, dentro de `Orbit 2 · Wireframe Deliverables` |
| Wireframes rediseñados con sus notas | Página `04 — Wireframes`, dentro de `Orbit 2 · Wireframe Deliverables`; incluye seis pasos móviles del cliente y variantes de escritorio para cliente y staff |
| Componentes | Página `03 — Componentes`, frame `Orbit 2 · Auto Layout Components`; seis componentes independientes, set `Button / Primary` de seis estados y dos iconos auxiliares |
| Mockups del happy path | Página `05 — Mockups`; incluye mockups de escritorio para cliente y staff/pedidos y seis pantallas móviles duplicadas de los wireframes |
| Prototipo móvil interactivo | Páginas `05 — Mockups` (inicio `189:2`) y `06 — Prototipo` (inicio `183:3`); ambas recorren los seis pasos con cinco transiciones |
| Pantalla principal a 1280 px | Página `05 — Mockups`; variantes cliente Claro/Oscuro de 1280 × 620 px con Auto Layout WRAP y tarjetas FILL |
| Pantallas en modo oscuro | Páginas `04 — Wireframes` y `05 — Mockups`; las variantes oscuras de cliente/staff y la nueva variante responsive están mapeadas a `Semánticos · Oscuro` |
| Guía de estilo | Página `02 — Guía de Estilo`, frame `Orbit 2 · Style Guide Content`; incluye tablas Auto Layout de contraste y mapeo HTML semántico |

## Lista de comprobación de Figma

Las casillas indican requisitos completados y verificados en el archivo, no intención. Las páginas oficiales ya existentes se reutilizaron sin duplicarlas. El material útil de las tres páginas redundantes se migró o comprobó en las páginas oficiales antes de eliminar solo esos tres IDs; las páginas originales de Órbita 1 permanecen.

- [x] Colección `Primitivos`: escalas de color Gold, Slate, Success, Error y Warning (10 tonos cada una), 8 tokens de espaciado con scope `GAP` y 8 radios con scope `CORNER_RADIUS`; variables con descripción y sintaxis WEB.
- [x] Colección `Semánticos`: modos `Claro` y `Oscuro`, 12 alias cromáticos hacia variables de `Primitivos`, con scopes, descripciones y sintaxis CSS.
- [x] Siete estilos tipográficos Inter (display, heading-1 a heading-3, body, label, caption) y tres estilos de efecto de elevación creados.
- [x] Estilo local `Grid / Mobile (4 cols - 16px gutter - 16px margin)` (4 columnas, gutter 16 px, offset/márgenes 16 px, alineación `STRETCH`) aplicado y leído por `gridStyleId` en los seis frames móviles de `05 — Mockups` (`189:2`, `189:14`, `189:26`, `189:38`, `189:50`, `189:62`); los wireframes originales no se modificaron.
- [ ] Vincular el estilo de retícula a variables; sus valores siguen siendo fijos.
- [x] Seis componentes funcionales independientes y un set `Button / Primary` de seis estados en Auto Layout; se añadieron dos componentes auxiliares de icono para la propiedad de intercambio.
- [x] El botón primario tiene variantes `Default`, `Hover`, `Focus`, `Pressed`, `Disabled` y `Loading`, propiedad de texto `Label`, propiedad de intercambio `Icon` y opción `Show icon`. `Focus` tiene un contorno exterior de 2 px; estados y propiedad `State` leídos de nuevo en el set.
- [ ] Variantes y propiedades completas del resto de componentes.
- [x] Tabla de contraste y tabla de mapeo HTML semántico añadidas a `02 — Guía de Estilo` con Auto Layout e Inter.
- [x] Contraste del botón `Default`: texto `#F8FAFC` sobre `action/primary` `#7D5A30` da 5,94:1 en Claro; texto `#0F172A` sobre `#E7CC98` da 11,47:1 en Oscuro.
- [ ] Auditoría WCAG AA de todas las demás combinaciones y estados (incluidos Hover, Pressed y Disabled).
- [ ] Mockups móviles 1.0–6.0 completos, con todos sus espacios vinculados a variables; las seis pantallas del prototipo son copias wireframe, no mockups terminados.
- [ ] Reutilización de los mismos componentes validada entre anchos de escritorio. Se añadieron variantes responsive específicas, pero las tarjetas son frames Auto Layout, no instancias del sistema de componentes.
- [x] Variantes cliente Claro/Oscuro de `1280 × 620 px` en `05 — Mockups` (`190:2`, `190:33`): contenedor y fila de tarjetas con Auto Layout `WRAP`, tres tarjetas `FILL` simétricas (310,67 px cada una a 1280 px; ancho mínimo 180 px). Una prueba temporal a 700 px verificó dos tarjetas de 181 px y una tercera en la fila siguiente; se restauró y leyó el ancho final de 1280 px.
- [x] Legibilidad del contenido de la variante Claro: se enlazó la superficie de productos a `action/primary` (`#7D5A30`) y sus títulos/resúmenes a `action/primary-text` (`#F8FAFC`), contraste 5,94:1; la lectura visual posterior mostró los textos con contraste legible.
- [x] Se asignó explícitamente `Semánticos · Oscuro` a `Customer desktop · Oscuro` (`162:337`), `Staff orders desktop · Oscuro` (`162:388`) y `Customer desktop · Oscuro · 1280px responsive` (`190:33`). Los colores semánticos coincidentes quedaron enlazados a variables; el CTA usa `action/primary` (`#E7CC98`) y texto `action/primary-text` (`#0F172A`).
- [ ] Todos los mockups comprobados cambiando el selector global de tema y las pruebas de visibilidad en Oscuro. La asignación/mapeo de los tres frames oscuros anteriores no sustituye una prueba global de todos los mockups.
- [x] Prototipo cliente que recorre los seis pasos en `05 — Mockups` (`189:2`) y `06 — Prototipo` (`183:3`): cinco transiciones `ON_CLICK`/`NAVIGATE` y punto inicial `Flow 1` en cada página, confirmados por lectura posterior.
- [ ] Nombre solicitado `Flujo Principal MOMART VIP` para el punto inicial de `05 — Mockups`: MCP confirma `189:2` como inicio, pero `flowStartingPoints[0].name` es de solo lectura; el nombre persistente continúa siendo `Flow 1`.
- [ ] Prueba 1 superada: al cambiar `color/primary`, cambian todas las pantallas a la vez.
- [ ] Prueba 2 superada: con todos los mockups en modo oscuro, nada desaparece contra el fondo.

**Lectura de Figma (MCP):** se leyeron 90 variables locales: 78 en `Primitivos` y 12 en `Semánticos`, con modos `Claro` y `Oscuro` para los alias semánticos. También se verificaron 11 estilos de texto locales (7 de Órbita 2 y 4 previos) y 3 estilos de efecto. En `03 — Componentes` hay seis componentes funcionales independientes, un set de botón primario con seis variantes y dos componentes auxiliares de icono. Las seis variantes usan Auto Layout, los fills/textos conservan enlaces a variables, y se verificaron las propiedades `State`, `Label`, `Icon` y `Show icon`. En `02 — Guía de Estilo` se verificaron dos tablas Auto Layout con tipografía Inter. Las referencias de contraste se recalcularon contra los colores resueltos reales: 4,55:1, 6,96:1 y 5,75:1 para las tres parejas proporcionadas con colores disponibles; `#D4AF37` no existe como token. Las seis páginas originales y las cuatro páginas oficiales se leyeron de nuevo después de la limpieza.

**Lectura adicional (MCP, 2026-11-08):** en `05 — Mockups` se leyeron los seis nuevos frames móviles de 304 × 450 px con el estilo de retícula aplicado, los cinco enlaces entre pantallas y `Flow 1` en `189:2`. Las nuevas variantes cliente `190:2` y `190:33` se verificaron a 1280 × 620 px. El contenedor y la fila de tarjetas usan WRAP; en la fila, tres tarjetas de ancho FILL se reparten simétricamente a 310,67 px. La prueba temporal a 700 px produjo dos tarjetas de 181 px y una tercera en la fila siguiente; el ancho se restauró a 1280 px. La lectura visual de ambas variantes confirmó que títulos, productos, precios y CTA permanecen visibles. Las variantes oscuras `162:337`, `162:388` y `190:33` tienen modo explícito Oscuro y colores semánticos coincidentes enlazados; no se ha probado el cambio global del tema para todos los mockups. Las variantes usan frames existentes y no instancias compartidas de componentes.

**Actualización de lectura MCP (2026-11-08, posterior):** el estilo aplicado a los seis frames de `05 — Mockups` se renombró al texto exacto `Grid / Mobile (4 cols - 16px gutter - 16px margin)` y se verificó que cada frame mantiene el `gridStyleId` de ese estilo (4 columnas, gutter y offset de 16 px, `STRETCH`). `Button / Primary` ahora tiene y lee las seis variantes `Default`, `Hover`, `Focus`, `Pressed`, `Disabled` y `Loading`; `Focus` se añadió con contorno exterior de 2 px. Se volvieron a leer cinco reacciones `ON_CLICK`/`NAVIGATE` en los cinco botones de avance. El inicio sigue en `189:2`, pero no se pudo renombrar: la API MCP devuelve el campo `flowStartingPoints[0].name` como de solo lectura, por lo que `Flow 1` persiste. Esta lectura posterior sustituye cualquier nombre antiguo del estilo o recuento anterior de variantes; no elimina el historial de cambios de las entradas fechadas más abajo.

## Resumen de decisiones

### Rediseño de los wireframes

En los wireframes se representó el flujo móvil de seis pasos para el cliente, junto con vistas de escritorio para cliente y staff. La propuesta central de las pantallas 3.0 (Configurador de refrescos) y 4.0 (Carrito) es un contador visible ("8 de 8 seleccionados") y un CTA con acción explícita. Los wireframes son editables, pero falta completar mockups móviles de todo el flujo y validar las decisiones con Álvaro Benítez y Carlos Navarro.

### Color

- **Color principal propuesto:** Gold / Dorado, asociado a la identidad premium del reservado de Momart. En los tokens actuales, `action/primary` resuelve a `#7D5A30` (`primitive/gold/700`) en modo Claro y `#E7CC98` (`primitive/gold/300`) en Oscuro.
- **Color secundario propuesto:** Slate / Carbón neutro (`slate-700` / `#334155`).
- **Contraste verificado contra los tokens actuales de Figma:** `primitive/slate/500` (`#64748B`) sobre `primitive/slate/50` (`#F8FAFC`) = **4,55:1**; `primitive/slate/400` (`#94A3B8`) sobre `primitive/slate/900` (`#0F172A`) = **6,96:1**; `primitive/slate/900` (`#0F172A`) sobre `primitive/gold/500` (`#B68B45`) = **5,75:1**. La pareja de referencia `#0F172A` / `#D4AF37` y el valor `8,49:1` quedan **sin verificar**, porque `#D4AF37` no existe en las variables actuales. Para el botón `Default`, `action/primary-text` (`#F8FAFC`) sobre `action/primary` (`#7D5A30`) = **5,94:1** en Claro; `#0F172A` sobre `#E7CC98` = **11,47:1** en Oscuro. No se afirma que todas las combinaciones o estados de la interfaz cumplan AA.

### Tipografía

Se propone la familia Inter en dos pesos: Regular (400) y Semi Bold (600). Su altura de x y la diferenciación de caracteres ayudan a leer precios y números de comanda en móvil, con poca luz y prisa. Limitar los pesos reduce descargas, pero el presupuesto total de transferencia (incluidas las fuentes) debe medirse; no se da por verificado aquí ningún umbral de sostenibilidad.

### Espaciado y retícula

- **Base propuesta:** escala de 4 px con pasos principales de 8 px. Tokens: `space/4` (4 px), `space/8` (8 px), `space/12` (12 px), `space/16` (16 px), `space/24` (24 px), `space/32` (32 px), `space/48` (48 px) y `space/64` (64 px). El script aplica el ámbito `GAP` de Figma a estas variables.
- **Retícula móvil propuesta (iPhone 15 / 393 px):** 4 columnas, medianil de 16 px y márgenes laterales de 16 px. Diseñar objetivos táctiles de al menos 44 × 44 px y validar la implementación y el criterio de accesibilidad aplicable antes de darlo por cumplido.

### Componentes

En `03 — Componentes` hay seis componentes independientes de Auto Layout y el botón primario se convirtió en un set de seis variantes:

- `Button / Primary`: `Default`, `Hover`, `Focus`, `Pressed`, `Disabled` y `Loading`. `Focus` tiene un contorno exterior de 2 px. Tiene Auto Layout, enlace de color a `action/primary`, enlace de texto a `action/primary-text`, propiedad de texto `Label`, propiedad de intercambio de instancia `Icon` y propiedad booleana opcional `Show icon`.
- `Button / Secondary`.
- `Badge / Order status`.
- `Card / Product`.
- `Row / Cart item`.
- `Card / Order summary`.
- `Navigation / Category tabs`.
- `Icon / Arrow right` y `Icon / Loading` como opciones auxiliares de intercambio de instancia, agrupadas en Auto Layout.

La propiedad `Show icon` oculta el icono opcional por defecto; se añadió una marca visual de puntos a la variante Loading. No se verificaron variantes/propiedades para el resto de componentes. Se corrigió el token semántico de acción primaria para Claro: ahora referencia `primitive/gold/700` (`#7D5A30`), con texto `#F8FAFC`, y el estado Default alcanza 5,94:1. Hover, Focus, Pressed, Disabled y el resto de combinaciones aún necesitan auditoría.

### Tablas de la guía de estilo

`02 — Guía de Estilo` contiene dos tablas construidas con Auto Layout e Inter: una registra contrastes calculados a partir de los colores reales de Figma y una nota que distingue colores heredados de tokens activos; la otra relaciona patrones de interfaz con elementos HTML semánticos y notas de accesibilidad.

### Responsive y modo oscuro

- **Segundo ancho:** en `05 — Mockups` se añadieron variantes de cliente de 1280 × 620 px con fila de producto WRAP y tarjetas FILL simétricas. Se comprobó el reflow temporalmente a 700 px y se restauró el ancho de 1280 px. La reutilización de instancias de componentes entre anchos sigue pendiente.
- **Modo oscuro:** los frames oscuros de cliente y staff (`162:337`, `162:388`) y la variante responsive `190:33` tienen el modo `Semánticos · Oscuro` y sus colores coincidentes enlazados a variables. Falta probar el cambio global del selector en todos los mockups y completar el mapeo/verificación visual del resto de pantallas.

## Uso de IA

Se utilizó asistencia de IA en VS Code y el MCP oficial de Figma para estructurar las variables, estilos, componentes, wireframes y mockups. Los cambios se verificaron mediante lectura del archivo de Figma. `figma_setup.js` y `figma-orbit2-plugin/` son alternativas locales generadas antes de contar con escritura MCP; no se ejecutaron en este archivo.

## Lo que ha quedado pendiente

Queda pendiente: cambiar el nombre del punto inicial de `Flow 1` a `Flujo Principal MOMART VIP` (la API MCP consultada expone el nombre como solo lectura); vincular a variables los valores del estilo de retícula; definir y revisar variantes/propiedades del resto de componentes; completar los mockups móviles de alta fidelidad y sus espacios vinculados; reutilizar instancias de componentes entre anchos de escritorio; probar el cambio global de tema en todos los mockups y las pruebas de visibilidad en oscuro; auditar el contraste de Hover/Focus/Pressed/Disabled y todas las demás combinaciones. El prototipo navegable de seis pasos y el reflow de las tarjetas a 700 px se verificaron; las capas de producto y las imágenes siguen siendo scaffolds/placeholders. También queda pendiente la implementación en HTML5/CSS3 y la optimización de assets SVG para Órbita 3.

## Páginas redundantes eliminadas

Se eliminaron únicamente `07 — Orbit 2 · Foundations` (ID `150:2`), `08 — Orbit 2 · Screen Scaffolds` (ID `152:19`) y `09 — Orbit 2 · Components` (ID `152:20`), después de migrar o confirmar lo útil en las páginas oficiales. La paleta histórica y la escala anterior se anotaron en `02 — Guía de Estilo` y sus valores legacy permanecen en variables; los seis pasos móviles y las operaciones staff/POS ya están representados en `04 — Wireframes` y `05 — Mockups`; el inventario de acciones, navegación, producto, pedido, estado y staff se conservó como nota de patrones pendientes en `03 — Componentes`. Se verificó después que las seis páginas originales de Órbita 1 y las cuatro páginas oficiales siguen presentes.
