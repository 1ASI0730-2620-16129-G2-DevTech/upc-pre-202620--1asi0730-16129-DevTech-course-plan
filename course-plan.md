# Fundamentos de Desarrollo Web

## Resumen del Curso

Este curso de 1 hora te enseña a crear tu propia página web desde cero usando **HTML** (el contenido) y **CSS** (el estilo). Al final tendrás una **página de perfil personal** hecha por ti. **¡No requiere descargas!** Solo abre tu navegador web.

**Duración total**: ~61 minutos (7 lecciones cortas)
**Público objetivo**: Estudiantes de 12 a 17 años sin experiencia en programación
**Prerrequisitos**: Ninguno. Si sabes usar un navegador, ¡ya puedes empezar!
**Herramientas necesarias**: **¡Solo tu navegador web!** (Chrome, Firefox, Safari, Edge) y un editor en línea gratuito
**💻 Editores en línea**: todas las prácticas vienen **precargadas en [JSFiddle](https://jsfiddle.net/)**: abres el enlace y el código ya está listo. No necesitas registrarte.
Si prefieres otro editor, también puedes usar [CodePen](https://codepen.io/pen/) (no necesita registro para practicar) o [Replit](https://replit.com/) (pide una cuenta gratuita). Solo copia el código de inicio desde la carpeta `starter-files` del repositorio.

**📂 Repositorio de código fuente**: [https://github.com/1ASI0730-2620-16129-G2-DevTech/upc-pre-202620--1asi0730-16129-DevTech-course-plan/tree/main](https://github.com/1ASI0730-2620-16129-G2-DevTech/upc-pre-202620--1asi0730-16129-DevTech-course-plan/tree/main)

## Secuencia de Lecciones
### Lección 1: ¿Qué es un sitio web? (6 minutos)

- **Descripción**: Descubre qué es un sitio web, en qué se diferencia de una página web y cómo trabajan el navegador y el servidor. Conoce las funciones de HTML, CSS y JavaScript, escribe tu primer código y aprende a evitar cuatro errores comunes al comenzar.
- **Enlace**: [Youtube](https://youtu.be/yLvqD2b4_Uw/)
- **Conceptos clave**:
  - Un sitio web reúne páginas relacionadas, como un libro reúne sus páginas.
  - El navegador solicita archivos al servidor y los interpreta para mostrar la página.
  - HTML organiza el contenido, CSS define la apariencia y JavaScript agrega interactividad.
  - `<h1>` representa un título principal y `<p>` representa un párrafo.
  - HTML es un lenguaje de marcado. Puedes consultar documentación, revisar los detalles del código y aprender paso a paso sin memorizarlo todo.
- **Práctica**: [Vamos a practicar](https://jsfiddle.net/GabrielRamirez/zca381ob/) 👈 **¡No necesitas instalar nada!**
  - Cambia el título por tu nombre o el nombre de tu página, personaliza el primer párrafo y agrega un segundo párrafo.
  - ¿Prefieres otro editor? Copia el código de `starter-files/leccion-01` en [JSFiddle](https://jsfiddle.net/), [CodePen](https://codepen.io/pen/) o [Replit](https://replit.com/).
  - Si el editor tiene un panel HTML separado, copia solo el contenido de `<body>`. Si utiliza un archivo `index.html` completo, conserva toda la estructura.

### Lección 2: El esqueleto de una página (9 minutos)

- **Descripción**: Aprende qué son las etiquetas, los elementos y los atributos, y arma la estructura básica que tiene toda página web. Se usa la analogía de un sándwich para entender cómo se abren y se cierran las etiquetas.
- **Enlace**: [YouTube](https://youtu.be/kZWn6u8JLGI)
- **Conceptos clave**:
  - Estructura básica: `<!DOCTYPE html>`, `<html>`, `<head>`, `<body>`, `<title>`
  - Etiqueta de apertura `<p>`, de cierre `</p>`, y etiquetas vacías como `<img>`
  - Los atributos dan información extra: `<html lang="es">`
  - Toda etiqueta que se abre debe cerrarse
- **Práctica**: [Vamos a practicar!](https://jsfiddle.net/czg03pou/3/) 👈 **¡No necesitas instalar nada!**
  - ¿Prefieres otro editor? Copia el código de `starter-files/leccion-02` en [JSFiddle](https://jsfiddle.net/), [CodePen](https://codepen.io/pen/) o [Replit](https://replit.com/).

### Lección 3: Llenando la página (10 minutos)

- **Descripción**: Agrega contenido a tu página creando "Mis cosas favoritas": títulos de distintos tamaños, párrafos, listas con puntos y numeradas, una imagen desde internet y un enlace a otro sitio.
- **Enlace**: [YouTube](https://youtu.be/fqDidSU5MJg)
- **Conceptos clave**:
  - Títulos y párrafos: `<h1>` a `<h6>`, `<p>`
  - Listas: `<ul>`, `<ol>`, `<li>`
  - Imágenes: `<img src="..." alt="...">`
  - Enlaces: `<a href="...">texto</a>`
  - El atributo `alt` en imágenes es importante para la accesibilidad
- **Práctica**: [Vamos a practicar!](https://jsfiddle.net/czg03pou/4/) 👈 **¡Empieza al instante!**
  - ¿Prefieres otro editor? Copia el código de `starter-files/leccion-03` en [JSFiddle](https://jsfiddle.net/), [CodePen](https://codepen.io/pen/) o [Replit](https://replit.com/).

### Lección 4: Dale estilo con CSS (9 minutos)

- **Descripción**: Aprende qué es CSS y cómo conectarlo con tu HTML para darle color y estilo a tu página "Mis cosas favoritas": colores de texto y de fondo, tipo y tamaño de letra, y texto centrado. Se usa la analogía de la ropa: si HTML es el esqueleto, CSS es la ropa.
- **Enlace**: [▶️ Ver la lección](https://youtu.be/XWjB9rQ_3_o)
- **Conceptos clave**:
  - Conectar CSS con HTML: `<link rel="stylesheet" href="style.css">` dentro de `<head>`
  - Forma de una regla: `selector { propiedad: valor; }`
  - Colores: `color` (texto) y `background-color` (fondo), por nombre o por código como `#dc143c`, eligiendo colores que se lean bien sobre el fondo
  - Texto: `font-family`, `font-size` y `text-align`
  - Clases: `class="destacado"` en HTML y `.destacado` en CSS para darle estilo a un solo elemento
  - Comentarios: `/* ... */` en CSS y `<!-- ... -->` en HTML son notas que el navegador ignora
- **Práctica**: [¡Vamos a practicar!](https://jsfiddle.net/jaeby6k2/1/) 👈 **¡Ponle color a tu página!**
  - ¿Prefieres otro editor? Copia el código de [`starter-files/leccion-04`](https://github.com/1ASI0730-2620-16129-G2-DevTech/upc-pre-202620--1asi0730-16129-DevTech-course-plan/tree/main/starter-files/leccion-04) en [JSFiddle](https://jsfiddle.net/), [CodePen](https://codepen.io/pen/) o [Replit](https://replit.com/).

### Lección 5: Cajas, bordes y centrado (10 minutos)

- **Descripción**: Descubre que cada elemento de tu página es una caja y aprende a darle espacio, bordes y esquinas redondeadas, y a centrar tu página "Mis cosas favoritas" en una columna ordenada que se vea bien también en el celular. Se usa la analogía de un cuadro en la pared: la foto es el contenido, el cartón es el relleno, el marco es el borde y el espacio en la pared es el margen.
- **Enlace**: [▶️ Ver la lección](https://youtu.be/AgF1RJGDLEE)
- **Conceptos clave**:
  - Modelo de caja: contenido, `padding`, `border` y `margin`, de adentro hacia afuera
  - Bordes: `border: 2px solid purple;` (grosor, estilo y color)
  - Espacios: `padding` (adentro del borde) y `margin` (afuera del borde), como `margin-top`
  - Esquinas redondeadas: `border-radius`
  - Centrar la página: `max-width: 600px;` y `margin: 0 auto;`
  - Imágenes que se adaptan al celular: `max-width: 100%;` en `img`
- **Práctica**: [¡Vamos a practicar!](https://jsfiddle.net/1oa6ybwg/) 👈 **¡Ordena tu página!**
  - ¿Prefieres otro editor? Copia el código de [`starter-files/leccion-05`](https://github.com/1ASI0730-2620-16129-G2-DevTech/upc-pre-202620--1asi0730-16129-DevTech-course-plan/tree/main/starter-files/leccion-05) en [JSFiddle](https://jsfiddle.net/), [CodePen](https://codepen.io/pen/) o [Replit](https://replit.com/).


### Lección 6: Proyecto final: tu página de perfil (12 minutos)


- **Descripción**: Integra todo lo aprendido sobre HTML y CSS para crear tu propia página de perfil personal. Agrega tu fotografía, nombre, una descripción sobre ti, tus gustos, enlaces favoritos y una frase que te represente. Organiza el contenido en secciones y tarjetas, utilizando etiquetas semánticas y aplicando estilos para personalizar el diseño de tu página.
- **Enlace**: [YouTube](https://youtu.be/ToHAiKemYY8?si=R5leE1fSAU0YHI4h)
- **Conceptos clave**:
  - Etiquetas semánticas: `<header>`, `<main>`, `<section>`, `<footer>`
  - Títulos y párrafos: `<h1>` a `<h6>`, `<p>`
  - Listas: `<ul>`, `<ol>`, `<li>`
  - Imágenes: `<img src="..." alt="...">`
  - Enlaces: `<a href="...">texto</a>`
  - Organización del contenido mediante secciones y tarjetas
  - Personalización con CSS: colores, fuentes, bordes, márgenes y espacios
- **Práctica**: [¡Vamos a practicar!](https://jsfiddle.net/arianaperez08/vh12jr5d/1/) 👈 **¡No necesitas instalar nada!**
- ¿Prefieres otro editor? Copia el código de `starter-files/leccion-06` en [JSFiddle](https://jsfiddle.net/), [CodePen](https://codepen.io/pen/) o [Replit](https://replit.com/).


### Lección 7: Errores comunes y próximos pasos (6 minutos)

- **Descripción**: Revisa los errores más comunes de HTML y CSS aplicados a la página de perfil que construiste en la Lección 6. Aprende a encontrar y corregir problemas paso a paso, comprueba tu proyecto final y descubre cómo seguir aprendiendo después del curso.
- **Enlace**: [YouTube](https://youtu.be/EJeZEE86Zss)
- **Conceptos clave**:
  - Etiquetas de apertura y cierre, anidación y organización de secciones.
  - Imágenes y enlaces: revisar `src`, `alt` y `href`.
  - Conexión de CSS y coincidencia entre `class="tarjeta"` y `.tarjeta`.
  - Sintaxis CSS: dos puntos `:`, punto y coma `;`, llaves `{ }` y comentarios `/* ... */`.
  - Unidades y espacios: `padding: 16px;`, diferencias entre `padding` y `margin`, y centrado de la página.
  - Revisión paso a paso: identificar el problema, hacer un cambio y comprobar el resultado.
  - Próximos pasos: mejorar el perfil, practicar diseños adaptables y continuar con Flexbox, Grid y JavaScript.
- **Práctica**: [¡Vamos a practicar!](https://jsfiddle.net/GabrielRamirez/v53gax0r/) 👈 **¡No necesitas instalar nada!**
  - Corrige los tres errores de la regla CSS: el selector de clase, los dos puntos de `color` y la unidad de `padding`.
  - Comprueba que las tarjetas tengan texto morado y 16 píxeles de espacio interior.
  - ¿Prefieres otro editor? Copia el código de `starter-files/leccion-07` en [JSFiddle](https://jsfiddle.net/), [CodePen](https://codepen.io/pen/) o [Replit](https://replit.com/).
  - Si tu editor tiene paneles separados, copia el contenido de `<body>` en HTML y el archivo `style.css` en CSS.
  - Al terminar, compara con `completed-examples/leccion-07` y aplica la revisión a tu perfil personal.


## Recursos Adicionales

- **Código Fuente Completo**: [https://github.com/1ASI0730-2620-16129-G2-DevTech/upc-pre-202620--1asi0730-16129-DevTech-course-plan/tree/main](https://github.com/1ASI0730-2620-16129-G2-DevTech/upc-pre-202620--1asi0730-16129-DevTech-course-plan/tree/main)
- **Archivos de práctica**: el código de inicio de cada lección está en la carpeta `starter-files` del repositorio y la solución en `completed-examples`. Úsalos si prefieres trabajar en CodePen o Replit.
- **Todas las actividades prácticas**:

| Lección | Actividad | Empezar a programar |
|---------|-----------|---------------------|
| 4 | Ponle color a tu página | [JSFiddle](https://jsfiddle.net/jaeby6k2/1/) |
| 5 | Ordena tu página | [JSFiddle](https://jsfiddle.net/1oa6ybwg/) |

- **Para seguir aprendiendo**: [MDN Web Docs en español](https://developer.mozilla.org/es/)

**¡Gracias por completar el curso!**

## 👥 Elaboración

Universidad Peruana de Ciencias Aplicadas
Carrera de Ingeniería de Software
Período 202620
1ASI0730 Aplicaciones Web
NRC 16129

**Nombre del equipo**: DevTech
**Líder del equipo**: Pérez Vásquez, Ariana Valeria
**Integrantes del equipo**:
- Pérez Vásquez, Ariana Valeria (u20241D338)
- Ramirez Gutierrez, Gabriel (u202416053)
- Ramos Fuentes Rivera, Adriana Nicole (u202018427)
- Tufiño Argüelles, Luis Angel (u202216240)