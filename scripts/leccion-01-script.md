# Guión — Lección 1: ¿Qué es un sitio web? + Errores comunes y próximos pasos

**Duración estimada**: 9 minutos

---

## Introducción (0:00 – 0:40)

¡Bienvenido a tu primera lección de desarrollo web!

Seguramente todos los días visitas páginas web. Puede ser para ver videos, buscar información, escuchar música o incluso hacer tus tareas.

Pero ¿alguna vez te has preguntado cómo funcionan esas páginas? ¿Cómo se construyen? ¿Y qué necesitas aprender para crear una tú mismo?

Hoy vamos a responder esas preguntas. Además, conocerás las herramientas básicas del desarrollo web, escribirás tu primer código y descubrirás algunos errores comunes que debes evitar.

¡Vamos a empezar!

---

## ¿Qué es un sitio web? (0:40 – 2:00)

Un **sitio web** es un conjunto de páginas que puedes visitar a través de Internet usando un navegador, como Google Chrome, Firefox o Safari.

Piensa en un sitio web como si fuera un libro.

- El **sitio web** es el libro completo.
- Las **páginas web** son las páginas individuales del libro.
- Los **enlaces** son como indicaciones que te permiten saltar de una página a otra.

Por ejemplo, cuando visitas YouTube, estás entrando a un sitio web. Dentro de él puedes encontrar diferentes páginas: la página principal, la de un video, la de un canal y muchas más.

Y aquí viene algo importante: **un sitio web y una página web no son exactamente lo mismo**.

Una página web es un documento individual que se muestra en tu navegador, mientras que un sitio web puede contener muchas páginas relacionadas.

---

## ¿Cómo funciona una página web? (2:00 – 3:15)

Cuando escribes una dirección en tu navegador y presionas Enter, ocurre algo parecido a pedir comida en un restaurante.

Tú haces el pedido, alguien lo prepara y finalmente recibes lo que solicitaste.

En Internet pasa algo similar:

1. Escribes la dirección de una página web.
2. Tu navegador solicita la información a un servidor.
3. El servidor responde enviando los archivos necesarios.
4. El navegador interpreta esos archivos y muestra la página en tu pantalla.

Un **servidor** es una computadora o sistema que almacena y entrega información a otros dispositivos.

Y el **navegador** es el programa que interpreta esa información para que puedas ver e interactuar con una página.

Lo interesante es que no necesitas tener un servidor para empezar a aprender. Puedes crear tus primeras páginas directamente en tu computadora o utilizando un editor en línea.

---

## Los tres pilares del desarrollo web (3:15 – 4:45)

La mayoría de las páginas web utilizan tres tecnologías fundamentales: **HTML, CSS y JavaScript**.

Imagina que estás construyendo una casa.

### HTML — La estructura

HTML es como los cimientos, las paredes y las habitaciones.

Define qué elementos existen dentro de la página: títulos, párrafos, imágenes, botones y enlaces.

Por ejemplo:

```html
<h1>Mi primera página</h1>
<p>Estoy aprendiendo desarrollo web.</p>
```

Este código crea un título y un párrafo.

### CSS — La apariencia

CSS es como la pintura, los muebles y la decoración de la casa.

Permite cambiar colores, tamaños, fuentes y posiciones.

Por ejemplo:

```css
h1 {
  color: blue;
}
```

Con este código, el título se mostrará de color azul.

### JavaScript — La interacción

JavaScript es como la electricidad y los mecanismos de la casa.

Permite que las páginas reaccionen a las acciones del usuario.

Por ejemplo, mostrar un mensaje cuando alguien presiona un botón.

```javascript
alert("¡Hola, mundo!");
```

No te preocupes si todavía no entiendes todo este código.

Por ahora, recuerda lo siguiente:

- **HTML** construye la estructura.
- **CSS** define la apariencia.
- **JavaScript** agrega interactividad.

En este curso empezaremos por HTML, porque antes de decorar una casa, primero necesitamos construirla.

---

## Tu primer contacto con HTML (4:45 – 6:00)

Ahora vamos a escribir nuestro primer código.

Para hacerlo, puedes utilizar un editor en línea que permita trabajar con HTML, como CodePen, o un editor de código en tu computadora.

Si estás utilizando un editor en línea con un panel llamado HTML, escribe lo siguiente:

```html
<h1>¡Hola, mundo!</h1>
<p>Esta es mi primera página web.</p>
```

Observa lo que aparece en la vista previa.

¡Acabas de crear el contenido de tu primera página web!

El texto más grande es un título y el texto pequeño es un párrafo.

Pero ¿por qué el navegador sabe que uno debe ser grande y el otro pequeño?

La respuesta está en las **etiquetas HTML**.

Las etiquetas le indican al navegador qué representa cada contenido.

Por ejemplo:

- `<h1>` representa un título principal.
- `<p>` representa un párrafo.

Y aunque ahora parezcan símbolos extraños, pronto te resultarán tan familiares como escribir un mensaje.

En la siguiente lección aprenderemos exactamente cómo funcionan estas etiquetas.

---

## Errores comunes al comenzar (6:00 – 7:15)

Antes de continuar, quiero mostrarte algunos errores muy comunes cuando empiezas a crear páginas web.

### Error 1: Confundir HTML con un lenguaje de programación

HTML no es un lenguaje de programación. Es un **lenguaje de marcado**, porque utiliza etiquetas para organizar y describir el contenido.

JavaScript, en cambio, sí es un lenguaje de programación.

### Error 2: Pensar que necesitas memorizar todo

No necesitas aprenderte todas las etiquetas desde el primer día.

Incluso los desarrolladores con experiencia consultan documentación cuando olvidan algo.

Lo importante es entender para qué sirve cada elemento y practicar.

### Error 3: Escribir código sin revisar los detalles

En desarrollo web, un pequeño error puede provocar que algo no aparezca como esperabas.

Por ejemplo:

```html
<h1>Mi página</h1>
```

Si olvidas escribir correctamente una etiqueta, el navegador podría interpretar el contenido de manera diferente.

Por eso es importante revisar lo que escribes.

### Error 4: Querer aprender todo al mismo tiempo

No necesitas dominar HTML, CSS y JavaScript en una sola tarde.

Aprender desarrollo web es como aprender a tocar un instrumento: primero entiendes lo básico, después practicas y finalmente puedes crear cosas más complejas.

---

## Práctica guiada (7:15 – 8:15)

Ahora te toca a ti.

Abre el enlace de práctica que encontrarás en la descripción del video y utiliza el editor en línea que prefieras.

Si estás trabajando en un panel HTML que ya prepara la estructura por ti, escribe lo siguiente:

```html
<h1>Mi primera página web</h1>
<p>Hola, estoy aprendiendo HTML.</p>
```

Ahora realiza estos tres cambios:

1. Cambia el título por tu nombre o por el nombre que quieras darle a tu página.
2. Modifica el párrafo para contar algo sobre ti o sobre un tema que te guste.
3. Agrega un segundo párrafo utilizando otra etiqueta `<p>`.

Por ejemplo:

```html
<h1>Bienvenido a mi página</h1>
<p>Me gusta la tecnología.</p>
<p>Quiero aprender a crear sitios web.</p>
```

Si utilizas un editor que trabaja con archivos completos, puedes usar su plantilla inicial de `index.html` y colocar estas líneas dentro del `<body>`.

No te preocupes si todavía no sabes qué significa esa parte. La explicaremos en la próxima lección.

Lo importante es que experimentes, cambies el texto y observes cómo se actualiza tu página.

---

## Próximos pasos (8:15 – 8:40)

¡Ya diste tu primer paso en el desarrollo web!

Ahora sabes qué es un sitio web, cómo funciona un navegador y cuáles son las tres tecnologías principales que utilizaremos.

A partir de aquí, nuestro siguiente objetivo será comprender HTML con más profundidad.

En la próxima lección aprenderás qué son las etiquetas, cómo se abren y se cierran, qué son los atributos y cómo se organiza la estructura completa de una página web.

---

## Cierre (8:40 – 9:00)

Hoy descubriste que las páginas web no aparecen por arte de magia: detrás de ellas hay archivos, etiquetas y tecnologías que trabajan juntas.

Y lo mejor es que ya comenzaste a utilizar una de ellas.

Recuerda: no necesitas saberlo todo para empezar. Solo necesitas practicar y avanzar paso a paso.

En la siguiente lección construiremos el esqueleto de nuestra primera página HTML.

¡Hasta la lección 2!
