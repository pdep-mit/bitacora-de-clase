# Orden superior + Tipos de datos compuestos (Parte 2): Listas

## Temas de la clase

En esta clase vimos uno de los conceptos más fuertes de la materia, sobre el cual vamos a volver una y otra vez a lo largo del año, que es [Orden Superior](http://wiki.uqbar.org/wiki/articles/orden-superior.html). Videíto introductorio que armamos con Alf: [Creando Abstracciones: Introducción a Orden Superior](https://www.youtube.com/watch?v=mSJdiZ-0pXk&list=PL2xYJ49ov_dc1hCGcRMvu8VU3jexRUjf3&index=6)

En particular hicimos foco en esta idea esta idea para trabajar con [listas](http://wiki.uqbar.org/wiki/articles/tipos-de-haskell.html), porque si bien se puede hacer todo con pattern matching y recursividad, podemos llegar a soluciones mucho mejores evitando esta mecánica.

Es importante entender que orden superior puede aplicarse en cualquier contexto, por ejemplo la composición no es más que una función de orden superior super genérica y sencilla!

```Haskell
(.) :: (b -> c) -> (a -> b) -> (a -> c)
(.) g f x = g (f x)
```

Además hablamos sobre [expresiones lambda](http://wiki.uqbar.org/wiki/articles/expresiones-lambda.html) y [currificación](http://wiki.uqbar.org/wiki/articles/currificacion.html).

Ahora que incorporamos el uso y definición de funciones de orden superior a nuestras herramientas para trabajar, vamos a poder armar [abstracciones](http://wiki.uqbar.org/wiki/articles/abstraccion.html) todavía más poderosas, pudiendo parametrizar parte de la lógica a ejecutar. En los lenguajes funcionales esto normalmente es sencillo, gracias a que las funciones son [ciudadanos de primera clase](https://en.wikipedia.org/wiki/First-class_citizen) (recordarán que varias veces les dijimos que las funciones son valores).

Entre las funciones de orden superior para trabajar con listas que vimos en esta clase están:
- `map :: (a -> b) -> [a] -> [b]`
- `filter :: (a -> Bool) -> [a] -> [a]`
- `all :: (a -> Bool) -> [a] -> Bool`
- `any :: (a -> Bool) -> [a] -> Bool`
- y las distintas variantes de [fold](http://wiki.uqbar.org/wiki/articles/fold.html).

Si bien vimos cómo se pueden definir algunas de estas funciones y otras para trabajar con listas usando recursividad, al trabajar con listas debemos recordar lo que hablamos la primer clase sobre [declaratividad](http://wiki.uqbar.org/wiki/articles/declaratividad.html). En general, para trabajar con listas, vamos a preferir siempre las soluciones que usen 1 o más funciones de orden superior adecuadas para el problema a resolver por sobre soluciones recursivas, ya que las primeras son más declarativas que las segundas.

Con esto no queremos decir que nunca vayan a usar recursividad:
- La recursividad es una gran herramienta cuando el problema tiene naturaleza recursiva (como el ejemplo del factorial que vimos en la primer clase de funcional), en cuyo caso la solución a la que lleguemos recursivamente a priori no va a ser criticable en términos de declaratividad.
- La recursividad trabajando con listas a veces simplemente es necesaria, porque el problema no se ajusta bien al algoritmo de recorrido estándar que viene resuelto con las funciones de orden superior que ya existen.

Pueden encontrar el código que hicimos en clase [acá](https://github.com/pdep-mit/ejemplos-de-clase-haskell/blob/master/src/Clase4.hs) y los video de clase de la cursada 2020:
- [Orden Superior](https://www.youtube.com/watch?v=Gl22i9u-keM&list=PL2xYJ49ov_dc1hCGcRMvu8VU3jexRUjf3)
- [Listas](https://www.youtube.com/watch?v=7fbSKZdQ5c8&list=PL2xYJ49ov_dc1hCGcRMvu8VU3jexRUjf3)

Luego de esta clase ya casi vimos todos los temas de este paradigma, nos falta revelar un par de misterios más que tenemos bajo la manga. Pero lo que falta sobre todo es práctica, mucha, para terminar de dominar las herramientas así como incorporar algunas nociones más de diseño.

De la [sección de apuntes](http://www.pdep.com.ar/material/apuntes): Módulos 5 y 6 de funcional.

[< Clase anterior](https://github.com/pdep-mit/bitacora-de-clase/blob/master/clase-06.md) - [Clase siguiente >](https://github.com/pdep-mit/bitacora-de-clase/blob/master/clase-08.md)
