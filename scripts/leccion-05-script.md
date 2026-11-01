# Guión — Lección 5: Cajas, bordes y centrado

**Duración estimada**: 9 minutos

---

## Introducción (0:00 – 0:30)

Tu página "Mis cosas favoritas" ya tiene colores y su propio tipo de letra. Pero todo está pegado al borde izquierdo de la pantalla y apretado. Hoy vas a aprender a darle **espacio**, **bordes** y a **centrar** tu página para que se vea ordenada.

---

## Todo es una caja (0:30 – 1:30)

Este es el secreto más importante de CSS: **cada elemento de tu página es una caja**. Un título es una caja, un párrafo es una caja, una imagen es una caja.

Piensa en un **cuadro colgado en la pared**:

- La **foto** es el contenido.
- El cartón blanco alrededor de la foto es el **padding** (relleno).
- El **marco** es el **border** (borde).
- El espacio en la pared hasta el siguiente cuadro es el **margin** (margen).

Así funcionan todas las cajas de tu página: contenido, padding, border y margin, de adentro hacia afuera.

---

## Bordes (1:30 – 3:00)

Empecemos por el marco. Para ponerle borde a un elemento usamos `border`:

```css
.destacado {
  border: 2px solid purple;
}
```

El valor tiene tres partes:

- `2px` es el **grosor** del borde.
- `solid` es el **estilo**: una línea continua. También puedes probar `dashed` (rayitas) o `dotted` (puntitos).
- `purple` es el **color**.

Ahora sí puedes ver la caja del párrafo. Fíjate que el texto queda pegado al borde… eso lo arreglamos con el padding.

---

## Padding: el espacio de adentro (3:00 – 4:15)

El `padding` es el espacio **entre el contenido y el borde**, como el cartón blanco del cuadro:

```css
.destacado {
  border: 2px solid purple;
  padding: 15px;
  background-color: white;
}
```

Con `padding: 15px;` el texto se separa 15 píxeles del borde por todos los lados. Le pusimos fondo blanco para que veas mejor que el padding forma parte de la caja: el fondo también pinta el relleno.

---

## Margin: el espacio de afuera (4:15 – 5:15)

El `margin` es el espacio **fuera del borde**, que separa una caja de las demás:

```css
h2 {
  color: tomato;
  margin-top: 30px;
}
```

Con `margin-top` agregamos espacio solo **arriba** de cada `h2`, así cada sección queda más separada de la anterior. También existen `margin-bottom` (abajo), `margin-left` (izquierda) y `margin-right` (derecha). Si escribes solo `margin`, cambia los cuatro lados a la vez.

Un truco para no confundirte: **padding es adentro, margin es afuera**.

---

## Esquinas redondeadas (5:15 – 6:00)

Las cajas tienen esquinas en punta, pero puedes redondearlas con `border-radius`:

```css
img {
  border: 4px solid tomato;
  border-radius: 15px;
}
```

Mientras más grande el número, más redondas las esquinas. ¡Tu foto ahora parece una tarjeta!

---

## Centrar la página (6:00 – 7:30)

En una pantalla grande, tu texto se estira de un lado a otro y cuesta leerlo. Vamos a convertir la página en una columna centrada:

```css
body {
  background-color: lightyellow;
  font-family: Arial, sans-serif;
  max-width: 600px;
  margin: 0 auto;
  padding: 20px;
}
```

- `max-width: 600px;` dice que el contenido **no puede medir más de 600 píxeles** de ancho.
- `margin: 0 auto;` significa: **0** de margen arriba y abajo, y **auto** a los lados. "Auto" reparte el espacio sobrante en partes iguales a izquierda y derecha, y así la caja queda **centrada**.
- `padding: 20px;` deja un poco de aire para que en celulares el texto no quede pegado a la orilla.

No lo confundas con `text-align: center;` de la lección pasada: `text-align` centra el **texto dentro** de una caja, y `margin: 0 auto` centra **la caja completa**.

---

## Práctica guiada (7:30 – 8:30)

Abre el enlace de práctica que está en la descripción del video, en el editor en línea que prefieras. Los archivos de inicio (`starter-files/leccion-05/`) traen tu página de la lección anterior con sus colores, y `style.css` tiene 4 pasos marcados en comentarios:

1. En `body`, centra la página con `max-width`, `margin: 0 auto` y un poco de `padding`.
2. En `.destacado`, conviértelo en una tarjeta: fondo blanco, `border`, `padding` y `border-radius`.
3. Escribe una regla para `img` con un borde y esquinas redondeadas.
4. En `h2`, agrega `margin-top` para separar las secciones.

Prueba con distintos números para ver cómo cambia cada caja.

Ojo con el error más común: olvidar el `px`. Si escribes `padding: 15;` no pasa nada, porque el navegador no sabe si son píxeles u otra medida. Se escribe `padding: 15px;`, sin espacio entre el número y `px`.

---

## Cierre (8:30 – 9:00)

¡Tu página ya se ve ordenada, con cajas, bordes y centrada! Ya sabes todo lo necesario para crear tu propia página. En la siguiente lección armarás tu proyecto final: **tu página de perfil**.

¡Hasta la lección 6!
