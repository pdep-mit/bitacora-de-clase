# Modelado con funciones

En esta clase resolvimos el ejercicio [Gravity Falls - Las Rarezas](https://docs.google.com/document/d/1ivhqJIWGanstr324ElRY6lev0b0UN-QN3kcYFH9wqMs/edit#heading=h.slln8607g6w) con el objetivo de pensar formas alternativas de modelar las abstracciones de nuestro dominio. Sabiendo que las funciones son valores, ¿qué nos impide usarlas para modelar los datos y no sólo las operaciones?

Algo que tenemos que tener en cuenta es que las funciones no son mostrables por consola (Show) ni son comparables por igualdad (Eq), lo cual complica un poco algunas cosas, sobre todo cuando queremos saber si nuestro programa está funcionando... Pero vimos cómo podemos solventar uno de esos problemas sin mucho esfuerzo importando el módulo `Text.Show.Functions`, que hace que por lo menos podamos seguir usando el `deriving Show` para nuestros datas.

Hay otras formas un poquito más complejas de encarar estos problemas, definiendo nuestras propias implementaciones para las funciones `show` e `(==)` para nuestros tipos de dato en vez de usar deriving, pero para lo que necesitamos hacer no hace falta.

Pueden encontrar el código de la clase [acá](https://github.com/pdep-mit/ejemplos-de-clase-haskell/blob/master/clase7.hs).

## Para profundizar y ejercitar
- De la [sección de apuntes](http://www.pdep.com.ar/material/apuntes): Módulo 3 de funcional
- De Mumuki, los últimos ejercicios de la guía de Modelado.

[< Clase anterior](https://github.com/pdep-mit/bitacora-de-clase/blob/master/clase-07.md) - [Clase siguiente >](https://github.com/pdep-mit/bitacora-de-clase/blob/master/clase-09.md)
