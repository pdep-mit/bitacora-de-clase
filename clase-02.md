# Introducción a Funcional

## Temas de la clase

En esta clase arrancamos con el [paradigma funcional](http://wiki.uqbar.org/wiki/articles/paradigma-funcional.html), 
para el cual usaremos el lenguaje [Haskell](https://pdep.com.ar/software/software-haskell), 
y vimos los siguientes temas:
- [Concepto de función](http://wiki.uqbar.org/wiki/articles/concepto-de-funcion.html)
  - Cumplen con unicidad y existencia, esto nos permite asegurar que luego de aplicar una función obtendremos siempre un único valor.
  - Tienen [transparencia referencial](http://wiki.uqbar.org/wiki/articles/transparencia-referencial--efecto-de-lado-y-asignacion-destructiva.html)
  - Las variables son incógnitas como las de matemática, no pensarlas como posiciones de memoria, no se pueden asignar.
  - Su principal operación: la [aplicación](http://wiki.uqbar.org/wiki/articles/aplicacion.html).
- Introducción a [tipado de Haskell](http://wiki.uqbar.org/wiki/articles/tipos-de-haskell.html):
  - Tipos de datos simples (Int, Float, Bool, ...)
  - Introducción a typeclasses (Num, Ord, Eq). No son tipos, sino familias de tipos, que determinan qué conjuntos de operaciones deben poder hacerse para formar parte de esa familia. Ejemplo, tanto Int como Float son Num (pueden sumarse), Ord (pueden compararse por menor y mayor) y Eq (pueden compararse por igualdad), mientras que los Char no son Num, pero sí Ord y Eq.
  - Entender de qué tipo son las funciones, en base al tipo de su dominio y de su imagen.
- [Funciones por Partes (Guardas)](http://wiki.uqbar.org/wiki/articles/funciones-por-partes.html)

Pueden encontrar el código de esta clase [acá](https://github.com/pdep-mit/ejemplos-de-clase-haskell/blob/master/clase1.hs)

## Para profundizar y ejercitar

- De la [sección de apuntes](https://pdep.com.ar/material/apuntes): Módulo 1 de funcional
- De [Mumuki](https://mumuki.io/chapters/82-programacion-funcional):
  - Valores y Funciones (Ejercicios 1 al 9 inclusive)
  - Práctica Valores y Funciones (todavía no vimos composición, si les pide usar ese concepto, vale saltear el ejercicio y hacerlo luego). Ejercicios sugeridos de esta guía:
    - esCuadradoPerfecto
    - dispersion
