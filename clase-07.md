# Modelado con funciones

En esta clase resolvimos el ejercicio [Minigolfito](https://github.com/pdep-mit/ejemplos-de-clase-haskell/tree/master/clase5) con el objetivo de pensar formas alternativas de modelar las abstracciones de nuestro dominio. Sabiendo que las funciones son valores, ¿qué nos impide usarlas para modelar los datos y no sólo las operaciones?

Algo que tenemos que tener en cuenta es que las funciones no son mostrables por consola (Show) ni son comparables por igualdad (Eq), lo cual complica un poco algunas cosas, sobre todo cuando queremos saber si nuestro programa está funcionando... Pero vimos cómo podemos solventar esos problemas, siendo una estrategia válida definir instancias de las clases Show y Eq para nuestros datas sin tener que depender exclusivamente de que los componentes puedan mostrarse y compararse.

[< Clase anterior](https://github.com/pdep-mit/bitacora-de-clase/blob/master/clase-06.md)
