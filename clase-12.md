# Lógica de Primer Orden

En esta clase introdujimos los predicados de [orden superior](http://wiki.uqbar.org/wiki/articles/orden-superior.html):
 - [not/1](http://wiki.uqbar.org/wiki/articles/paradigma-logico---negacion.html) para la negación
 - [forall/2](http://wiki.uqbar.org/wiki/articles/paradigma-logico---el-forall.html) para el cuantificador universal (para todo)

De esa forma cubrimos todo lo relacionado con existencia, no existencia y para todo, que es lo que nos faltaba para poder trabajar con [lógica de primer orden](http://wiki.uqbar.org/wiki/articles/paradigma-logico---existe-vs-para-todo.html).

Recuerden que ambos predicados tienen problemas de [inversibilidad](http://wiki.uqbar.org/wiki/articles/paradigma-logico---inversibilidad.html), con lo cual hay que tomar ciertos recaudos al usarlos para que nuestros predicados sean inversibles. En general alcanza con que los parámetros de nuestros predicados lleguen unificados al consultar not/1 y forall/2, lo cual se logra consultando un predicado inversible más arriba que ligue esas variables.

Pueden encontrar el código de esta clase [acá](https://github.com/pdep-mit/ejemplos-de-clase-prolog/blob/master/clase2.pl)

## Para profundizar y ejercitar

- De la [sección de apuntes](http://www.pdep.com.ar/material/apuntes): Módulo 4 de Lógico hasta sección 4 inclusive.
- De [Mumuki](https://mumuki.io/chapters/8-programacion-logica) pueden trabajar con las guías de negación y cuantificación y además las de inversibilidad (no vimos cómo hacer cuentas hasta ahora, vale saltear los ejercicios que lo requieran).
- Ejercicios sugeridos:
  - TEG 2 (guía 4)
  - Gran compañero de viaje (guía 4)
  - Asesinato (guía 7)

[< Clase anterior](https://github.com/pdep-mit/bitacora-de-clase/blob/master/clase-11.md)
