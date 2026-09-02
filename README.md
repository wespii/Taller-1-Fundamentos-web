# Taller 1 - Fundamentos Web

## Mi espacio universitario

Página elaborada exclusivamente con HTML5 para Fundamentos Web, grupo 4303, de UNICAMACHO.

## Archivos

- `index.html`: estructura semántica, textos, enlaces, multimedia, tabla y formulario.
- `multimedia/`: recursos locales usados por la página.

No se utilizaron CSS, JavaScript, Bootstrap ni frameworks. `audio.mp3` y `video.mp4` quedan referenciados con rutas relativas para que el estudiante agregue recursos autorizados antes de publicar la entrega.

## Explicación del código

El contenido visible en el navegador está dentro de `body`: encabezado, navegación, secciones, enlaces, multimedia, tabla, formulario y pie de página. El contenido de `title` aparece en la pestaña del navegador y en el título de la ventana.

`video` reproduce un archivo multimedia local con sus controles. `iframe` incrusta otro documento o servicio externo dentro de la página. `progress` representa el avance de una tarea conocida; `meter` representa una medida dentro de un rango.

## Verificación de código

### Caso A

Problema identificado: `img` no utiliza `href` para indicar la imagen.

Corrección realizada: se utilizó `src="multimedia/estudio.svg"` y un `alt` descriptivo. `img` es un elemento vacío y no lleva etiqueta de cierre.

Fuente consultada: [MDN: img](https://developer.mozilla.org/es/docs/Web/HTML/Element/img)

### Caso B

Problema identificado: `a` no utiliza `src` para definir el destino.

Corrección realizada: se utilizó `href="https://developer.mozilla.org/es/docs/Web/HTML"`; los enlaces en pestaña nueva incluyen `target="_blank"` y `rel="noopener noreferrer"`.

Fuente consultada: [MDN: a](https://developer.mozilla.org/es/docs/Web/HTML/Element/a)

### Caso C

Problema identificado: `source` utiliza `href`, pero el atributo correcto para el archivo es `src`.

Corrección realizada: se usó `<source src="multimedia/video.mp4" type="video/mp4">` dentro de `video`.

Fuente consultada: [MDN: source](https://developer.mozilla.org/es/docs/Web/HTML/Element/source)

### Caso D

Problema identificado: `correo` no es un valor válido para `input type`.

Corrección realizada: se utilizó `type="email"`, que permite reconocer y validar direcciones de correo.

Fuente consultada: [MDN: input email](https://developer.mozilla.org/es/docs/Web/HTML/Element/input/email)

### Caso E

La afirmación es incorrecta.

Justificación: la etiqueta estándar es `img`, no `image`. Se escribe con `src` y `alt`, es un elemento vacío y no se cierra con `</image>`. En este proyecto funciona, por ejemplo, `<img src="multimedia/estudio.svg" alt="Ilustración de un espacio de estudio universitario">`.

Fuente consultada: [MDN: img](https://developer.mozilla.org/es/docs/Web/HTML/Element/img)

## Verificación final

Abrir `index.html` en un navegador permite comprobar la navegación interna, las imágenes, la tabla y el formulario. La validación formal puede realizarse con el [validador HTML del W3C](https://validator.w3.org/). El documento contiene un único `h1`, controles con `label` y enlaces internos con destinos existentes.
