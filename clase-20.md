# Colecciones

En esta clase vimos cómo trabajar con [Colecciones](http://wiki.uqbar.org/wiki/articles/intro-a-colecciones.html):
  - Vimos que en Wollok existen dos tipos de colecciones: [las listas y los sets](http://wiki.uqbar.org/wiki/articles/sabores-de-colecciones.html). Es común que cada lenguaje defina distintos tipos de colecciones para poder elegir cuál usar en base a la necesidad para cada problema.
  - También vimos algunos de los [mensajes que entienden las colecciones](http://wiki.uqbar.org/wiki/articles/mensajes-de-colecciones.html) de Wollok. Algunos eran muy similares a los que ya conocíamos de Haskell, otros directamente no estaban en Haskell porque están pensados para trabajar con efecto colateral.
  
Además empezamos a hablar un poquito sobre la idea de error (o [excepción](http://wiki.uqbar.org/wiki/articles/excepciones.html)). Vamos a retomar ese tema más adelante, nos faltan incorporar más herramientas, pero en principio queremos que quede claro que hay veces que el **comportamiento esperado** como resultado de un envío de mensaje es **que falle**, interrumpiendo la ejecución de ese mensaje y de aquellos que se enviaron hasta llegar a ese punto de la ejecución. Está bien que un método lance una excepción cuando no puede cumplir con lo que prometía que iba a hacer (por ejemplo, obtener el primer elemento de una lista que no tiene ningún elemento). Con eso nos alcanza de momento, más adelante profundizaremos sobre lo que falta, pero sobre todo vamos a **formar criterio** sobre cómo usarlas.

El código de la clase lo pueden encontrar [acá](https://github.com/pdep-mit/ejemplos-de-clase-wollok/tree/master/src/clase04).

> Pueden encontrar un ejemplo de testeo de casos excepcionales [acá](https://github.com/pdep-mit/ejemplos-de-clase-wollok/blob/master/src/clase04/atencionDeAnimales_parte1.wtest#L131).

De la [sección de apuntes](http://www.pdep.com.ar/material/apuntes): el módulo 4 explica cómo trabajar con los distintos tipos de colecciones. El módulo 10 aborda todo lo relativo a excepciones, incluyendo temas **que no vimos todavía**.

[< Clase anterior](https://github.com/pdep-mit/bitacora-de-clase/blob/master/clase-19.md) - [Clase siguiente >](https://github.com/pdep-mit/bitacora-de-clase/blob/master/clase-21.md)
