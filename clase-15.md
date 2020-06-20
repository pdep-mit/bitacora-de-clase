# Listas y Agregación

En esta clase cerramos los temas del paradigma lógico viendo cómo se trabaja con otro tipo de [individuo compuesto](http://wiki.uqbar.org/wiki/articles/paradigma-logico---individuos-compuestos.html) que son las [listas](http://wiki.uqbar.org/wiki/articles/paradigma-logico---listas.html).

Vimos cómo se puede hacer para trabajar con listas [recursivamente](http://wiki.uqbar.org/wiki/articles/recursividad-en-logico.html) usando pattern matching, y también los principales predicados que ya vienen para trabajar con listas más cómodamente:
- length/2
- sumlist/2
- member/2
- nth0/3 y nth1/3
- y findall/3 que es un predicado de [orden superior](http://wiki.uqbar.org/wiki/articles/orden-superior.html).

Importante! No olviden que la mayoría de los problemas ya los podíamos resolver sin listas, de forma declarativa. Para no caer en la tentación, les dejamos [Los Donny, no!](https://docs.google.com/presentation/d/e/2PACX-1vSKFGF0920302VpDPVrnRKez_O_wjgDg4_cssbsH3G4RBt7sTKEfl5KnUVchASdH4tnW9Hx8pGHUpdu/embed?start=false&loop=false&delayms=60000) para el uso responsable de findall.

Acá pueden encontrar el [código](https://github.com/pdep-mit/ejemplos-de-clase-prolog/blob/master/clase5.pl) de esta clase.

## Para profundizar y ejercitar

- De la [sección de apuntes](http://www.pdep.com.ar/material/apuntes):
  - En el **Módulo 3** sobre individuos compuestos **se explica listas** más en profundidad de lo que llegamos a ver, incluyendo otros predicados para trabajar con listas sencillos pero menos cotidianos.
  - En el **Módulo 4** sobre predicados de orden superior se explica el predicado **findall/3**.
  - En el **Módulo 5** sobre **recursividad** se termina de explicar este tema para cuando las otras herramientas se quedan cortas.
  - En el **Módulo 6**, en la sección de **Code Smells**, pueden encontrar una versión extendida con ejemplos concretos de los **Donny, no!**.
- De Mumuki pueden trabajar con todas las guías, ya que terminamos de ver todo el contenido teórico que teníamos planeado para este paradigma.

Finalmente, pueden encontrar contenido adicional muy interesante en el **Módulo 7** de la sección de apuntes. Esto no se evalúa, pero es muy recomendable para entender el poder que gana este paradigma al incorporar las listas como herramienta de modelado, cómo hacer predicados de orden superior, y algún que otro tema BONUS que no cubrimos en clase.

[< Clase anterior](https://github.com/pdep-mit/bitacora-de-clase/blob/master/clase-14.md) - [Clase siguiente >](https://github.com/pdep-mit/bitacora-de-clase/blob/master/clase-16.md)
