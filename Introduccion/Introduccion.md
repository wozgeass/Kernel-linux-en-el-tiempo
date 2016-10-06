# Introducción
Todos los que en algún momento hemos usado alguna **distribución linux** o celular con **android**, hemos interactuado sin saberlo con versiónes del **kernel linux**. Aunque en la actualidad las características son más complejas y requieren en muchos casos una revisión más extensa para poder entender los aspectos técnicos.

Si tu interes es empezar con el desarrollo del **kernel linux** muchas veces tendras que regresarte un poco para poder entender el por que agregaron ciertas caracteristicas, si ese es tu interes creo que este libro te ayudara muchísimo.

**Linux** es un sistema operativo derivado de **UNIX** que ha ganado una gran popularidad en los ultimos años, con sus ya *25 años* de vida conserva una arquitectura y estilo similares a los de cualquier otro **UNIX**; de hecho la compatibilidad  ha sido una de los principales objetivos del diseño del proyecto. Su diseño es mucho más actual que algunos **UNIX** ha sido gracias a que la comunidad de desarrolladores ha venido agregando nuevas características y solucionado un gran numero de Bugs.

# En el principio de los tiempos
**UNIX** es el perfecto ejemplo del trabajo que se puede efectuar cuando se encauzan todas las energias a la busqueda de un ideal tecnologico. Cuando *AT&T* distribuye casi libremente en 1974 el código fuente del sistema operativo a la Universidades por que, entre otras razones, no ve ningun futuro economico a su producto. No parece dudar del entusiasmo de los estudiantes, profesores e investigadores de la Computacion. Esta primer comunidad pasara mucho tiempo modificando y mejorando el producto, subiendo todas la novedades a *AT&T* para que se integre al producto oficial. Tras el cambio de licencia en 1978, la energia de la comunidad se encauzo hacia el proyecto Universitario **BSD**, dejando al **UNIX** comercial de AT&T.

Los primeros ordenadores eran escencialmente herramientas de investigacion en manos de universitarios y necesidades militares. En los laboratorios de investigacion, los programas circulaban como las ideas: libremente. Era absolutamente normal que un programa desarrollado por un equipo de programadores o investigadores se distribuyera a otros equipos de otras universidades y a cualquier otro lugar donde hiciera falta.

Y nada habia de raro en que este programa fuera modificado por otro equipo, y asi sucesivamente. A dia de hoy, cuando un ilustre matematico demuestra un teorema dificil, publica el resultado de sus investigaciones en obras especializadas con el fin de ayudar al progreso de la ciencia. Todo el mundo tiene acceso a ello.

Pero el universo de la computación ha seguido otros caminos. Pese a ser una ciencia, el futuro de las investigaciones no se circunscribe al mundo Universitario. 

Rapidamente las empresas vieron el inmenso interes de automatizar varias de sus tareas, como la contabilidad, los pagos, etc. Con la compra de los primeros grandes ordenadores de gestion, se necesitaron programas. Estos programas tuvieron que ser protegidos como secretos industriales, habia nacido una nueva industria: el desarrollo de programas. Con su entrada en la dinamica de las grandes empresas, la Computacion perdio rapidamente la inocencia y se hizo mucho menos libre. Se empezo a hablar de licencias, impuestos, tasas, prohibición de copia.

## El proyecto GNU y la FSF

Es importante resaltar que **Linux** no seria lo que es sin el proyecto llamado **GNU**.

A principios de *1984*, **Richard Stallman**, en aquella época empleado en el *AI Lab* del **MIT**, abandonó su trabajo para comenzar el proyecto **GNU**. **Stallman** se consideraba un desarrollador de los que gozaban compartiendo sus inquietudes tecnológicas y su código. Veía con desagrado cómo su negativa a firmar acuerdos de exclusividad y no compartición le estaban convirtiendo en un extraño en su propio mundo, y cómo el uso de ~~software propietario~~ en su entorno le dejaba impotente ante situaciones que antes podía solventar fácilmente.

Su idea al abandonar el **MIT** era construir un sistema de software completo, de propósito general, pero completamente libre. El sistema (y el proyecto que se encargaría de hacerlo realidad) se llamó **GNU** *(acrónimo recursivo, **GNU's Not Unix**)*. Aunque desde el principio el proyecto **GNU** incluyó en su sistema software ya disponible (como *Tex*, o más adelante, el sistema *X Window*), había mucho que construir. **Richard Stallman** comenzó por escribir un compilador de **C** (**GCC**) y un editor (**Emacs**), ambos aún en uso (y muy populares) hoy día.

Desde el principio del proyecto **GNU**, **Richard Stallman** estaba preocupado por las libertades que tendrían los usuarios de su software.

Estaba interesado en que no sólo los que recibieran los programas directamente del proyecto **GNU**, sino cualquiera que lo recibiera después de cualquier número de redistribuciones y (quizás) modificaciones, siguiera disfrutando de los mismos derechos (modificación,redistribución, etc.). Para ello, escribió la licencia **GPL**, probablemente la primera licencia de software diseñada específicamente para garantizar que un programa fuera libre en este sentido. Al mecanismo genérico que utilizan las licencias tipo **GPL** para conseguir estas garantías, **Richard Stallman** lo llamó **copyleft**, que hoy día es el nombre de una gran familia de licencias de software libre.

Richard Stallman también fundó la **Free Software Foundation** (**FSF**) con el fin de conseguir fondos para el desarrollo y la protección del **software libre**, y sentó los fundamentos éticos del **software libre**, con documentos como **The GNU Manifesto y Why Software Should Not Have Owners**.

Desde el punto de vista técnico, el proyecto **GNU** fue concebido como un trabajo muy estructurado y con metas muy claras. El método habitual estaba basado en grupos relativamente pequeños de personas (habitualmente voluntarios) que desarrollaban alguna de las herramientas que luego encajarían perfectamente en el rompecabezas completo (el sistema **GNU**). La modularidad de **UNIX**, en la que se inspiraba el desarrollo, encajaba perfectamente en esta idea.

El método de trabajo generalmente implicaba el uso de Internet, pero ante la escasa implantación de aquellos días, la **Free Software Foundation** también vendía cintas en las que grababa las aplicaciones, siendo probablemente uno de las primeras organizaciones en beneficiarse económicamente (aunque de manera bastante limitada) de la creación de **software libre**.

A principios de la década de 1990, unos seis años después de su nacimiento, el proyecto GNU estaba muy cerca de tener un sistema completo similar a Unix. Aun así, hasta ese momento todavía no ha-
ANOTACIONES bía producido una de las piezas fundamentales: el kernel del sistema (el núcleo del sistema operativo que se relaciona con el hardware y permite que todo funcione). Sin embargo, el software de GNU era muy popular entre los usuarios de las distintas variantes de Unix, por aquella época el sistema operativo más usado en las empresas. Además, el proyecto GNU había conseguido ser relativamente conocido entre los profesionales informáticos, y muy especialmente entre los
que trabajaban en universidades. En esa época, sus productos ya gozaban de una merecida reputación de estabilidad y calidad.

A continuación te mostrare una tabla con los proyectos que **GNU** considera son proyectos **software libre**.

| **Proyectos GNU** |
| :--: | :--: | :--: | :--: |
| *3dldf* | 1:2 | 2:2 | 3:2 |
| *anubis* | 1:3 | 2:3 | 3:3 |
| *autoconf* | 1:4 | 2:4 | 3:4 |
| *bash* | 1:5 | 2:5 | 3:5 |
| *bool* | 1:6 | 2:6 | 3:6 |
| *ccscript* | 1:7 | 2:7 | 3:7 |
| *clisp* | 1:8 | 2:8 | 3:8 |
| *coreutils* | 1:9 | 2:9 | 3:9 |
| *dc* | 1:10 | 2:10 | 3:10 |
| *diction* | 1:11 | 2:11 | 3:11 |
| *easejs* | 1:12 | 2:12 | 3:12 |
| *enscript* | 1:13 | 2:13 | 3:13 |
| *foliot* | 1:14 | 2:14 | 3:14 |
| *fribidi* | 1:15 | 2:15 | 3:15 |
| *gcide* | 1:16 | 2:16 | 3:16 |
| *gleem* | 1:17 | 2:17 | 3:17 |
| *gnash* | 1:17 | 2:17 | 3:17 |
| *gettext* | 1:17 | 2:17 | 3:17 |
| *gnu-c-manual* | 1:17 | 2:17 | 3:17 |
| *gnubiff* | 1:17 | 2:17 | 3:17 |
| *gnue* | 1:17 | 2:17 | 3:17 |
| *gnulib* | 1:17 | 2:17 | 3:17 |
| *gnupg* | 1:17 | 2:17 | 3:17 |
| *gnusound* | 1:17 | 2:17 | 3:17 |
| *gnuzilla* | 1:17 | 2:17 | 3:17 |
| *greg* | 1:17 | 2:17 | 3:17 |
| *gsl* | 1:17 | 2:17 | 3:17 |
| *guile* | 1:17 | 2:17 | 3:17 |
| *guix* | 1:17 | 2:17 | 3:17 |
| *health* | 1:17 | 2:17 | 3:17 |
| *hyperbole* | 1:17 | 2:17 | 3:17 |
| *intlfonts* | 1:17 | 2:17 | 3:17 |
| *kopi* | 1:17 | 2:17 | 3:17 |
| *libextractor* | 1:17 | 2:17 | 3:17 |
| *libmicrohttpd* | 1:17 | 2:17 | 3:17 |
| *libunistring* | 1:17 | 2:17 | 3:17 |
| *lispintro* | 1:17 | 2:17 | 3:17 |
| *make* | 1:17 | 2:17 | 3:17 |
| *mediagoblin* | 1:17 | 2:17 | 3:17 |
| *mit-scheme* | 1:17 | 2:17 | 3:17 |
| *nana* | 1:17 | 2:17 | 3:17 |
| *octave* | 1:17 | 2:17 | 3:17 |
| *pexec* | 1:17 | 2:17 | 3:17 |
| *powerguru* | 1:17 | 2:17 | 3:17 |
| *qexo* | 1:17 | 2:17 | 3:17 |
| *reftex* | 1:17 | 2:17 | 3:17 |
| *screen* | 1:17 | 2:17 | 3:17 |
| *shtool* | 1:17 | 2:17 | 3:17 |
| *speex* | 1:17 | 2:17 | 3:17 |
| *superopt* | 1:17 | 2:17 | 3:17 |
| *termutils* | 1:17 | 2:17 | 3:17 |
| *tramp* | 1:17 | 2:17 | 3:17 |
| *uucp* | 1:17 | 2:17 | 3:17 |
| *websocket4j* | 1:17 | 2:17 | 3:17 |
| *xhippo* | 1:17 | 2:17 | 3:17 |
| *8sync* | 1:17 | 2:17 | 3:17 |
| *autoconf-archive* | 1:17 | 2:17 | 3:17 |
| *apl* | 1:17 | 2:17 | 3:17 |
| *bayonne* | 1:17 | 2:17 | 3:17 |
| *bpel2owfn* | 1:17 | 2:17 | 3:17 |
| *cflow* | 1:17 | 2:17 | 3:17 |
| *cobol* | 1:17 | 2:17 | 3:17 |
| *cpio* | 1:17 | 2:17 | 3:17 |
| *ddd* | 1:17 | 2:17 | 3:17 |
| *diffutils* | 1:17 | 2:17 | 3:17 |
| *ed* | 1:17 | 2:17 | 3:17 |
| *eprints* | 1:17 | 2:17 | 3:17 |
| *fontopia* | 1:17 | 2:17 | 3:17 |
| *g-golf* | 1:17 | 2:17 | 3:17 |
| *gcl* | 1:17 | 2:17 | 3:17 |
| *gforth* | 1:17 | 2:17 | 3:17 |
| *glib* | 1:17 | 2:17 | 3:17 |
| *gnat* | 1:17 | 2:17 | 3:17 |
| *gnu-crypto* | 1:17 | 2:17 | 3:17 |
| *gnubik* | 1:17 | 2:17 | 3:17 |
| *gnufm* | 1:17 | 2:17 | 3:17 |
| *gnumach* | 1:17 | 2:17 | 3:17 |
| *gnupod* | 1:17 | 2:17 | 3:17 |
| *gnuspeech* | 1:17 | 2:17 | 3:17 |
| *goptical* | 1:17 | 2:17 | 3:17 |
| *grep* | 1:17 | 2:17 | 3:17 |
| *gslip* | 1:17 | 2:17 | 3:17 |
| *guile-dbi* | 1:17 | 2:17 | 3:17 |
| *xhippo* | 1:17 | 2:17 | 3:17 |
| *xhippo* | 1:17 | 2:17 | 3:17 |
| *xhippo* | 1:17 | 2:17 | 3:17 |
| *xhippo* | 1:17 | 2:17 | 3:17 |
| *xhippo* | 1:17 | 2:17 | 3:17 |
| *xhippo* | 1:17 | 2:17 | 3:17 |
| *xhippo* | 1:17 | 2:17 | 3:17 |
| *xhippo* | 1:17 | 2:17 | 3:17 |
| *xhippo* | 1:17 | 2:17 | 3:17 |
| *xhippo* | 1:17 | 2:17 | 3:17 |
| *xhippo* | 1:17 | 2:17 | 3:17 |
| *xhippo* | 1:17 | 2:17 | 3:17 |
