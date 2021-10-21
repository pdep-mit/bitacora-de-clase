# Práctica: Yaaar!

En esta clase hicimos la primer práctica grande, pensando mucho en las responsabilidades de los distintos objetos.

Pueden encontrar el enunciado acá: [Yaaar!](https://docs.google.com/document/d/1W7d0K3ZsYQyUVb7eis-2IXO8gmaBwJwf892oDZkPpEg/edit#).

El código al que llegamos al final de la clase está [acá](https://github.com/pdep-mit/ejemplos-de-clase-wollok/tree/master/src/clase06) (versiones 2020 y 2021), junto con un diagrama general armado para la clase de 2020. Ambas soluciones tienen decisiones similares para la mayoría de los puntos, la mayor diferencia a nivel modelo está en el punto 3 en caso de que sirva para comparar.

## Disclaimer: Igualdad de ítems - solución 2020

Los items podían ser strings directamente en vez de usar una clase `Item` que no suma nada y agrega complejidad. Si tuvieran algún comportamiento extra ok, pero en este ejercicio no lo tenían.

Habría que tener en cuenta que dos ítems distintos con el mismo nombre se consideren iguales, para eso hace falta [redefinir la igualdad](http://wiki.uqbar.org/wiki/articles/igual-o-identico-----vs---.html) (definida en Object), así logramos que esto de true:

```wollok
new Item(nombre = "mapa") == new Item(nombre = "mapa")
```

De esta forma se puede redefinir la igualdad para los ítems:

```wollok
 class Item {
 	const property nombre
 	
 	override method ==(otroItem) = nombre == otroItem.nombre()
 }
```

## Para profundizar 

- De la [sección de apuntes](http://www.pdep.com.ar/material/apuntes) ver el Módulo 14: Mutabilidad. Igualdad e identidad. 

[< Clase anterior](https://github.com/pdep-mit/bitacora-de-clase/blob/master/clase-22.md) - [Clase siguiente >](https://github.com/pdep-mit/bitacora-de-clase/blob/master/clase-23.md)
