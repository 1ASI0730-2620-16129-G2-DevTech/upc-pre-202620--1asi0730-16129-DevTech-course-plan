# Guión — Lección 6: Proyecto final: tu página de perfil

**Duración estimada:** 12 minutos

---

## Introducción (0:00 – 0:45)

¡Llegó el momento de juntar todo lo que aprendiste! Hoy vas a construir tu propia **página de perfil personal**, donde podrás presentar quién eres, tus intereses, tus pasatiempos y algunos de tus enlaces favoritos. Al final tendrás una página que refleje tu personalidad.

Crear una página es como cocinar: primero eliges la receta (planificar), luego juntas los ingredientes (HTML) y al final sirves el plato bonito (CSS).

---

## Paso 1: Planifica tu página (0:45 – 2:00)

Antes de escribir código, haz un boceto rápido en una hoja. Nuestra página tendrá tres zonas:

- **Arriba (cabecera):** tu foto, tu nombre y una breve descripción sobre ti.
- **En el medio (contenido):** tres tarjetas: "Sobre mí", "Cosas que me gustan" y "Mis enlaces favoritos".
- **Abajo (pie de página):** una frase que te inspire o represente.

---

## Etiquetas con nombre propio (2:00 – 3:00)

Para organizar estas zonas usaremos cuatro etiquetas nuevas. Funcionan de manera similar a un `<div>`, pero sus nombres indican qué contenido contienen:

- `<header>`: representa la cabecera de la página.
- `<main>`: contiene el contenido principal.
- `<section>`: organiza cada sección o bloque del contenido.
- `<footer>`: representa el pie de página.

Estas etiquetas se conocen como etiquetas semánticas y ayudan a los buscadores y a los lectores de pantalla a comprender mejor cómo está organizada tu página.

---

## Paso 2: Escribe el HTML (3:00 – 6:00)

Empecemos por la cabecera. Aquí colocaremos una imagen de perfil, nuestro nombre y una pequeña descripción.

```html
<header>
    <img src="https://picsum.photos/id/64/150/150"
         alt="Foto de perfil">

    <h1>Hola, soy Ariana</h1>

    <p class="subtitulo">
        Estudiante de Ingeniería de Software | Me gusta la tecnología y aprender cosas nuevas
    </p>
</header>
```

Ahora agregaremos el contenido principal con sus tres tarjetas.

Primero, la sección "Sobre mí", donde presentamos quiénes somos y nuestros intereses.

```html
<main>

    <section class="tarjeta">
        <h2>Sobre mí</h2>

        <p>
            Soy estudiante de Ingeniería de Software.
            Me interesa el desarrollo web, la programación
            y la tecnología. Me gusta aprender nuevas
            herramientas y desarrollar proyectos que
            permitan resolver problemas.
        </p>
    </section>
```

Después, crearemos la sección "Cosas que me gustan". Para mostrar nuestros intereses utilizaremos una lista con la etiqueta `<ul>` y sus elementos `<li>`.

```html
    <section class="tarjeta">
        <h2>Cosas que me gustan</h2>

        <ul>
            <li>Aprender sobre tecnología y programación.</li>
            <li>Escuchar música.</li>
            <li>Compartir tiempo con mis mascotas.</li>
            <li>Conocer cosas nuevas.</li>
        </ul>
    </section>
```

Por último, agregaremos nuestros enlaces favoritos. Utilizaremos la etiqueta `<a>` para crear enlaces a páginas web como YouTube, GitHub y W3Schools.

```html
    <section class="tarjeta">
        <h2>Mis enlaces favoritos</h2>

        <ul>
            <li>
                <a href="https://www.youtube.com/" target="_blank">
                    YouTube
                </a>
            </li>

            <li>
                <a href="https://github.com/" target="_blank">
                    GitHub
                </a>
            </li>

            <li>
                <a href="https://www.w3schools.com/" target="_blank">
                    W3Schools
                </a>
            </li>
        </ul>
    </section>

</main>
```

Y para terminar la estructura HTML, agregaremos el pie de página con una frase que nos inspire.

```html
<footer>
    <p>
        "Nunca dejes de aprender, porque la vida nunca deja de enseñar."
    </p>
</footer>
```

**¡Pausa!** Detén el video y cambia el contenido por el tuyo: tu nombre, tu descripción, tus gustos, tus enlaces favoritos y una frase que te represente.

---

## Paso 3: Dale estilo con CSS (6:00 – 10:00)

Ahora vamos a la zona CSS de nuestro editor. Primero personalizaremos toda la página y después le daremos estilo a la cabecera.

```css
body {
    background-color: #f3e8ff;
    font-family: Verdana, sans-serif;
    color: #333333;
    margin: 0;
}

header {
    background-color: #7c3aed;
    color: white;
    text-align: center;
    padding: 30px 20px;
}

header img {
    border-radius: 50%;
    border: 4px solid white;
}

.subtitulo {
    font-style: italic;
}
```

Usamos `margin: 0` en el `body` para quitar el pequeño espacio que el navegador deja en los bordes de la página.

También utilizamos `border-radius: 50%` para que nuestra imagen tenga forma circular y `text-align: center` para centrar el contenido de la cabecera.

Ahora centraremos el contenido principal y le daremos forma a nuestras tres tarjetas.

```css
main {
    max-width: 600px;
    margin: 0 auto;
    padding: 20px;
}

.tarjeta {
    background-color: white;
    border: 2px solid #c4b5fd;
    border-radius: 12px;
    padding: 15px 20px;
    margin-bottom: 20px;
}
```

Con `max-width` limitamos el ancho del contenido, mientras que `margin: 0 auto` permite centrarlo horizontalmente.

Por otro lado, utilizamos `background-color`, `border` y `border-radius` para darle a las tarjetas un fondo blanco, un borde de color y esquinas redondeadas.

Por último, personalizaremos los títulos, los enlaces y el pie de página.

```css
h2 {
    color: #7c3aed;
}

a {
    color: #db2777;
    font-weight: bold;
}

footer {
    text-align: center;
    padding: 20px;
    font-size: 14px;
}
```

De esta manera, los títulos tendrán un color morado, los enlaces destacarán en rosado y nuestra frase final aparecerá centrada en la parte inferior.

**¡Pausa!** Detén el video y cambia los colores, la fuente y los estilos por los que más te gusten. ¡Haz que tu página tenga tu propio estilo!

---

## Guarda tu trabajo (10:00 – 11:30)

Para guardar tu página tienes dos opciones:

- Crear una cuenta gratuita en tu editor en línea y utilizar su botón de guardar (normalmente dice **Save**). Así podrás conservar tu proyecto y obtener un enlace para compartirlo.
- Si no quieres crear una cuenta, copia tu código HTML y CSS en documentos para no perder tu trabajo.

El archivo de inicio está en `starter-files/leccion-06/` y la versión terminada en `completed-examples/leccion-06/`.

---

## Cierre (11:30 – 12:00)

¡Felicidades, ya eres creador web! Has construido una página de perfil personal utilizando HTML para organizar el contenido y CSS para darle estilo.

Aprendiste a utilizar etiquetas semánticas, organizar información en tarjetas, crear listas y agregar enlaces a otras páginas.

En la última lección conocerás los errores más comunes al trabajar con HTML y CSS y aprenderás cómo solucionarlos.

¡Hasta la lección 7!