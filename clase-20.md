# Bloques y Colecciones

En esta clase vimos dos tipos de objetos muy útiles:
- [Bloques](http://wiki.uqbar.org/wiki/articles/bloques.html)
- [Colecciones](http://wiki.uqbar.org/wiki/articles/intro-a-colecciones.html)
  - Vimos que en Wollok existen dos tipos de colecciones: [las listas y los sets](http://wiki.uqbar.org/wiki/articles/sabores-de-colecciones.html). Es común que cada lenguaje defina distintos tipos de colecciones para poder elegir cuál usar en base a la necesidad para cada problema.
  - También vimos algunos de los [mensajes que entienden las colecciones](http://wiki.uqbar.org/wiki/articles/mensajes-de-colecciones.html) de Wollok. Algunos eran muy similares a los que ya conocíamos de Haskell, otros directamente no estaban en Haskell porque están pensados para trabajar con efecto colateral.
  
Además empezamos a hablar un poquito sobre la idea de error (o excepción). Vamos a retomar ese tema más adelante, pero en principio queremos que quede claro que hay veces que el **comportamiento esperado** como resultado de un envío de mensaje es **que falle**, interrumpiendo la ejecución de ese mensaje y de aquellos que se enviaron hasta llegar a ese punto de la ejecución. Está bien que un método lance una excepción cuando no puede cumplir con lo que prometía que iba a hacer (por ejemplo, obtener el primer elemento de una lista que no tiene ningún elemento). Con eso nos alcanza de momento, más adelante incorporaremos más herramientas, pero sobre todo vamos a **formar criterio** sobre cómo usarlas.

El código de la clase (incluyendo también algunas cosas que quedaron a medio implementar) lo pueden encontrar [acá](https://github.com/pdep-mit/ejemplos-de-clase-wollok/tree/master/ejemplos-de-clase/src/clase04).

## Para profundizar y ejercitar

- De la [sección de apuntes](http://www.pdep.com.ar/material/apuntes): el módulo 4 explica qué son y cómo se usan los bloques y las colecciones (sets y listas) en Wollok.
- De [Mumuki](https://wollok.mumuki.io/chapters/31-programacion-con-objetos): las lecciones 6, 7 y 8 cubren estos temas. Además con esto se desbloquea el resto de la lección de clases e instancias :)

[< Clase anterior](https://github.com/pdep-mit/bitacora-de-clase/blob/master/clase-19.md) - [Clase siguiente >](https://github.com/pdep-mit/bitacora-de-clase/blob/master/clase-21.md)
