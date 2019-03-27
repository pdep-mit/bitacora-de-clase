# Tipos de datos compuestos (Parte 2): Listas, Recursividad vs. Orden Superior

## Temas de la clase

En esta clase vimos uno de los temas fuertes de la materia, sobre el cual vamos a volver una y otra vez a lo largo del año, que es [Orden Superior](http://wiki.uqbar.org/wiki/articles/orden-superior.html). En particular vimos esta idea para trabajar con listas, para poder dejar a un lado las soluciones recursivas que son menos declarativas. Sin embargo este concepto es mucho más grande, por ejemplo la composición no es más que una función de orden superior super genérica y sencilla!

```Haskell
(.) :: (b -> c) -> (a -> b) -> (a -> c)
(.) g f x = g (f x)
```

Entre las funciones de orden superior que vimos en esta clase están:
- `map :: (a -> b) -> [a] -> [b]`
- `filter :: (a -> Bool) -> [a] -> [a]`
- `all :: (a -> Bool) -> [a] -> Bool`
- `any :: (a -> Bool) -> [a] -> Bool`
- y las distintas variantes de [fold](http://wiki.uqbar.org/wiki/articles/fold.html)
que sirven para trabajar con [Listas](http://wiki.uqbar.org/wiki/articles/tipos-de-haskell.html), y vimos cómo se pueden definir estas funciones y otras para trabajar con listas usando [recursividad](http://wiki.uqbar.org/wiki/articles/recursividad-en-haskell.html).

Al trabajar con listas debemos recordar lo que hablamos la primer clase sobre [declaratividad](http://wiki.uqbar.org/wiki/articles/declaratividad.html). En general vamos a preferir siempre las soluciones que usen 1 o más funciones de orden superior adecuadas para el problema a resolver por sobre soluciones recursivas, ya que las primeras son más declarativas que las segundas.

Además aprovechamos para ver una forma más de definir funciones, que es particularmente útil para salir del paso ocasionalmente al trabajar con funciones de orden superior: [las expresiones lambda](http://wiki.uqbar.org/wiki/articles/expresiones-lambda.html).

Con esto ya casi que vimos todos los temas de este paradigma, nos falta terminar de formalizar algunas cosas de tipado y revelar un par de misterios más que tenemos bajo la manga. Pero lo que falta sobre todo es práctica, mucha, para terminar de dominar las herramientas así como incorporar algunas nociones más de diseño.

## Para profundizar y ejercitar

- De la [sección de apuntes](http://www.pdep.com.ar/material/apuntes): Módulos 5 y 6 de funcional.
- De Mumuki, con lo que vimos ya podrían hacer todas las guías, pero en particular estas guías sirven como práctica de los temas vistos en esta clase:
  - Práctica de Listas
  - Práctica Recursividad
  - Práctica de Aplicación Parcial y Orden Superior
  - Dominar el mundo con nada <- para practicar fold

[< Clase anterior](https://github.com/pdep-mit/bitacora-de-clase/blob/master/clase-05.md) - [Clase siguiente >](https://github.com/pdep-mit/bitacora-de-clase/blob/master/clase-07.md)
