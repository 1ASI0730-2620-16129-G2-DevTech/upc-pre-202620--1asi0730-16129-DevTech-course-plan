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

