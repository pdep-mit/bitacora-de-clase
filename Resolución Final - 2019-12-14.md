# Parte A

1- no hace falta usar listas para representar la información

```
productoBuscado(mati, mesa(circular, vidrio), 1).
productoBuscado(mati, silla(metal), 4).
productoBuscado(leo, sillon(cama, 2), 1).
productoBuscado(leo, sillon(reclinable, 1), 1).
```

Ejemplo de consulta para cumplir lo pedido:
```
?- productoBuscado(leo, Producto, _).
Producto = sillon(cama, 2);
Producto = sillon(reclinable, 1).
```

Como son relaciones, no funciones, podemos hacer consultas con múltiples respuestas.

2-

```
trabajaMaterial(Sucursal, Material):-
  stock(Sucursal, Producto, _),
  material(Producto, Material).

material(silla(Material), Material).
material(mesa(_, Material), Material).
material(sillon(_, _), madera).
```

Polimorfismo, el predicado material/2 es polimórfico y se aprovecha en la definición de trabajaMaterial/2

3-

```
sucursalIdeal(Sucursal, Cliente):-
  stock(Sucursal, _,_),
  productoBuscado(Cliente, _, _),
  forall(productoBuscado(Cliente, Producto, CantidadBuscada), (stock(Sucursal, Producto, CantidadEnStock), CantidadEnStock >= CantidadBuscada)).
```

Orden Superior

----------

# Parte B

Función dada:
```
funcion x y lista = (filter (> x) . map (\ f -> f y)) lista
```

1- Retorna los resultados de aplicar `y` a las funciones de la lista que sean mayores a `x`

(si bien no se pedía, inferimos el tipo de la función para practicar y ayudarnos a responder mejor al 1 y el 3)
- `funcion :: Ord a => a -> b -> [ b -> a ] -> [ a ]`

Propuesta de mejores nombres para la función y sus parámetros para que sea más expresiva:
`transformacionesMayoresA minimo valorATransformar transformaciones = ...`

Es discutible si renombrar el parámetro `f` de la lambda haría que sea más expresiva, porque `f` por convención está fuertemente asociado a la idea de función, pero también podría renombrarse.

2- Sí, puede terminar de evaluarse usando una lista infinita gracias a la Evaluación Perezosa (lazy), si ese resultado es acotado por algo más.

Ejemplo: `take 3 (funcion 10 20 (repeat id))`

--

Reemplazamos en el tipo que inferimos antes con el tipo de cada parámetro para identificar si el uso es válido y qué retorna:

a- `funcion 3 "hola" []`
`Int -> String -> [String -> Int] -> [Int]` --> es válida, retornaría `[Int]`

b- `funcion 3 7`
`Int -> Int -> [Int -> Int] -> [Int]` --> es válida, por aplicación parcial retornaría una función de tipo `[Int -> Int] -> [Int]`

c- `funcion "chau" "hola" [length]`
`String -> String -> [ String -> Int ] -> ???`  --> no es válida, no tipa, Int y String no son el mismo tipo

Por el mismo motivo que:
`4 > "chau"`  --> no tipa

El tipo de (>) es: `Ord a => a -> a -> Bool`

----------

# Parte C

1a. V, al trabajar con 3 colecciones distintas en Pedido no se están tratando de forma indistinta, por más que todas las prendas entiendan el mismo mensaje tiempo().

1b. F, no es coincidencia que todas se basen en el número 120. Si hubiera que cambiarlo en un lugar o agregar una falda de otro material, habría que asegurar que sea consistente con lo demás.

1c. F, con herencia simple no alcanza porque hay más de una clasificación, por lo tanto la combinatoria de tipo de prenda y material va a seguir llevando a repeticiones de lógica.

1d. V, el método tiempoDeConfeccion() es demasiado algorítmico, se podrían reemplazar las iteraciones con forEach incrementando una variable por el uso de sum (abstracción de más alto nivel que permite preocuparnos por qué quiero hacer, y no en cómo hacerlo).

Código propuesto que resuelve los problemas identificados:

```
class Prenda {
  const material
  method tiempo() = material.tiempoFinal(self.tiempoBase())
}

class Short inherits Prenda {
  method tiempoBase() = tiempoNecesario
}

class Falda inherits Prenda {
  method tiempoBase() = 120
}

class Blusa inherits Prenda {
  var cantBotones
  method tiempoBase() = 200 + cantBotones * 5
}

object modal {
  method tiempoFinal(tiempoBase) = tiempoBase
}

object lycra {
  method tiempoFinal(tiempoBase) = tiempoBase * 1.2
}

object denim {
  method tiempoFinal(tiempoBase) = tiempoBase + 25
}

class Pedido {
  var prendas = []
  method tiempoDeConfeccion() {
    return prendas.sum({prenda => prenda.tiempo()})
  }
}
```