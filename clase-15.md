# Listas y Agregación

En esta clase cerramos los temas del paradigma lógico viendo cómo se trabaja con otro tipo de [individuo compuesto](http://wiki.uqbar.org/wiki/articles/paradigma-logico---individuos-compuestos.html) que son las [listas](http://wiki.uqbar.org/wiki/articles/paradigma-logico---listas.html).

Vimos cómo se puede hacer para trabajar con listas [recursivamente](http://wiki.uqbar.org/wiki/articles/recursividad-en-logico.html) usando pattern matching y recursividad, y también los principales predicados que ya vienen para trabajar con listas más cómodamente:
- length/2
- sum_list/2
- member/2
- nth0/3 y nth1/3

... y findall/3 que es un predicado de [orden superior](http://wiki.uqbar.org/wiki/articles/orden-superior.html).

Además, de la mano de recursividad, vimos cómo podemos jugar con las múltiples respuestas para ciertos problemas que englobamos bajo el título **Explosión Combinatoria**, para entender el poder que gana este paradigma al incorporar las listas como herramienta de modelado.

Importante! No olviden que la mayoría de los problemas ya los podíamos resolver sin listas, de forma declarativa. Para no caer en la tentación, les dejamos [Los Donny, no!](https://docs.google.com/presentation/d/e/2PACX-1vSKFGF0920302VpDPVrnRKez_O_wjgDg4_cssbsH3G4RBt7sTKEfl5KnUVchASdH4tnW9Hx8pGHUpdu/embed?start=false&loop=false&delayms=60000) para el uso responsable de findall.

Acá pueden encontrar el [código](https://github.com/pdep-mit/ejemplos-de-clase-prolog/blob/master/clase5.pl) de esta clase y la clase en vivo de la cursada 2020: [Tipos compuestos (parte 2)](https://www.youtube.com/watch?v=0Fb6QZXG-5c).

De la [sección de apuntes](http://www.pdep.com.ar/material/apuntes):
  - En el **Módulo 3** sobre individuos compuestos **se explica listas** más en profundidad de lo que llegamos a ver, incluyendo otros predicados para trabajar con listas sencillos pero menos cotidianos.
  - En el **Módulo 4** sobre predicados de orden superior se explica el predicado **findall/3**.
  - En el **Módulo 5** sobre **recursividad** se termina de explicar este tema para cuando las otras herramientas se quedan cortas.
  - En el **Módulo 6**, en la sección de **Code Smells**, pueden encontrar una versión extendida con ejemplos concretos de los **Donny, no!**.
  - En el **Módulo 7**, sobre **Explosión Combinatoria**.

Finalmente, pueden encontrar contenido adicional muy interesante en el **Módulo 7** que no se evalúa pero puede parecerles interesante: cómo hacer predicados de orden superior y predicados dinámicos (para lo cual aparece la necesidad de incorporar efecto colateral).

[< Clase anterior](https://github.com/pdep-mit/bitacora-de-clase/blob/master/clase-14.md) - [Clase siguiente >](https://github.com/pdep-mit/bitacora-de-clase/blob/master/clase-16.md)
