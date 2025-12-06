# CRUDScope – HTML MediaPanel

## Descripción general

`CRUDScope – HTML MediaPanel` es un proyecto pequeño que simula un panel de gestión de tareas (CRUD) con foco didáctico. La página se diseñó para practicar y demostrar el uso de etiquetas HTML5 semánticas, formularios y elementos multimedia, manteniendo una estructura clara y accesible.

## Investigación de etiquetas
Abajo agrupo las etiquetas usadas en el proyecto por categoría; para cada grupo indico para qué se usan y un caso típico.

- **Estructura:** `html`, `head`, `body`, `title`, `meta`, `base`.
	- Uso: Definen la estructura global y metadatos del documento.
	- Caso típico: Configurar título, codificación y (opcionalmente) una URL base para enlaces relativos.

- **Semánticas:** `header`, `nav`, `main`, `section`, `article`, `aside`, `footer`, `address`, `time`.
	- Uso: Dan significado a las secciones de la página, facilitando accesibilidad y SEO.
	- Caso típico: Encapsular el menú en `nav`, y el contenido principal en `main` dividido por `section`.

- **No semánticas:** `div`, `span`.
	- Uso: Contenedores genéricos para layout o estilos cuando no existe una etiqueta semántica apropiada.
	- Caso típico: Agrupar elementos para aplicar estilos CSS o scripts.

- **Texto:** `h1`–`h3`, `p`, `strong`, `em`, `u`, `mark`, `abbr`.
	- Uso: Marcar jerarquía y formatos textuales (títulos, énfasis, abreviaturas, resaltes).
	- Caso típico: `abbr` para siglas con `title`, `mark` para destacar fragmentos importantes.

- **Tablas:** `table`, `thead`, `tbody`, `tr`, `th`, `td`.
	- Uso: Mostrar datos tabulares; `thead`/`tbody` mejoran semántica y accesibilidad.
	- Caso típico: Listados de tareas con columnas de fecha, prioridad y acciones.

- **Formularios:** `form`, `label`, `input`, `textarea`, `button`, `select`, `option`.
	- Uso: Capturar datos del usuario y controlar su envío.
	- Caso típico: Formulario para crear o editar una tarea con campos `title`, `description` y `date`.

- **Multimedia:** `img`, `audio`, `video`, `source`.
	- Uso: Integrar imágenes y reproductores de audio/video nativos en la página.
	- Caso típico: Video demostrativo del sistema y audios tutoriales.

## Diferencias entre etiquetas semánticas y no semánticas

Las etiquetas semánticas describen el propósito del contenido (por ejemplo `header` indica un encabezado de página). Esto mejora la accesibilidad (lectores de pantalla), el SEO y la mantenibilidad del código.

Las etiquetas no semánticas (`div`, `span`) no aportan significado por sí mismas; se usan para estructura visual o para envolver elementos cuando no existe una etiqueta semántica adecuada.

Ejemplos:
- Usar `nav` para agrupar la navegación principal (correcto y recomendable).
- Usar `div` para crear un contenedor flexible cuando se necesita un layout específico que no tiene una etiqueta semántica directa.

## Enfoque en etiquetas poco comunes

- **`<base>`**
	- Qué hace: establece una URL base para todas las URLs relativas del documento (enlaces, `src`, `href`).
	- Cómo afecta: si `base` apunta a un dominio o ruta distinta, el navegador resolverá todas las referencias relativas en base a esa URL, lo que puede romper la carga local de recursos si no se pretende.
	- Recomendación: usar `base` solo cuando realmente necesites que todas las rutas relativas dependan de una base diferente; en proyectos simples locales suele ser mejor no incluirla.

- **`<abbr>`**
	- Qué hace: marca abreviaturas o siglas y permite añadir descripción con `title` para que el lector vea el significado completo al pasar el cursor o al acceder por tecnologías de asistencia.
	- Ejemplo: `<abbr title="Create, Read, Update, Delete">CRUD</abbr>`.

- **`<time>`**
	- Qué hace: representa fechas y horas en formato legible y, opcionalmente, en un formato `datetime` legible por máquinas.
	- Ventaja: facilita el parseo automático de fechas por herramientas y mejora la semántica temporal en el documento.

## Ventajas de usar etiquetas multimedia en vez de solo enlaces

- Integración nativa: `audio` y `video` ofrecen controles integrados (play/pause, volumen, subtítulos) sin depender de reproductores externos.
- Accesibilidad: permiten añadir subtítulos, transcripciones y descripciones que mejoran la experiencia para usuarios con discapacidades.
- Experiencia de usuario: se puede controlar el comportamiento (autoplay con `muted`, `loop`, `controls`) y ofrecer reproducción inline.

## Referencias

- MDN Web Docs — HTML: https://developer.mozilla.org/docs/Web/HTML
- W3C — HTML Living Standard: https://html.spec.whatwg.org/
- MDN — Accessibility: https://developer.mozilla.org/docs/Learn/Accessibility
- Arg: Artículo sobre semántica HTML (ejemplo educativo): https://developer.mozilla.org/en-US/docs/Glossary/Semantics
- Google Fonts — integración de tipografías: https://fonts.google.com/

---

Si querés, dejo este `README.md` con formato adicional (íconos, ejemplos de código más extensos o una tabla de contenidos). ¿Querés que incluya alguna referencia específica que usaste durante el trabajo?