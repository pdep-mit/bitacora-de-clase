# Introducción a Funcional

## Temas de la clase

En esta clase arrancamos con el [paradigma funcional](http://wiki.uqbar.org/wiki/articles/paradigma-funcional.html), 
para el cual usaremos el lenguaje [Haskell](https://pdep.com.ar/software/software-haskell), 
y vimos los siguientes temas:
- [Concepto de función](http://wiki.uqbar.org/wiki/articles/concepto-de-funcion.html)
(principalmente desde el punto de vista de transformación matemática e imperativo)
  - Cumplen con unicidad y existencia, esto nos permite asegurar que luego de aplicar una función obtendremos siempre un único valor.
  - Tienen [transparencia referencial](http://wiki.uqbar.org/wiki/articles/transparencia-referencial--efecto-de-lado-y-asignacion-destructiva.html)
  - Las variables son incógnitas como las de matemática, no pensarlas como posiciones de memoria, no se pueden asignar.
  - Su principal operación: la [aplicación](http://wiki.uqbar.org/wiki/articles/aplicacion.html).
- Introducción a [tipado de Haskell](http://wiki.uqbar.org/wiki/articles/tipos-de-haskell.html):
  - Tipos de datos simples (Int, Float, Bool, ...)
  - Introducción a typeclasses (Num, Ord, Eq)
  - Entender de qué tipo son las funciones
- [Funciones por Partes (Guardas)](http://wiki.uqbar.org/wiki/articles/funciones-por-partes.html)

## Para profundizar y ejercitar

- De la [sección de apuntes](https://pdep.com.ar/material/apuntes): Módulo 1 de funcional
- De [Mumuki](https://mumuki.io/chapters/82-programacion-funcional):
  - Valores y Funciones (Ejercicios 1 al 9 inclusive)
  - Práctica Valores y Funciones (todavía no vimos composición, si les pide usar ese concepto, vale saltear el ejercicio y hacerlo luego). Ejercicios sugeridos de esta guía:
    - esCuadradoPerfecto
    - dispersion
