# Excepciones

En esta clase estuvimos hablando sobre [excepciones](http://wiki.uqbar.org/wiki/articles/excepciones.html), cómo usarlas, cuándo usarlas y qué hacer al respecto cuando ocurren. También vimos qué herramientas hay disponibles para poder testear los casos infelices, donde lo esperado es que un envío de mensajes resulte en un error.

El manejo de errores no es algo propio del paradigma de objetos, sin embargo forma parte de las herramientas básicas que ofrecen los lenguajes que se basan en él.

En funcional (en particular en Haskell) vimos que existen funciones que lanzan errores (por ejemplo, `head []` estalla porque no tiene ninguna respuesta razonable), pero como cortar el flujo de ejecución va bastante en contra de la ausencia de efecto, a su vez propone otra alternativa para aquellos problemas que consideremos recuperables que se atienen a la idea de función. Esto es algo que excede el alcance de esta materia, los curiosos pueden investigar qué es una Mónada o mejor aún, cursar [Técnicas Avanzadas de Programación](http://tadp-utn-frba.github.io/contenidos/).

Pueden encontrar el código de la clase [acá](https://github.com/pdep-mit/ejemplos-de-clase-wollok/tree/master/ejemplos-de-clase/src/clase7).

## Para profundizar

- De la [sección de apuntes](http://www.pdep.com.ar/material/apuntes):
  - El Módulo 10 explica la necesidad, buenos y malos usos.
  - El Módulo 11 explica, entre muchas otras cosas que pueden interesarles, cómo testear casos infelices.

[< Clase anterior](https://github.com/pdep-mit/bitacora-de-clase/blob/master/clase-22.md) - Clase siguiente >
