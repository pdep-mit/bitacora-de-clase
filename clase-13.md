# Ejercicio: Tales of Zestiria

En esta clase resolvimos el ejercicio: [Tales of Zestiria](https://docs.google.com/document/d/1TrcfZiwKriniMkeUQTxvgUVCbJla263jYux7o4jVbfw/edit#heading=h.k55i1crzbyp7) para repasar lo que estuvimos viendo hasta ahora.

Además aprovechamos el ejercicio para introducir [Aritmética en Prolog](http://wiki.uqbar.org/wiki/articles/aritmetica-en-prolog.html), porque tener relaciones en vez de funciones nos obliga a repensar algunas cosas que damos por obvias. En este ratito que le dedicamos a analizar las diferencias entre funciones y predicados recordamos que:
 - Los predicados no devuelven cosas, tienen valor de verdad. Tenemos que tener eso en cuenta para entender cuál es la aridad que tiene sentido que tengan los predicados que hacemos, y también para no usarlos pretendiendo que se comporten como funciones respecto al retorno.
 - Recordamos que la unicidad ya no es la norma, si queremos que se comporten de esa forma nuestros predicados, tenemos que asegurar que las cláusulas sean mutuamente excluyentes como parte de la lógica de los mismo.

Finalmente pusimos como caso de estudio el viejo y querido cálculo del factorial de un número, que como ya sabemos es un problema con naturaleza recursiva. Pueden ver una explicación de ese problema, así como otro caso típico de predicado recursivo que mencionamos en clase, en el artículo de [Recursividad en lógico (sin listas)](http://wiki.uqbar.org/wiki/articles/recursividad-en-logico.html).

Pueden encontrar el código de la clase [acá](https://github.com/pdep-mit/ejemplos-de-clase-prolog/blob/master/clase3.pl).

## Para profundizar y ejercitar

- De Mumuki pueden trabajar con la guía de Aritmética. Además la práctica de Inversibilidad ya la pueden hacer completa.

[< Clase anterior](https://github.com/pdep-mit/bitacora-de-clase/blob/master/clase-12.md) - [Clase siguiente >](https://github.com/pdep-mit/bitacora-de-clase/blob/master/clase-14.md)
