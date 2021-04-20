# Introducción a Funcional

## Temas de la clase

En esta clase arrancamos con el [paradigma funcional](http://wiki.uqbar.org/wiki/articles/paradigma-funcional.html),
para el cual usaremos el lenguaje [Haskell](https://www.pdep.com.ar/software/haskell),
y vimos los siguientes temas:
- [Concepto de función](http://wiki.uqbar.org/wiki/articles/concepto-de-funcion.html)
  - Cumplen con unicidad y existencia, esto nos permite asegurar que luego de aplicar una función obtendremos siempre un único valor.
  - Tienen [transparencia referencial](http://wiki.uqbar.org/wiki/articles/transparencia-referencial--efecto-de-lado-y-asignacion-destructiva.html)
  - Las variables son incógnitas como las de matemática, no pensarlas como posiciones de memoria, no se pueden asignar.
  - Su principal operación: la [aplicación](http://wiki.uqbar.org/wiki/articles/aplicacion.html).
- Introducción a [tipado de Haskell](http://wiki.uqbar.org/wiki/articles/tipos-de-haskell.html):
  - Tipos de datos simples (Int, Float, Bool, ...).
  - Entender de qué tipo son las funciones, en base al tipo de su dominio y de su imagen.
  - Más adelante vamos a ampliar mucho más este tema y agregar más tipos de datos.
- [Pattern Matching con tipos básicos](http://wiki.uqbar.org/wiki/articles/pattern-matching-en-haskell.html)
- [Funciones por Partes o Guardas](http://wiki.uqbar.org/wiki/articles/funciones-por-partes.html)
- [Intro a Recursividad (sin listas)](http://wiki.uqbar.org/wiki/articles/recursividad-en-haskell.html)
  
Acá pueden encontrar el [código de la clase](https://github.com/pdep-mit/ejemplos-de-clase-haskell/blob/master/src/Clase1.hs) y videos de clase donde explicamos estos temas:
- [Clase 2.1 - Intro a Funcional con Haskell](https://www.youtube.com/watch?v=SOOytHnqkug&list=PL2xYJ49ov_dc1hCGcRMvu8VU3jexRUjf3)
- [Clase 2.2 - Intro a Funcional, primeros ejemplos](https://www.youtube.com/watch?v=wtODGk8J0Ng&list=PL2xYJ49ov_dc1hCGcRMvu8VU3jexRUjf3)
- [Clase 2.3 - Intro a Pattern Matching y Guardas](https://www.youtube.com/watch?v=TIo7c4hWZi0&list=PL2xYJ49ov_dc1hCGcRMvu8VU3jexRUjf3)

## Para profundizar y ejercitar

- De la [sección de apuntes](http://www.pdep.com.ar/material/apuntes): Módulo 1 de funcional
- De Mumuki (Capítulo de Programación Funcional), las guías:
  - Valores y Funciones (Ejercicios 1 al 9 inclusive).
  - Práctica Valores y Funciones (todavía no vimos composición, si les pide usar ese concepto, vale saltear el ejercicio y hacerlo luego).
  - Alternativas: Guardas y Patrones (hasta ejercicio 9 inclusive).

[< Clase anterior](https://github.com/pdep-mit/bitacora-de-clase/blob/master/clase-01.md) - [Clase siguiente >](https://github.com/pdep-mit/bitacora-de-clase/blob/master/clase-03.md)
