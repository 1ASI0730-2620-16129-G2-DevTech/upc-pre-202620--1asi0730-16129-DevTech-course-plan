# Guión — Lección 3: Elementos HTML comunes

**Duración estimada**: 10 minutos

---

## Introducción (0:00 – 0:30)

Ya conoces el esqueleto de una página. Ahora vamos a llenarla de contenido. En esta lección crearemos juntos una página llamada **"Mis cosas favoritas"** con títulos, párrafos, listas, una imagen y un enlace.

---

## Títulos (0:30 – 2:00)

HTML tiene seis tamaños de título, desde `<h1>` (el más grande) hasta `<h6>` (el más pequeño):

```html
<h1>Título principal</h1>
<h2>Subtítulo</h2>
<h3>Título más pequeño</h3>
<h4>Más pequeño aún</h4>
<h5>Casi chiquito</h5>
<h6>El más pequeño</h6>
```

Funcionan como en un periódico: el `<h1>` es el gran titular de portada y los demás son los títulos de cada sección.

Un consejo: usa **un solo `<h1>` por página**, igual que un libro tiene un solo título.

---

## Párrafos (2:00 – 3:00)

Para escribir texto normal usamos la etiqueta `<p>`:

```html
<p>Hola, aquí te cuento lo que más me gusta.</p>
<p>Cada párrafo aparece separado del anterior.</p>
```

---

## Listas (3:00 – 4:30)

Hay dos tipos de listas:

```html
<!-- Lista con puntos: el orden no importa -->
<ul>
  <li>Dibujar</li>
  <li>Jugar fútbol</li>
  <li>Escuchar música</li>
</ul>

<!-- Lista numerada: el orden sí importa -->
<ol>
  <li>Calienta la leche</li>
  <li>Agrega el chocolate</li>
  <li>Mueve y sirve</li>
</ol>
```

- `<ul>` crea una lista con puntos, como tu lista de compras.
- `<ol>` crea una lista con números, como los pasos de una receta.
- `<li>` es cada elemento de la lista. Siempre va dentro de un `<ul>` o un `<ol>`.

---

## Imágenes (4:30 – 6:30)

Para mostrar una imagen usamos `<img>`, que necesita dos atributos:

```html
<img src="https://picsum.photos/id/1018/400/250" alt="Montañas con un río y árboles verdes">
```

- `src` dice **dónde** está la imagen (su dirección).
- `alt` **describe** la imagen con palabras.

El `alt` es muy importante: ayuda a las personas que no pueden ver la pantalla (sus programas les leen la descripción) y además aparece si la imagen no carga.

Recuerda que `<img>` es una etiqueta vacía, así que no lleva cierre.

---

## Enlaces (6:30 – 8:00)

Para crear un enlace usamos `<a>` con el atributo `href`, que es la dirección a la que te lleva:

```html
<p>Aprende más en <a href="https://developer.mozilla.org/es/">MDN Web Docs</a>.</p>
```

El texto entre `<a>` y `</a>` es lo que se puede hacer clic.

Fíjate que la dirección empieza con `https://`. Si no lo pones, el navegador buscará esa página dentro de tu propio sitio y no la encontrará.

---

## Práctica guiada (8:00 – 9:30)

Abre el enlace de práctica que está en la descripción del video, en el editor en línea que prefieras. El archivo de inicio (`starter-files/leccion-03/index.html`) ya tiene los títulos y 4 pasos marcados en comentarios:

1. Crea una lista `<ul>` con 3 de tus pasatiempos.
2. Crea una lista `<ol>` con los pasos de una receta sencilla.
3. Agrega una imagen con su `alt`. Puedes cambiar el número `1018` por otro, por ejemplo `237`, para ver otra foto.
4. Agrega un enlace a tu página educativa favorita.

Cuidado con olvidar las comillas: se escribe `src="https://..."` y no `src=https://...`.

---

## Cierre (9:30 – 10:00)

Tu página ya tiene mucho contenido, pero todavía se ve muy simple: todo en blanco y negro. En la siguiente lección aprenderás CSS para darle color y estilo.

¡Hasta la lección 4!
