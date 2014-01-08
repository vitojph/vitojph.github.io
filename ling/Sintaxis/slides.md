n   # Sintaxis

## Introducción a la Lingüística.

Área de Lingüística, Fac. de Filología, UCM | 19/12/2013

Víctor Peinado | v.peinado@filol.ucm.es

--SLIDE--

# Gramática Generativa

--SLIDE--

### ¿Qué es la sintaxis?

- En las últimas clases, repasamos las categorías gramaticales generales empleadas para describir la estructura de sintagmas
y oraciones.

- Cuando estudiamos la estructura y la combinación de los componentes de la oración, estamos estudiando la **sintaxis**.

- Hemos visto cómo la sintaxis trata de producir un análisis preciso de una secuencia de elementos de la oración, o el análisis de una combinación ordenada de elementos.

- A continuación vamos a ver algunos estudios que plantean nuevos enfoques que den cuenta de las combinaciones en la estructura de las oraciones.


--SUBSLIDE--

### La Gramática Generativa

- El lingüista estadounidense Noam Chomsky, a partir de los años 1950s, propuso dar un enfoque matemático a la descripción gramatical: la **gramática generativa**.

    Consideraré que el lenguaje es un conjunto (finito o infinito) de oraciones.

- La gramática generativa está formada por un conjunto explícito de reglas que especifican qué combinaciones de elementos básicos conforman las oraciones bien formadas de una lengua.

--SUBSLIDE--

- En la expresión algebraica *3x + 2y* podemos asignar a las variables *x* e *y* diferentes valores.

- A partir de esa sencilla expresión, asignando distintos valores, podemos *a priori* generar un nuevo conjunto infinito de
resultados.

- Si el conjunto de todas las oraciones bien formadas de una lengua conforma un conjunto comparable, entonces debe de
exisitir un conjunto de reglas explícitas, que produzcan estas oraciones.

- Este conjunto de reglas explícitas se conoce con el nombre de **gramatica generativa**.


--SLIDE--

### Propiedades de la gramática generativa

1. La gramática deberá generar **todas** las estructuras sintácticas bien formadas de la lengua, y **solo** las que están bien formadas.

2. La gramática deberá tener un **número finito de reglas** que deberán ser capaces de generar un **número infinito de oraciones** bien formadas &rarr; **productividad del lenguaje**.

3. Las reglas de la gramática deberán cumplir la propiedad de la **recursión** y permitir ser aplicadas más de una vez al generar una estructura.

4. La gramática deberá ser capaz de mostrar tanto la **estructura superficial** como la **estructura profunda**.


--SUBSLIDE--

### Recursión

- La recursión es la propiedad de definir algo en términos de sí mismo.

- Sea cual sea la regla que genera el componente *que cazó el gato* en la oración *Ese es el perro que cazó el gato*, la gramática generativa deberá permitir aplicar dicha regla de nuevo para generar cualquier estructura similar a *Ese es el perro que cazó el gato que se comió el ratón*.

- La gramática generativa deverá considerar la posibilidad de que una oración pueda contener otra oración dentro de ella, o de que un sintagma determinado pueda estar formado por otro sintagma.

- Esta caracteristica es la que nos permite, a partir de un número finito de reglas, un número (potencialmente) infinito de oraciones válidas.

    Para entender a recursividad, primero hay que entender la recursividad.

--SLIDE--

### Estructura superficial y estructura profunda

- La gramática deberá dar cuenta de cómo dos oraciones superficialmente distintas pueden estar estrechamente relacionadas.

- En inglés, las oraciones *John fed the dog* y *The dog was fed by John* son dos oraciones superficialmente distintas. 

    - Según la gramática tradicional, la primera es una oración activa y la segunda es pasiva.
    
    - Difieren en su **estructura superficial** en en la forma sintáctica en la que se realizan.
    
- Sin embargo, ambas oraciones están estrechamente relacionadas y pueden considerarse idénticas si atendemos a su **estructura profunda**.

    - La estructura profunda es un nivel abstracto de organización en el que representamos todos los elementos de la interpretación estructural.

--SLIDE--

### Ambigüedad estructural

- La gramática deberá dar cuenta también de cómo dos oraciones superficialmente parecidas son, en realidad, diferentes.

- Pensemos en dos oraciones con estructuras profundas distintas:

    - *Ana tenía un paraguas y, con él, golpeó a un hombre*.
    - *Ana golpeó a n hombre, y el hombre tenía un paraguas*.
    
- Estos dos hechos diferentes pueden expresase con la misma estructura superficial: *Ana golpeó a un hombre con un paraguas*. 

- Esta oración es **estructuralmente ambigua**.

--SUBSLIDE--

- Los sintagmas también pueden ser estructuralmente ambiguos.

- *hombres y mujeres mayores* puede interpretarse como *hombres mayores y mujeres mayores* u *hombres, de cualquier edad, y mujeres mayores*.

--SLIDE--

# Formalización de gramáticas

--SLIDE--

### Símbolos utilizados en la descripción sintáctica

- Ya hemos visto en clases anteriores los nombres o etiquetas de las categorías sintácticas tales como oración (O/S), sintagma nominal (SN/NP), sintagma verbal (SV/VP), determinante (Det/DT), verbo (V/VB), etc.

- Las reglas generarivas se componen de dos partes:

    - una **parte izquierda**, situada antes de la flecha, en la que indicamos qué elemento estructural queremos definir.
     
    - una **parte derecha**, situada después de la flecha, en la que indicamos la definición del elemento estructural que aparece en la parte izquierda.

- La **flecha &rarr;** que divide las partes izquierdas y derechas de la regla se interpreta como *consta de*, *es esquivalente a* o *se reescribe como*. 

--SUBSLIDE--

- La regla generativa:

    SN &rarr; Det N
    
- se interpreta como *un sintagma nominal consta de un determinante y un nombre*

- Cualquier cosa encerrada entre paréntesis se entenderá como un componente opcional.

- Podemos completar la regla anterior diciendo que un SN consta obligatoriamente de un determinante y un nombre y, que opcionalmente, puede contener un adjetivo:

    SN &rarr; Det N (Adj)
	
--SUBSLIDE--

- Las **llaves {}** indican un conjunto de opciones posibles, de las que solo se puede elegir una.

- Por ejemplo, en español, un SN puede presentar varias estructuras distintas.

    - un determinante y un nombre
    
        SN &rarr; Det N (Adj)

    - un pronombre
    
        SN &rarr; Pro

    - un nombre propio
    
        SN &rarr; NP

- Estas tres opciones pueden formalizarse en una única regla.

    SN &rarr; {Det N (Adj), Pro, NP}

--SUBSLIDE--

--SUBSLIDE--

O: oración
Pro: pronombre
V: verbo
Det: determinante
Prep: preposición
SV: sintagma verbal
Conj: conjunción
N: nombre
NP: nombre propio
Adj: adjetivo
Adv: adverbio
SN: sintagma nominal
SP: sintagma preposicional

*: secuencia agramatical
&rarr;: consta de
(): consituyente opcional
{}: opciones disponibles, solo uno puede ser seleccionado

--SUBSLIDE--

# Tipos de reglas

--SLIDE--

### Otros enfoques de la gramática generativa

- 60 años después, la Gramática generativa sigue causando discusiones y excepticismo.

- Para algunos lingüistas, las únicas cuestiones relevsantes que debería cubir una gramática son de tipo sintáctico: es decir, cómo describir la estructura independientemente del significado.

- Para otros, el significado es un componente básico, hasta el punto de que abandonan la idea de estructura profunda en favor de una representación semántica.




### Referencias

- Hudson, G. *Introductory Linguistics*. Blackwell. 2006.
- O'Grady, W., Dobrovolsky, M., Katmaba, F. *Contemporary Linguistics. An Introduction*. Addison Wesley Longman. 1998.
- O'Grady, W., Archivald, J., Aronoff, M., Rees-Miller, J. *Contemporary Linguistics. An Introduction (5th Edition)*. Bedford/St. Martin's. 2005.
- Yule, G. *The Study of Language (4th Edition)*. Cambridge University Press. 2010.



