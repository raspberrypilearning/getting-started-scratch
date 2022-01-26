## Depurar

**Depurar** es encontrar y corregir errores en tu código que se denominan **errores**.

* Es más fácil identificar problemas si realizas un cambio a la vez y luego ejecutas tu programa

* Es posible que se necesiten algunos experimentos para que tu proyecto funcione de la manera que planeaste

Aquí hay algunos consejos que pueden ayudarte a depurar un proyecto cuando no está haciendo lo que quieres que haga:

--- collapse ---
---
title: Ejecutar pequeños fragmentos de código
---

No necesitas ejecutar un programa completo para comprobar si los últimos bloques que has agregado nuevos funcionan.

* Haz clic en un bloque en el área de Código para ejecutarlo - es una forma rápida de verificar que un bloque está funcionando como esperas

* Para poner a prueba un conjunto de bloques por sí mismos, arrástralos lejos del script que los **contiene**, haz clic en ellos para probarlos, luego arrástralos de regreso al script principal

--- /collapse ---

--- collapse ---
---
title: Agregar demoras temporales
---

Ralentiza la **ejecución** de tu código cuando se ejecuta. Para hacer esto, agrega un bloque `esperar`{:class="block3control"} o `esperar hasta que tecla presionada`{:class="block3control"}, luego elimina el bloque cuando hayas terminado de depurar tu código.

--- /collapse ---

--- collapse ---
---
title: Mostrar variables en el Escenario
---

Si tu proyecto usa `variables`{:class="block3variables"} para almacenar datos, entonces puede ser útil mostrar esas `variables`{:class="block3variables"} en el Escenario.

Haz clic en la casilla de verificación junto a una `variable`{:class="block3variables"} en el menu de bloques `Variables`{:class="block3variables"} para mostrarla u ocultarla en el Escenario.

¿La variable siempre tiene el valor que esperas?

--- /collapse ---

--- collapse ---
---
title: Agregar comentarios
---

Agrega comentarios a bloques, conjuntos de bloques y/o scripts. Utiliza un lenguaje cotidiano para explicar lo que hace el código. A veces, esto te hará darte cuenta de que tu código no hace realmente lo que quieres que haga!

Los comentarios son útiles para cuando desees entender tu código más adelante y ayudan a otras personas a entender tus proyectos.

--- /collapse ---


Hay problemas comunes que experimentan muchos principiantes (¡y expertos!) en Scratch.

--- collapse ---
---
title: Consejos de depuración para problemas específicos
---

+ **Mi objeto va al revés** - Agrega un bloque `fijar estilo de rotación a izquierda-derecha`{:class="block3motion"} o `fijar estilo de rotación a no rotar`{:class="block3motion"}.

+ **Mi objeto 'salta' cuando cambia de disfraz o rebota** - Asegúrate de que el disfraz está centrado en el Editor de dibujo (alinea la cruz azul en el disfraz con la cruz en el centro del Editor de dibujo).

+ **Mi objeto se detiene cuando llega al borde del Escenario** - Agrega un bloque `si toca un borde, rebotar`{:class="block3motion"}.

+ **Mi sonido no se reproduce** - ¿Has agregado un bloque a `iniciar sonido`{:class="block3sound"} cuando se hace clic en el objeto? Si has copiado el código de otro objeto, deberás agregar el sonido a este objeto en la pestaña **Sonidos**. Comprueba el volumen en tu computadora o tableta, y asegúrate de no haber bajado el volumen con el código - intenta `fijar volumen a`{:class="block3sound"} `100`.

+ **Otros objetos siguen delante de mi objeto** - Usa un bloque `ir a la capa de adelante`{:class="block3looks"}.

+ **Mi objeto solo se mueve/cambia una vez** - Pon tu código dentro de un bloque `por siempre`{:class="block3control"} para que siga ejecutándose.

+ **Mi objeto no cambia cuando muevo un deslizador variable** - Pon tu código dentro de un bloque `por siempre`{:class="block3control"} para que siga actualizándose.

--- /collapse ---

**Consejo:** Si no puedes encontrar el problema después de haber probado estas técnicas, tómate un descanso o trabaja en una parte diferente de tu proyecto. ¡Cuando regreses, es posible que encuentres el error de inmediato!

