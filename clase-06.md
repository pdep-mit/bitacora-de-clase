# Orden Superior

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

Además aprovechamos para ver una forma más de definir funciones, que es particularmente útil para salir del paso ocasionalmente al trabajar con funciones de orden superior: [las expresiones lambda](http://wiki.uqbar.org/wiki/articles/expresiones-lambda.html).

El código de la clase lo puede encontrar [acá](https://github.com/pdep-mit/ejemplos-de-clase-haskell/blob/master/clase4.hs).

Con esto ya casi que vimos todos los temas de este paradigma, nos falta terminar de formalizar algunas cosas de tipado y revelar un par de misterios más que tenemos bajo la manga. Pero lo que falta sobre todo es práctica, mucha, para terminar de dominar las herramientas así como incorporar algunas nociones más de diseño.

## Desafío café con leche!

Basándonos en el ejercicio [intercalar de la guía de Recursividad](https://mumuki.io/exercises/1914-programacion-funcional-practica-recursividad-intercalar), el desafío es resolver el problema sólo con un llamado a fold (la variante que consideren más apropiada). Alcanza con que funcione para listas de al menos un elemento. La primer persona que me mande una solución que cumpla con estas pautas a [mi mail](mailto:mmatos87@gmail.com), se gana un café con leche para la próxima clase.

## Para profundizar y ejercitar

- De la [sección de apuntes](http://www.pdep.com.ar/material/apuntes): Módulos 5 y 6 de funcional.
- De [Mumuki](https://mumuki.io/chapters/82-programacion-funcional), con lo que vimos ya podrían hacer todas las guías, pero en particular los siguientes son los ejercicios propuestos para la clase que viene:
  - De la práctica de Aplicación Parcial y Orden Superior: pam
  - De la práctica de Listas: iniciales

[< Clase anterior](https://github.com/pdep-mit/bitacora-de-clase/blob/master/clase-05.md) - [Clase siguiente >](https://github.com/pdep-mit/bitacora-de-clase/blob/master/clase-07.md)
