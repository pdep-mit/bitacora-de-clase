# Inversibilidad y Negación

En esta clase hicimos foco en uno de los conceptos fundamentales del paradigma lógico: [**Inversibilidad**](http://wiki.uqbar.org/wiki/articles/paradigma-logico---inversibilidad.html), e introdujimos el primer predicado de [orden superior](http://wiki.uqbar.org/wiki/articles/orden-superior.html) que estaremos usando en Prolog: [not/1](http://wiki.uqbar.org/wiki/articles/paradigma-logico---negacion.html) para la negación.

Además aprovechamos el ejercicio para introducir [Aritmética en Prolog](http://wiki.uqbar.org/wiki/articles/aritmetica-en-prolog.html) con el predicado `is/2`, porque tener relaciones en vez de funciones nos obliga a repensar algunas cosas que damos por obvias. En este ratito que le dedicamos a analizar las diferencias entre funciones y predicados recordamos que los predicados no devuelven cosas, tienen valor de verdad. Tenemos que tener eso en cuenta para entender cuál es la aridad que tiene sentido que tengan los predicados que hacemos, y también para no usarlos pretendiendo que se comporten como funciones.

También vimos que ambos predicados tienen [problemas de inversibilidad](http://wiki.uqbar.org/wiki/articles/paradigma-logico---casos-de-no-inversibilidad.html), con lo cual hay que tomar ciertos recaudos al usarlos para que nuestros predicados sean inversibles.

Pueden encontrar el código de esta clase [acá](https://github.com/pdep-mit/ejemplos-de-clase-prolog/blob/master/clase2.pl)

## Para profundizar y ejercitar

- De la [sección de apuntes](http://www.pdep.com.ar/material/apuntes):
    - Módulo 3 de Lógico - **Individuos Simples** (después se abordan temas que no vimos todavía)
    - Módulo 4 de Lógico - **Predicado not/2** (después se abordan temas que no vimos todavía)
- De Mumuki pueden trabajar con las guías de aritmética, negación e inversibilidad, a sabiendas de que algunos ejercicios abarcan los temas de la próxima clase.

[< Clase anterior](https://github.com/pdep-mit/bitacora-de-clase/blob/master/clase-11.md) - [Clase siguiente >](https://github.com/pdep-mit/bitacora-de-clase/blob/master/clase-13.md)
