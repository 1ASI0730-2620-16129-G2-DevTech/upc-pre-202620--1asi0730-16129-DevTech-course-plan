# Guión — Lección 5: Cajas, bordes y centrado

**Duración estimada**: 10 minutos

> **Cómo leer este guion**: el texto normal es la narración en off. Lo que está entre **[corchetes]** no se lee: son indicaciones para grabar y editar.
> - **[EN PANTALLA]**: texto o imagen que aparece en el video.
> - **[ANOTACIÓN]**: flechas, recuadros o resaltados sobre el código.
> - **[ZOOM]**: acercar la grabación a una parte del código.
> - **[DEMO]**: acción que se muestra en vivo en JSFiddle.
> - **[LETRERO]**: cartel grande que se queda unos segundos en pantalla.

---

## Gancho (0:00 – 0:30)

**[EN PANTALLA: la página "Mis cosas favoritas" de la lección 4, pegada al borde izquierdo y estirada de lado a lado]**

Tu página "Mis cosas favoritas" ya tiene colores y su propio tipo de letra. Pero mírala bien: todo está pegado al borde izquierdo de la pantalla y apretado.

**[TRANSICIÓN: la misma página centrada, con la tarjeta del párrafo destacado y la imagen con bordes redondeados]**

Ahora mírala así. ¡Mucho más ordenada! Hoy vas a aprender a darle **espacio**, **bordes** y a **centrar** tu página.

**[EN PANTALLA: "Lección 5: Cajas, bordes y centrado"]**

---

## Todo es una caja (0:30 – 1:45)

**[EN PANTALLA: "🔑 El secreto de CSS: todo es una caja"]**

Este es el secreto más importante de CSS: **cada elemento de tu página es una caja**. Un título es una caja, un párrafo es una caja, una imagen es una caja.

**[DEMO: agregar por un momento `* { border: 1px solid red; }` en el panel CSS y presionar Run. Todas las cajas de la página se ven con un borde rojo. Luego borrar esa línea]**

¿Lo ves? Cada parte de tu página es una caja, aunque normalmente no se note.

Piensa en un **cuadro colgado en la pared**:

**[EN PANTALLA: foto de un cuadro real a la izquierda y, a la derecha, el diagrama de 4 cajas, una dentro de otra, con los mismos colores: contenido (azul), padding (verde), border (naranja), margin (gris)]**

- La **foto** es el contenido.
- El cartón blanco alrededor de la foto es el **padding** (relleno).
- El **marco** es el **border** (borde).
- El espacio en la pared hasta el siguiente cuadro es el **margin** (margen).

**[ANOTACIÓN: cada parte del cuadro se ilumina al mismo tiempo que su parte en el diagrama, mientras se nombra]**

Así funcionan todas las cajas de tu página: contenido, padding, border y margin, de adentro hacia afuera.

---

## Bordes (1:45 – 3:00)

**[DEMO: escribir en vivo en la regla `.destacado` del panel CSS]**

Empecemos por el marco. Para ponerle borde a un elemento usamos `border`:

```css
.destacado {
  border: 2px solid purple;
}
```

**[ANOTACIÓN: flechas de colores. `2px` → "GROSOR" · `solid` → "ESTILO" · `purple` → "COLOR"]**

El valor tiene tres partes:

- `2px` es el **grosor** del borde.
- `solid` es el **estilo**: una línea continua. También puedes probar `dashed` (rayitas) o `dotted` (puntitos).
- `purple` es el **color**.

**[DEMO: cambiar `solid` por `dashed` y luego por `dotted`, presionando Run cada vez]**

**[LETRERO: "⏸️ Pausa el video y prueba los 3 estilos de borde en tu página"]**

Pausa el video y prueba los tres estilos en tu página. … ¿Cuál te gustó más? Sigamos.

Ahora sí puedes ver la caja del párrafo. Fíjate que el texto queda pegado al borde…

**[ZOOM: el texto pegado al borde]**

… eso lo arreglamos con el padding.

---

## Padding: el espacio de adentro (3:00 – 4:15)

**[EN PANTALLA: en el diagrama del cuadro se ilumina solo el cartón (padding, verde)]**

El `padding` es el espacio **entre el contenido y el borde**, como el cartón blanco del cuadro:

```css
.destacado {
  border: 2px solid purple;
  padding: 15px;
  background-color: white;
}
```

**[DEMO: agregar `padding: 15px;` y presionar Run. Luego agregar `background-color: white;` y presionar Run]**

Con `padding: 15px;` el texto se separa 15 píxeles del borde por todos los lados. Le pusimos fondo blanco para que veas mejor que el padding forma parte de la caja: el fondo también pinta el relleno.

**[LETRERO: "🤔 ¿Qué pasará si cambio padding por margin?"]**

Una pregunta: ¿qué pasará si cambio `padding` por `margin`? Piénsalo un segundo…

**[DEMO: cambiar `padding: 15px;` por `margin: 15px;` y presionar Run. El texto vuelve a pegarse al borde y la caja entera se aleja de las demás. Luego regresar a `padding`]**

¡El texto se vuelve a pegar al borde! Y en lugar de eso, toda la caja se alejó de las demás. Eso es justamente lo que hace el margin. Veámoslo.

---

## Margin: el espacio de afuera (4:15 – 5:15)

**[EN PANTALLA: en el diagrama del cuadro se ilumina solo el espacio en la pared (margin, gris)]**

El `margin` es el espacio **fuera del borde**, que separa una caja de las demás:

```css
h2 {
  color: crimson;
  margin-top: 30px;
}
```

**[DEMO: agregar `margin-top: 30px;` en `h2` y presionar Run. Las secciones se separan]**

Con `margin-top` agregamos espacio solo **arriba** de cada `h2`, así cada sección queda más separada de la anterior. También existen `margin-bottom` (abajo), `margin-left` (izquierda) y `margin-right` (derecha). Si escribes solo `margin`, cambia los cuatro lados a la vez.

**[LETRERO: "💡 padding = adentro · margin = afuera"]**

Un truco para no confundirte: **padding es adentro, margin es afuera**.

---

## Esquinas redondeadas (5:15 – 6:15)

**[DEMO: escribir en vivo una regla nueva para `img`]**

Las cajas tienen esquinas en punta, pero puedes redondearlas con `border-radius`:

```css
img {
  border: 4px solid crimson;
  border-radius: 15px;
}
```

**[DEMO: cambiar el número de `border-radius` de 5px a 15px y luego a 30px, presionando Run cada vez]**

Mientras más grande el número, más redondas las esquinas. ¡Tu foto ahora parece una tarjeta!

**[DEMO: agregar `border-radius: 10px;` en `.destacado` y presionar Run]**

Y no solo sirve para imágenes: `border-radius` funciona con **cualquier caja**. Si se lo pones a tu párrafo `.destacado`, que ya tiene borde y fondo blanco, ¡se convierte en una tarjeta con esquinas redondeadas!

---

## Centrar la página (6:15 – 8:00)

**[EN PANTALLA: la página en una pantalla ancha, con el texto estirado de lado a lado]**

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

**[DEMO: agregar las 3 líneas en `body` una por una, presionando Run después de cada una]**

- `max-width: 600px;` dice que el contenido **no puede medir más de 600 píxeles** de ancho.
- `margin: 0 auto;` significa: **0** de margen arriba y abajo, y **auto** a los lados. "Auto" reparte el espacio sobrante en partes iguales a izquierda y derecha, y así la caja queda **centrada**.
- `padding: 20px;` deja un poco de aire para que en celulares el texto no quede pegado a la orilla.

**[ANOTACIÓN: dos flechas iguales a los lados de la columna con el texto "auto = mismo espacio a cada lado"]**

¿Y la imagen? Mide 400 píxeles de ancho, pero en un celular la columna es más angosta, así que la imagen **se saldría** de la página. Lo arreglamos con una línea en la regla de `img`:

```css
img {
  border: 4px solid crimson;
  border-radius: 15px;
  max-width: 100%;
}
```

**[DEMO: angostar el panel de resultado de JSFiddle hasta el tamaño de un celular, primero sin `max-width: 100%` (la imagen se sale) y luego con esa línea (la imagen se achica sola)]**

`max-width: 100%;` significa: "la imagen nunca puede ser más ancha que su caja". En una computadora se ve igual, y en un celular se achica sola para caber. Así tu página se ve bien en **cualquier pantalla**.

**[EN PANTALLA: "text-align: center → centra el TEXTO dentro de la caja · margin: 0 auto → centra LA CAJA completa"]**

No lo confundas con `text-align: center;` de la lección pasada: `text-align` centra el **texto dentro** de una caja, y `margin: 0 auto` centra **la caja completa**.

---

## Práctica guiada (8:00 – 9:15)

**[EN PANTALLA: abrir el enlace de práctica desde la descripción del video]**

¡Ahora te toca a ti! Abre el enlace de práctica que está en la descripción del video, en el editor en línea que prefieras. Los archivos de inicio (`starter-files/leccion-05/`) traen tu página de la lección anterior con sus colores, y `style.css` tiene 4 pasos marcados en comentarios:

**[EN PANTALLA: los 4 pasos en una lista]**

1. En `.destacado`, conviértelo en una tarjeta: fondo blanco, `border`, `padding` y `border-radius`.
2. En `h2`, agrega `margin-top` para separar las secciones.
3. Escribe una regla para `img` con un borde, esquinas redondeadas y `max-width: 100%;`.
4. Por último, en `body`, centra la página con `max-width`, `margin: 0 auto` y un poco de `padding`.

Los pasos siguen el mismo orden de esta lección: primero las cajas, luego los espacios y al final el centrado.

**[ZOOM: `padding: 15;` tachado en rojo ❌ al lado de `padding: 15px;` en verde ✅]**

Ojo con el error más común: olvidar el `px`. Si escribes `padding: 15;` no pasa nada, porque el navegador no sabe si son píxeles u otra medida. Se escribe `padding: 15px;`, sin espacio entre el número y `px`.

**[LETRERO GRANDE: "⏸️ PAUSA EL VIDEO Y PRACTICA"]**

Pausa el video ahora y vuelve cuando termines. Prueba con distintos números para ver cómo cambia cada caja.

**[EN PANTALLA: la solución terminada durante unos segundos]**

¿Ya está? Así queda una solución. La tuya puede tener otros números y colores, ¡y está perfecto!

Para comprobar que tu página se adapta, haz más angosta la ventana del navegador (o el panel de resultado): la imagen debe achicarse y nunca salirse de la columna.

---

## Resumen, reto y cierre (9:15 – 10:00)

**[EN PANTALLA: lista que aparece línea por línea]**
**"Hoy aprendiste:**
**✔ Todo es una caja**
**✔ `border`: el marco**
**✔ `padding`: el espacio de adentro**
**✔ `margin`: el espacio de afuera**
**✔ `border-radius`: esquinas redondeadas**
**✔ Centrar la página con `margin: 0 auto`**
**✔ Imágenes que se adaptan con `max-width: 100%`"**

Hoy aprendiste que todo es una caja, a ponerle bordes, a darle espacio por dentro y por fuera, a redondear las esquinas y a centrar tu página para que se vea bien en cualquier pantalla.

**[LETRERO: "🏆 Reto extra: convierte tu imagen en un óvalo con border-radius: 50%; y prueba un borde dashed en tu tarjeta"]**

Y si quieres un reto extra: ponle `border-radius: 50%;` a tu imagen y mira cómo se convierte en un **óvalo**. Y prueba un borde `dashed` en tu tarjeta.

¡Tu página ya se ve ordenada, con cajas, bordes y centrada! Ya sabes todo lo necesario para crear tu propia página. En la siguiente lección armarás tu proyecto final: **tu página de perfil**.

**[EN PANTALLA: "Siguiente: Lección 6, Proyecto final: tu página de perfil"]**

¡Hasta la lección 6!
