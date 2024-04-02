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
  - Tipos de datos básicos (números, booleanos, strings, ...).
  - Entender de qué tipo son las funciones, en base al tipo de su dominio y de su imagen.
  - Más adelante vamos a ampliar mucho más este tema y agregar más tipos de datos.
- [Pattern Matching con tipos básicos](http://wiki.uqbar.org/wiki/articles/pattern-matching-en-haskell.html)
- [Funciones por Partes o Guardas](http://wiki.uqbar.org/wiki/articles/funciones-por-partes.html)
- [Intro a Recursividad (sin listas)](http://wiki.uqbar.org/wiki/articles/recursividad-en-haskell.html)
  
Acá pueden encontrar el [código de la clase](https://github.com/pdep-mit/ejemplos-de-clase-haskell/blob/master/src/Clase1.hs) y videos de clase donde explicamos estos temas en 2020 / 2021:
- [Intro a Funcional con Haskell](https://www.youtube.com/watch?v=SOOytHnqkug&list=PL2xYJ49ov_dc1hCGcRMvu8VU3jexRUjf3)
- [Intro a Funcional, primeros ejemplos](https://www.youtube.com/watch?v=wtODGk8J0Ng&list=PL2xYJ49ov_dc1hCGcRMvu8VU3jexRUjf3)
- [Intro a Pattern Matching y Guardas](https://www.youtube.com/watch?v=TIo7c4hWZi0&list=PL2xYJ49ov_dc1hCGcRMvu8VU3jexRUjf3)

> :warning: En esta cursada estamos la biblioteca [PdePreludat](https://github.com/10Pines/pdepreludat/blob/master/README.md) que apunta a mejorar la experiencia de aprendizaje. Por ese motivo, en vez de usar tipos de datos nativos para los números como son Int, Float, Double... usaremos para todo el tipo Number provisto por esta biblioteca.
> Tené en cuenta que los videos disponibles fueron grabados usando Haskell sin esta biblioteca, por lo que aparecerán los tipos numéricos nativos de Haskell.

Los temas de esta clase están cubiertos en la [sección de apuntes](http://www.pdep.com.ar/material/apuntes) por:
- Módulo 1 de funcional

[< Clase anterior](https://github.com/pdep-mit/bitacora-de-clase/blob/master/clase-01.md) - [Clase siguiente >](https://github.com/pdep-mit/bitacora-de-clase/blob/master/clase-03.md)
