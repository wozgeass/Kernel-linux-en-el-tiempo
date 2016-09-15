# Introducción
Todos los que en algún momento hemos usado alguna **distribución linux** o celular con **android**, hemos interactuado sin saberlo con versiónes del **kernel linux**. Aunque en la actualidad las características son mas complejas y requieren en muchos casos una revisión mas extensa para poder entender los aspectos técnicos.

Si tu interes es empezar con el desarrollo del **kernel linux** muchas veces tendras que regresarte un poco para poder entender el por que agregaron ciertas tecnologías, si ese es tu interes creo que este libreo te ayudara muchísimo.

**Linux** es un sistema operativo derivado de **UNIX** que ha ganado una gran popularidad en los ultimos años, con sus ya *25 años* de vida conserva una arquitectura y estilo similares a los de cualquier otro **UNIX**; de hecho la compatibilidad  ha sido una de los principales objetivos del diseño del proyecto. Aun que su diseño es mucho mas actual que algunos **UNIX** ha sido gracias a que la comunidad de desarrolladores ha venido agregando nuevas características y solucionando un gran numero de Bugs.

# En el principio de los tiempos
Unix es el perfecto ejemplo del trabajo que se puede efectuar cuando se encauzan 

## Gnu's not Unix

Es importante resaltar que **Linux** no seria lo que es sin el proyecto llamado **GNU**.

A principios de *1984*, **Richard Stallman**, en aquella época empleado en el *AI Lab* del **MIT**, abandonó su trabajo para comenzar el proyecto **GNU**. **Stallman** se consideraba un desarrollador de los que gozaban compartiendo sus inquietudes tecnológicas y su código. Veía con desagrado cómo su negativa a firmar acuerdos de exclusividad y no compartición le estaban convirtiendo en un extraño en su propio mundo, y cómo el uso de ~~software propietario~~ en su entorno le dejaba impotente antes situaciones que antes podía solventar fácilmente.

Su idea al abandonar el **MIT** era construir un sistema de software completo, de propósito general, pero completamente libre. El sistema (y el proyecto que se encargaría de hacerlo realidad) se llamó **GNU** *(acrónimo recursivo, **GNU's Not Unix**)*. Aunque desde el principio el proyecto **GNU** incluyó en su sistema software ya disponible (como *Tex*, o más adelante, el sistema *X Window*), había mucho que construir. **Richard Stallman** comenzó por escribir un compilador de **C** (**GCC**) y un editor (**Emacs**), ambos aún en uso (y muy populares) hoy día.

Desde el principio del proyecto **GNU**, **Richard Stallman** estaba preocupado por las libertades que tendrían los usuarios de su software.
Estaba interesado en que no sólo los que recibieran los programas directamente del proyecto **GNU**, sino cualquiera que lo recibiera después de cualquier número de redistribuciones y (quizás) modificaciones, siguiera disfrutando de los mismos derechos (modificación,redistribución, etc.). Para ello, escribió la licencia **GPL**, probablemente la primera licencia de software diseñada específicamente para garantizar que un programa fuera libre en este sentido. Al mecanismo genérico que utilizan las licencias tipo **GPL** para conseguir estas garantías, **Richard Stallman** lo llamó **copyleft**, que hoy día es el nombre de una gran familia de licencias de software libre.

