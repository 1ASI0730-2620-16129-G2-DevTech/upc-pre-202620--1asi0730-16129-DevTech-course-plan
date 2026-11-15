# Guion — Lección 7: Errores comunes y próximos pasos

**Duración estimada:** 6 minutos, conforme al plan del curso.

**Público:** estudiantes que ya completaron las lecciones 1 a 6 y construyeron su perfil personal con HTML y CSS.

**Objetivo:** revisar y corregir errores en el proyecto final y definir próximos pasos después del curso.

**Cómo leerlo:** el texto normal es narración. Lo que está entre corchetes son indicaciones que no se leen. Cada sección corresponde a una diapositiva. Los tiempos son orientativos; incluye una pausa de diez segundos en la práctica y ensaya antes de grabar.

---

## Diapositiva 1: Errores comunes y próximos pasos (0:00–0:30)

[EN PANTALLA: Muestra el perfil terminado de la Lección 6 antes de pasar a la presentación. Presenta esta sesión como cierre del curso.]

¡Llegamos a la última lección! Pasaste de descubrir cómo funciona una página web a crear tu propio perfil con HTML y CSS.

Ya conoces etiquetas, listas, imágenes y enlaces. También aprendiste a cambiar colores, dar espacio y organizar tarjetas.

Hoy vamos a revisar los errores que pueden aparecer en ese proyecto y cómo encontrarlos. Al final tendrás una lista para comprobar tu página y un camino para seguir aprendiendo.

---

## Diapositiva 2: Etiquetas y secciones (0:30–1:10)

[EN PANTALLA: Señala el cierre incorrecto de section y luego la versión corregida. Relaciona con las tarjetas del perfil.]

Si una parte de tu perfil aparece en un lugar inesperado, empieza por el HTML.

Revisa que los nombres de apertura y cierre coincidan. Una sección que empieza con section debe terminar con barra section. Si un párrafo está dentro, ciérralo antes de cerrar la sección.

La sangría ayuda a reconocer esa relación, aunque no reemplaza las etiquetas.

Recuerda también que title nombra la pestaña y h1 es el título principal del contenido. Las etiquetas vacías, como img, no llevan cierre.

Mantén las secciones de tu perfil dentro de main, como hicimos en el proyecto.

---

## Diapositiva 3: Imágenes y enlaces (1:10–1:50)

[EN PANTALLA: Distingue src, alt y href. Las direcciones de ejemplo son las utilizadas en el curso.]

Si la imagen no aparece o un enlace lleva a otro lugar, revisa sus atributos.

En una imagen, src indica la dirección del archivo y alt aporta una alternativa en texto. En un enlace, href indica el destino. Comprueba los nombres y escribe los valores entre comillas.

Para enlazar una web externa, utiliza su dirección completa con https. Si la imagen falla, prueba su dirección por separado: quizá el recurso ya no esté disponible.

Y aunque cargue bien, conserva un texto alternativo útil. Ayuda a comprender el contenido sin depender de ver la imagen.

---

## Diapositiva 4: El estilo no llega a la tarjeta (1:50–2:30)

[EN PANTALLA: Muestra class="tarjeta" y .tarjeta. Explica las dos formas de conectar CSS, sin exigir archivos en JSFiddle.]

¿Tu tarjeta no cambia de color? Comprueba que el selector coincide con el HTML.

En el proyecto usamos class igual a tarjeta. En CSS, esa clase se selecciona con un punto: punto tarjeta. Sin el punto, estás buscando una etiqueta llamada tarjeta.

Si no se aplica ningún estilo, revisa dónde colocaste el CSS. En un editor con paneles separados, va en el panel CSS. Si trabajas con archivos, el link del head debe apuntar al nombre y la ubicación correctos de style.css.

Una letra distinta puede bastar para que la regla no llegue al elemento esperado.

---

## Diapositiva 5: Signos, llaves y comentarios (2:30–3:10)

[EN PANTALLA: Señala dos puntos, punto y coma y llaves en la regla. Muestra el comentario cerrado.]

A veces el selector está bien, pero una declaración tiene un error.

La forma es propiedad, dos puntos, valor y punto y coma. Las llaves delimitan la regla. Por ejemplo: color, dos puntos, purple y punto y coma.

Si falta un separador entre declaraciones, parte del estilo puede dejar de aplicarse. Por eso conviene terminar cada declaración con punto y coma.

Revisa también los comentarios: en CSS empiezan con barra asterisco y terminan con asterisco barra. Si olvidas cerrarlos, puedes dejar código dentro del comentario. Escribe los cambios fuera de esas notas.

---

## Diapositiva 6: Espacios y pantallas pequeñas (3:10–3:45)

[EN PANTALLA: Recuerda la analogía del cuadro de la Lección 5. Demuestra el panel de resultado más angosto.]

En las cajas, revisa primero las unidades. Para separar el texto del borde, padding quince necesita una medida, como quince píxeles. El cero puede escribirse sin unidad.

Padding deja espacio adentro y margin deja espacio afuera. Text-align centra el texto; para centrar una columna de bloque usamos un ancho limitado y márgenes laterales automáticos.

Después haz más angosta la vista previa. Comprueba que las imágenes se adapten y que el texto siga siendo legible. Un diseño que funciona en tu pantalla todavía necesita esa revisión.

---

## Diapositiva 7: Un cambio por vez (3:45–4:20)

[EN PANTALLA: Aplica el método a un problema real del perfil. Evita introducir herramientas nuevas.]

No cambies todo cuando algo falle. Primero describe qué esperabas y qué estás viendo.

Después busca la parte relacionada: contenido y enlaces en HTML; colores y espacios en CSS.

Haz un solo cambio, ejecuta o actualiza la vista previa y comprueba el resultado. Si trabajas con archivos, guarda antes y verifica que estés viendo el archivo correcto.

Puedes comparar con los ejemplos terminados del repositorio. Busca una diferencia concreta y explica por qué la corregiste. Así conviertes el error en aprendizaje.

---

## Diapositiva 8: Práctica: tres detalles por corregir (4:20–5:00)

[EN PANTALLA: Deja 10 segundos para buscar. En una grabación, invita a pausar. Después muestra o lee la solución incluida en las notas.]

Esta tarjeta tiene tres detalles por corregir. En el HTML su clase es tarjeta. Mira el selector, la declaración de color y el valor de padding.

Pausa el video si necesitas más tiempo.

[Deja diez segundos para revisar.]

La solución lleva un punto delante de tarjeta, dos puntos después de color y px después de dieciséis.

Ahora ejecuta el código y comprueba el color y el espacio interior. Haz después una revisión similar en una tarjeta de tu perfil.

---

## Diapositiva 9: Después del curso (5:00–5:35)

[EN PANTALLA: Presenta estos pasos como recomendaciones posteriores al curso, no como lecciones ya realizadas. MDN figura en los recursos del repositorio.]

Tu siguiente reto puede ser mejorar el perfil que ya construiste: personaliza una sección y prueba que se lea bien con una ventana estrecha.

Después puedes profundizar en diseños adaptables con Flexbox y Grid. Son temas para continuar, no requisitos para terminar este curso.

Cuando quieras añadir comportamientos, retoma JavaScript, que conocimos al principio.

Usa MDN Web Docs en español para consultar ejemplos. Conserva una copia de tu HTML y CSS y, si tu editor permite guardar y compartir, comprueba el enlace antes de enviarlo.

---

## Diapositiva 10: Tu perfil, listo para revisar (5:35–6:00)

[EN PANTALLA: Cierra mostrando el perfil. No anuncies una Lección 8 ni vuelvas a presentar la Lección 2 como futura.]

Antes de cerrar, comprueba tu perfil: etiquetas y secciones ordenadas, imágenes con alternativa en texto, enlaces correctos, estilos aplicados y contenido legible en una pantalla pequeña.

Lo importante es que puedas explicar tu página, modificarla y revisar lo que falla.

¡Felicidades por completar Fundamentos de Desarrollo Web! Ya tienes una base para seguir creando y mejorando tus propios proyectos.

---


## Práctica de la diapositiva 8

Este ejercicio nuevo retoma la clase `tarjeta` de la Lección 6. No requiere un enlace de práctica nuevo.

### Panel HTML o interior de `<body>`

```html
<section class="tarjeta">
  <h2>Sobre mí</h2>
  <p>Me gusta crear páginas web.</p>
</section>
```

### Panel CSS: versión con tres errores intencionales

```css
tarjeta {
  color purple;
  padding: 16;
}
```

### Solución

```css
.tarjeta {
  color: purple;
  padding: 16px;
}
```

Comprobación: la tarjeta muestra texto morado y 16 píxeles de relleno interior. Si trabajas con archivos, coloca el CSS en la hoja conectada desde el `<head>`; en un editor con paneles, utiliza el panel CSS.

## Lista de revisión del proyecto final

- Los títulos y secciones describen y organizan el contenido.
- Las etiquetas y su anidación corresponden a la estructura prevista.
- Las imágenes cargan y tienen alternativas en texto adecuadas a su función.
- Los enlaces abren el destino esperado.
- Las clases coinciden entre HTML y CSS y la hoja de estilos se aplica.
- Las reglas CSS tienen signos y unidades válidos.
- El texto se lee bien sobre el fondo.
- La página se revisó con una vista previa estrecha.
- Hay una copia guardada del HTML y CSS.

## Material del curso utilizado

Se revisaron los seis guiones, el plan, los archivos de inicio y los ejemplos disponibles. La rama `develop` reúne las lecciones 1 a 6; los guiones de las ramas de cada lección coinciden con esas versiones. La Lección 7 figura en el plan con una duración de 6 minutos y sin desarrollo de contenido al momento de la revisión.

- [Guion de la Lección 1](https://github.com/1ASI0730-2620-16129-G2-DevTech/upc-pre-202620--1asi0730-16129-DevTech-course-plan/blob/develop/scripts/leccion-01-script.md)
- [Guion de la Lección 2](https://github.com/1ASI0730-2620-16129-G2-DevTech/upc-pre-202620--1asi0730-16129-DevTech-course-plan/blob/develop/scripts/leccion-02-script.md)
- [Guion de la Lección 3](https://github.com/1ASI0730-2620-16129-G2-DevTech/upc-pre-202620--1asi0730-16129-DevTech-course-plan/blob/develop/scripts/leccion-03-script.md)
- [Guion de la Lección 4](https://github.com/1ASI0730-2620-16129-G2-DevTech/upc-pre-202620--1asi0730-16129-DevTech-course-plan/blob/develop/scripts/leccion-04-script.md)
- [Guion de la Lección 5](https://github.com/1ASI0730-2620-16129-G2-DevTech/upc-pre-202620--1asi0730-16129-DevTech-course-plan/blob/develop/scripts/leccion-05-script.md)
- [Guion de la Lección 6](https://github.com/1ASI0730-2620-16129-G2-DevTech/upc-pre-202620--1asi0730-16129-DevTech-course-plan/blob/develop/scripts/leccion-06-script.md)
- [Plan completo](https://github.com/1ASI0730-2620-16129-G2-DevTech/upc-pre-202620--1asi0730-16129-DevTech-course-plan/blob/develop/course-plan.md)
- [Perfil terminado de la Lección 6](https://github.com/1ASI0730-2620-16129-G2-DevTech/upc-pre-202620--1asi0730-16129-DevTech-course-plan/blob/develop/completed-examples/leccion-06/index.html)
- [CSS terminado de la Lección 5](https://github.com/1ASI0730-2620-16129-G2-DevTech/upc-pre-202620--1asi0730-16129-DevTech-course-plan/blob/develop/completed-examples/leccion-05/style.css)

### Continuidad entre lecciones

| Lección | Aprendizaje previo retomado en la Lección 7 |
|---|---|
| 1 | Diferencia entre contenido HTML, presentación CSS e interacción JavaScript. |
| 2 | Estructura del documento, etiquetas, atributos y anidación. |
| 3 | Títulos, párrafos, listas, imágenes, alternativas en texto y enlaces. |
| 4 | Conexión de CSS, selectores de clase, declaraciones y comentarios. |
| 5 | Unidades, padding, margin, centrado e imágenes adaptables. |
| 6 | Perfil con header, main, section, footer y tarjetas. |

