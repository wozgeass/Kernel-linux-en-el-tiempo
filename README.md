# Kernel linux en el tiempo

En este libro tratare de presentar un estudio lo mas detallado posible sobre los cambio que han sido agregados en el  **kernel linux** hasta llegar a lo que se ha implementado en la actualidad.

Toma en cuenta que las primeras versiones no estuvieron bien documentados los cambios, pero estaremos revisando las características agregadas desde el primer release del  **kernel**.

Así entenderemos como ha sido la evolución del  **kernel** en sus 28 años de vida.

Básicamente se trata de una recopilación de las características agregadas a los kernels al pasar de cada versión.

Comienzos
| **Versión** |            **Fecha**            |
|:-----------:|:-------------------------------:|
|  **0.01**   |    **17 de Septiembre 1991**    |
|     0.2     |        4 de Octubre 1991        |
|    0.11     |       8 de Diciembre 1991       |
|    0.95     |         7 de Marzo 1992         |

Inicio de la madures

| **Versión** | **Fecha**            |
| ----------- | -------------------- |
| **1.0**     | **13 de Marzo 1994** |
| 1.1         | 6 de Abril 1994      |
| 1.2         | 6 de Abril 1995      |
| 1.3         | 12 de Junio 1995     |

Inicio de la madurez

| **versión** | **Fecha**             |
| ----------- | --------------------- |
| **2.0**     | **9 de Junio 1996**   |
| 2.1         | 30 de Septiembre 1996 |
| 2.2         | 26 de Enero 1999      |
| 2.3         | 11 de Mayo 1999       |
| 2.4         | 4 de Enero 2001       |
| 2.5         | 23 de Noviembre 2001  |
| 2.6         | 18 de Diciembre 2003  |
| 2.6.1       | 9 de Enero 2004       |
| 2.6.2       | 4 de Febrero 2004     |
| 2.6.3       | 18 de Febrero 2004    |
| 2.6.4       | 11 de Marzo 2004      |
| 2.6.5       | 4 de Abril 2004       |
| 2.6.6       | 10 de Mayo 2004       |
| 2.6.7       | 16 de Junio 2004      |
| 2.6.8       | 14 de Agosto 2004     |
| 2.6.9       | 19 de Octubre 2004    |
| 2.6.10      | 24 de Diciembre 2004  |
| 2.6.11      | 2 de Marzo 2006       |
| 2.6.12      | 17 de Junio 2005      |
| 2.6.13      | 29 de Agosto 2005     |
| 2.6.14      | 27 de Octubre 2005    |
| 2.6.15      | 3 de Enero 2006       |
| 2.6.16      | 20 de Marzo 2006      |
| 2.6.17      | 17 de Junio 2006      |
| 2.6.18      | 20 de Septiembre 2006 |
| 2.6.19      | 19 de Noviembre 2006  |
| 2.6.20      | 5 de Febrero 2007     |
| 2.6.21      | 26 de Abril 2007      |
| 2.6.22      | 8 de Julio 2007       |
| 2.6.23      | 9 de Octubre 2007     |
| 2.6.24      | 25 de Enero 2008      |
| 2.6.25      | 16 de Abril 2008      |
| 2.6.26      | 13 de Julio 2008      |
| 2.6.27      | 9 de Octubre 2008     |
| 2.6.28      | 25 de Diciembre 2008  |
| 2.6.29      | 24 de Marzo 2009      |
| 2.6.30      | 9 de Junio 2009       |
| 2.6.31      | 9 de Septiembre 2009  |
| 2.6.32      | 3 de Diciembre 2009   |
| 2.6.33      | 24 de Febrero 2010    |
| 2.6.34      | 16 de Mayo 2010       |
| 2.6.35      | 1 de Agosto 2010      |
| 2.6.36      | 20 de Octubre 2010    |
| 2.6.37      | 4 de Enero 2011       |
| 2.6.38      | 14 de Marzo 2011      |
| 2.6.39      | 18 de Mayo 2011       |

Madurez

| **Versión** | **Fecha**                       |
| ----------- | ------------------------------- |
| **3.0**     | **21 de Julio 2011**            |
| 3.1         | 24 de Octubre 2011              |
| 3.2         | 4 de Enero 2012                 |
| 3.3         | 18 de Marzo 2012                |
| 3.4         | 20 de Mayo 2012                 |
| 3.5         | 21 de Julio 2012                |
| 3.6         | 20 de Mayo 2012                 |
| 3.7         | 10 de Diciembre 2012            |
| 3.8         | 18 de Febrero 2013              |
| 3.9         | 28 de Abril 2013                |
| 3.10        | 30 de Junio 2013                |
| 3.11        | 2 de Septiembre 2013            |
| 3.12        | 2 de Noviembre 2013             |
| 3.13        | 19 de Enero 2014                |
| 3.14        | 30 de Marzo 2014                |
| 3.15        | 8 de Junio 2014                 |
| 3.16        | 3 de Agosto 2014                |
| 3.17        | 5 de Octubre 2014               |
| 3.18        | 7 de Diciembre 2014             |
| 3.19        | 8 de Febrero 2015               |

Profesionalizacion.

| **Versión** | **Fecha**            |
| ----------- | -------------------- |
| **4.0**     | **12 de Abril 2015** |
| 4.1         | 21 de Junio 2015     |
| 4.2         | 30 de Agosto 2015    |
| 4.3         | 1 de Noviembre 2016  |
| 4.4         | 10 de Enero 2016     |
| 4.5         | 13 de Marzo 2016     |
| 4.6         | 15 de Mayo 2016      |
| 4.7         | 24 de Julio 2016     |
| 4.8         | 2 de Septiembre 2016 |
| 4.9         | 7 de Diciembre 2016  |
| 4.10        | 8 de Febrero 2017    |
| 4.11        | 19 de Abril 2017     |
| 4.12        | 2 de Julio 2017      |
| 4.13        | 3 de Septiembre 2017 |
| 4.14        | 12 de Noviembre 2017 |
| 4.15        | 18 de Enero 2018     |
| 4.16        | 1 de Abril 2018      |
| 4.17        | 3 de Junio 2018      |
| 4.18        | 12 de Agosto 2018    |
| 4.19        | 22 de Octubre 2018   |
| 4.20        | 23 de Diciembre 2018 |

Actualidad

| **Versión** | **Fecha**                   |
| ----------- | --------------------------- |
| **5.0**     | **3 de marzo 2019**         |
| 5.1         | 5 de mayo de 2019           |
| 5.2         | 7 de Julio 2019             |
| **5.3**     | **Mediados de Septiembre** |
| **5.4**     | **Por Definir**             |
