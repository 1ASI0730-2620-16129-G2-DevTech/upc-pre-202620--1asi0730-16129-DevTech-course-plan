# Guión — Lección 2: El esqueleto de una página HTML

**Duración estimada**: 9 minutos

---

## Introducción (0:00 – 0:30)

En la lección pasada escribiste tu primer código. Hoy vas a entender qué significa cada parte y cómo se arma el esqueleto que tienen todas las páginas web.

---

## Etiquetas y elementos (0:30 – 2:30)

HTML funciona con **etiquetas**. Una etiqueta es una palabra entre los símbolos `< >` que le dice al navegador qué tipo de contenido viene.

Piensa en un sándwich: hay un pan de arriba, un relleno y un pan de abajo.

```html
<p>Hola, este es mi párrafo.</p>
```

- `<p>` es la **etiqueta de apertura** (el pan de arriba).
- `Hola, este es mi párrafo.` es el **contenido** (el relleno).
- `</p>` es la **etiqueta de cierre** (el pan de abajo). Fíjate que lleva una barra `/`.

Todo junto, desde `<p>` hasta `</p>`, se llama **elemento**.

---

## Etiquetas vacías (2:30 – 3:30)

Algunas etiquetas no tienen contenido en medio, así que no necesitan cierre. Se llaman **etiquetas vacías**:

```html
<img src="foto.jpg" alt="Mi foto">
<br>
```

- `<img>` muestra una imagen.
- `<br>` hace un salto de línea.

---

## Atributos (3:30 – 4:30)

Un **atributo** es información extra que se agrega dentro de la etiqueta de apertura. Es como pedir un sándwich "sin cebolla": no cambia qué es, pero le da un detalle.

Siempre se escribe así: nombre, signo igual y valor entre comillas.

```html
<html lang="es">
```

Aquí el atributo `lang` le dice al navegador que la página está en español.

---

## El esqueleto completo (4:30 – 7:00)

Toda página web tiene esta misma estructura:

```html
<!DOCTYPE html>
<html lang="es">
  <head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Mi primera página</title>
  </head>
  <body>
    <h1>Bienvenidos a mi página</h1>
    <p>Aquí va todo lo que se ve.</p>
  </body>
</html>
```

Veamos qué hace cada parte:

- `<!DOCTYPE html>` le avisa al navegador que es una página HTML moderna.
- `<html>` envuelve toda la página.
- `<head>` es la parte "invisible": información para el navegador. Piensa en ella como el cerebro 🧠.
- `<meta charset="UTF-8">` permite que se vean bien las tildes y la ñ.
- `<meta name="viewport" ...>` hace que la página se vea bien en celulares.
- `<title>` es el texto que aparece en la pestaña del navegador.
- `<body>` es el cuerpo: todo lo que sí ves en la pantalla.

Fíjate que las etiquetas van unas dentro de otras, como cajas dentro de cajas. Por eso usamos espacios al inicio de cada línea (la **sangría**): así se ve claramente qué está dentro de qué.

---

## Un detalle sobre los editores en línea (7:00 – 7:45)

Algunos editores en línea tienen un panel HTML separado y ya agregan el `<head>` y el `<body>` por ti. Si tu editor es así, en ese panel solo escribes lo que va **dentro** del `<body>`:

```html
<h1>Bienvenidos a mi página</h1>
<p>Aquí va todo lo que se ve.</p>
```

Otros editores trabajan con un archivo `index.html` completo. En ese caso, escribe el esqueleto entero. Y recuerda: en un archivo `.html` real siempre necesitas el esqueleto completo.

---

## Práctica guiada (7:45 – 8:30)

Abre el enlace de práctica que está en la descripción del video, en el editor en línea que prefieras. El archivo de inicio (`starter-files/leccion-02/index.html`) tiene 3 pasos marcados en comentarios:

1. Escribe un `<title>` con el texto "Mi primera página".
2. Escribe un `<h1>` con el nombre de tu canción favorita.
3. Escribe un `<p>` explicando por qué te gusta.

Ojo con el error más común: olvidar la etiqueta de cierre. Si escribes `<h1>Hola` sin `</h1>`, ¡todo lo que venga después se volverá un título gigante!

---

## Cierre (8:30 – 9:00)

Ya tienes el esqueleto de tu página. En la siguiente lección le pondremos "músculos": títulos, listas, imágenes y enlaces.

¡Hasta la lección 3!
