# Guión — Lección 4: Dale estilo con CSS

**Duración estimada**: 9 minutos

---

## Introducción (0:00 – 0:30)

Tu página "Mis cosas favoritas" ya tiene títulos, listas, una imagen y un enlace. Pero todo se ve en blanco y negro, con la misma letra. Hoy vas a aprender **CSS** para darle color y personalidad.

---

## ¿Qué es CSS? (0:30 – 1:30)

CSS significa "hojas de estilo en cascada", pero lo importante es qué hace: **decide cómo se ve** cada parte de tu página.

Piénsalo así: si HTML es el **esqueleto** de tu página, CSS es la **ropa**. El esqueleto dice dónde va cada cosa; la ropa decide los colores, el tipo de letra y el estilo.

- HTML → **qué** hay en la página (un título, una lista, una imagen).
- CSS → **cómo se ve** (de qué color, de qué tamaño, con qué letra).

---

## Conectar CSS con tu HTML (1:30 – 3:00)

El CSS se escribe en un archivo aparte llamado `style.css`. Para que tu página lo use, agregamos esta línea dentro del `<head>`:

```html
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Mis cosas favoritas</title>
  <link rel="stylesheet" href="style.css">
</head>
```

- `<link>` conecta tu página con otro archivo. Es una etiqueta vacía, así que no lleva cierre.
- `rel="stylesheet"` le dice al navegador que ese archivo es de estilos.
- `href="style.css"` es el nombre del archivo, igual que en los enlaces.

Un detalle: si tu editor en línea tiene un **panel CSS** separado (como JSFiddle o CodePen), no necesitas el `<link>`. Lo que escribas en ese panel se conecta solo.

---

## ¿Cómo se escribe una regla CSS? (3:00 – 4:30)

Cada instrucción de CSS se llama **regla** y siempre tiene la misma forma:

```css
h1 {
  color: blue;
}
```

- `h1` es el **selector**: a quién le hablamos. Aquí, a todos los `<h1>` de la página.
- `color` es la **propiedad**: qué queremos cambiar.
- `blue` es el **valor**: cómo lo queremos.

Es como dar una orden: "A todos los `h1`: pónganse de color azul".

Fíjate en tres detalles:

1. Las llaves `{ }` abren y cierran la regla.
2. Entre la propiedad y el valor van **dos puntos** `:`.
3. Cada línea termina con **punto y coma** `;`.

---

## Colores (4:30 – 5:30)

Hay dos propiedades de color que usarás todo el tiempo:

```css
body {
  background-color: lightyellow;
}

h2 {
  color: tomato;
}
```

- `color` cambia el color del **texto**.
- `background-color` cambia el color del **fondo**.

Puedes escribir los colores por su nombre en inglés: `red`, `blue`, `tomato`, `purple`, `lightyellow`… También existen códigos como `#ff6347`, que es otra forma de escribir `tomato`. Con los códigos tienes millones de colores, pero para empezar los nombres son suficientes.

Como pusimos el fondo en `body`, se pinta **toda** la página.

---

## Letras y texto (5:30 – 6:45)

Ahora cambiemos cómo se ve la letra:

```css
body {
  background-color: lightyellow;
  font-family: Arial, sans-serif;
}

h1 {
  color: darkblue;
  text-align: center;
}
```

- `font-family` elige el **tipo de letra**. Ponemos dos opciones: si la computadora no tiene Arial, usa cualquier letra parecida (`sans-serif`).
- `font-size` cambia el **tamaño** de la letra, por ejemplo `font-size: 20px;`. `px` significa píxeles, los puntitos de tu pantalla.
- `text-align: center;` **centra el texto**.

Una regla puede tener varias propiedades: solo escribe una debajo de otra, cada una con su `;`.

---

## Clases: darle estilo a un solo elemento (6:45 – 7:30)

¿Y si quieres que **solo un** párrafo se vea distinto? Para eso usamos una **clase**. Primero le pones un nombre en el HTML:

```html
<p class="destacado">Hola, aquí te cuento lo que más me gusta.</p>
```

Y en el CSS lo llamas con un **punto** delante:

```css
.destacado {
  font-size: 20px;
  color: purple;
}
```

El punto le dice al CSS: "esto no es una etiqueta, es una clase". Así solo cambia el párrafo que tiene `class="destacado"` y los demás se quedan igual.

---

## Práctica guiada (7:30 – 8:30)

Abre el enlace de práctica que está en la descripción del video, en el editor en línea que prefieras. Los archivos de inicio (`starter-files/leccion-04/`) son dos: `index.html`, con tu página de la lección anterior y el `<link>` ya puesto, y `style.css`, que trae la regla de `body` hecha como ejemplo y 3 pasos marcados en comentarios:

1. Escribe una regla para `h1` que cambie su color y lo centre.
2. Escribe una regla para que los `h2` tengan otro color.
3. Escribe una regla `.destacado` para que el primer párrafo se vea más grande.

Antes de empezar, prueba a cambiar el color de fondo de `body` para ver cómo funciona.

¡Elige los colores que más te gusten!

Ojo con el error más común: olvidar el `;` o la llave de cierre `}`. Si una regla no funciona, revisa primero esos signos. Y recuerda que las propiedades se escriben en inglés: es `color`, no `colour` ni `colores`.

---

## Cierre (8:30 – 9:00)

¡Tu página ya tiene color y estilo propio! En la siguiente lección aprenderás a usar cajas, bordes y a centrar elementos para que todo se vea ordenado.

¡Hasta la lección 5!
