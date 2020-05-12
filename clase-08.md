# Modelado con funciones

En esta clase resolvimos el ejercicio de parcial [Lambda Prop](https://docs.google.com/document/d/1Gc-ot4AStIaGePl-q2V1KJBhpiXL0ye6pWvLki4vWZg/edit) con el objetivo de pensar formas alternativas de modelar las abstracciones de nuestro dominio. Sabiendo que las funciones son valores, ¿qué nos impide usarlas para modelar los datos y no sólo las operaciones?

Algo que tenemos que tener en cuenta es que las funciones no son mostrables por consola (Show) ni son comparables por igualdad (Eq), lo cual complica un poco algunas cosas, sobre todo cuando queremos saber si nuestro programa está funcionando... Pero vimos cómo podemos solventar uno de esos problemas sin mucho esfuerzo importando el módulo `Text.Show.Functions`, que hace que por lo menos podamos seguir usando el `deriving Show` para nuestros datas.

Hay otras formas un poquito más complejas de encarar estos problemas, definiendo [nuestras propias implementaciones](http://wiki.uqbar.org/wiki/articles/data--definiendo-nuestros-tipos-en-haskell.html#tocAnchor-1-6) para las funciones `show` e `(==)` para nuestros tipos de dato en vez de usar deriving, pero para lo que necesitamos hacer normalmente no hace falta.

Pueden encontrar el código de la clase [acá](https://github.com/pdep-mit/ejemplos-de-clase-haskell/blob/master/src/Clase5.hs).

## Para profundizar y ejercitar
- De la [sección de apuntes](http://www.pdep.com.ar/material/apuntes): Módulo 3 de funcional
- De Mumuki, los últimos ejercicios de la guía de Modelado.

[< Clase anterior](https://github.com/pdep-mit/bitacora-de-clase/blob/master/clase-07.md) - [Clase siguiente >](https://github.com/pdep-mit/bitacora-de-clase/blob/master/clase-09.md)
