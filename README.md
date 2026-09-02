# Taller 1 - Fundamentos Web

## Mi espacio universitario

P谩gina elaborada exclusivamente con HTML5 para Fundamentos Web, grupo 4303, de UNICAMACHO.

## Archivos

- `index.html`: estructura sem谩ntica, textos, enlaces, multimedia, tabla y formulario.
- `multimedia/`: recursos locales usados por la p谩gina.

No se utilizaron CSS, JavaScript, Bootstrap ni frameworks. `audio.mp3` y `video.mp4` quedan referenciados con rutas relativas para que el estudiante agregue recursos autorizados antes de publicar la entrega.

## Explicaci贸n del c贸digo

El contenido visible en el navegador est谩 dentro de `body`: encabezado, navegaci贸n, secciones, enlaces, multimedia, tabla, formulario y pie de p谩gina. El contenido de `title` aparece en la pesta帽a del navegador y en el t铆tulo de la ventana.

`video` reproduce un archivo multimedia local con sus controles. `iframe` incrusta otro documento o servicio externo dentro de la p谩gina. `progress` representa el avance de una tarea conocida; `meter` representa una medida dentro de un rango.

## Verificaci贸n de c贸digo

### Caso A

Problema identificado: `img` no utiliza `href` para indicar la imagen.

Correcci贸n realizada: se utiliz贸 `src="multimedia/estudio.svg"` y un `alt` descriptivo. `img` es un elemento vac铆o y no lleva etiqueta de cierre.

Fuente consultada: [MDN: img](https://developer.mozilla.org/es/docs/Web/HTML/Element/img)

### Caso B

Problema identificado: `a` no utiliza `src` para definir el destino.

Correcci贸n realizada: se utiliz贸 `href="https://developer.mozilla.org/es/docs/Web/HTML"`; los enlaces en pesta帽a nueva incluyen `target="_blank"` y `rel="noopener noreferrer"`.

Fuente consultada: [MDN: a](https://developer.mozilla.org/es/docs/Web/HTML/Element/a)

### Caso C

Problema identificado: `source` utiliza `href`, pero el atributo correcto para el archivo es `src`.

Correcci贸n realizada: se us贸 `<source src="multimedia/video.mp4" type="video/mp4">` dentro de `video`.

Fuente consultada: [MDN: source](https://developer.mozilla.org/es/docs/Web/HTML/Element/source)

### Caso D

Problema identificado: `correo` no es un valor v谩lido para `input type`.

Correcci贸n realizada: se utiliz贸 `type="email"`, que permite reconocer y validar direcciones de correo.

Fuente consultada: [MDN: input email](https://developer.mozilla.org/es/docs/Web/HTML/Element/input/email)

### Caso E

La afirmaci贸n es incorrecta.

Justificaci贸n: la etiqueta est谩ndar es `img`, no `image`. Se escribe con `src` y `alt`, es un elemento vac铆o y no se cierra con `</image>`. En este proyecto funciona, por ejemplo, `<img src="multimedia/estudio.svg" alt="Ilustraci贸n de un espacio de estudio universitario">`.

Fuente consultada: [MDN: img](https://developer.mozilla.org/es/docs/Web/HTML/Element/img)

## Verificaci贸n final

Abrir `index.html` en un navegador permite comprobar la navegaci贸n interna, las im谩genes, la tabla y el formulario. La validaci贸n formal puede realizarse con el [validador HTML del W3C](https://validator.w3.org/). El documento contiene un 煤nico `h1`, controles con `label` y enlaces internos con destinos existentes.

## Lista de comprobaci髇

- Documento con un 鷑ico h1 y estructura HTML5 completa.
- Navegaci髇 interna, enlaces externos y enlace mailto.
- Im醙enes locales con rutas relativas y texto alternativo.
- Tabla con cinco asignaturas y formulario con controles variados.
- Sin hojas de estilo, JavaScript ni frameworks.
