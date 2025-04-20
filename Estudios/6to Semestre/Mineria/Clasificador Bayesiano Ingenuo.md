
El clasificador bayesiano ingenuo o simple(NBC: Naive Bayesian Classifier) es un tipo de [[Clasificador Bayesiano]]. Se basa en el supuesto de que **todos los atributos son independientes dada la variable de clase**:

- Es decir, cada atributo **Ai** es condicionalmente independiente de todos los demás atributos dada la clase:
- $P(A_i|A_j,C) = P(A_i|C), para todo j = i$

Bajo este supuesto la ecuación (1) puede escribirse como:
$$P(C|A_1, A_2, ..., A_n) = \frac{P(C)P(A_1|C)P(A_2|C)...P(A_n|C)} {P(A)}$$
Aprender un clasificador bayesiano ingenuo consiste en estimar la probabilidad previa de la clase, $P(C)$, y la tabla de probabilidad condicional (CPT) de cada atributo dada la clase, $P(A_i|C)$.

Estas pueden obtenerse mediante estimaciones subjetivas de un experto o a partir de los datos por máxima verosimilitud.

Las probabilidades pueden estimarse a partir de los datos mediante, por ejemplo, la estimación de máxima verosimilitud. Las probabilidades previas de la variable de clase, C, se dan por:

$$P(C_i) \frac{N_i}{N}$$

donde $N_i$ es el número de veces que $c_i$ aparece en las N muestras.

Las probabilidades condicionales de cada atributo $A_j$, se pueden estimar como:

$$P(A_{jk}|c_i) ~ N_{jki}|N_i$$

Donde $N_{jki}$ es el numero de veces que el atributo $A_i$ toma el valor k y es de la clase i y $N_i$ es el número de muestras de la clase $c_i$ en el conjunto de datos.

Tenemos:

$$P(C|A_1,A_2,...A_n) = \frac{P(C)P(A_1|C)P(A_2|C)...P(A_n|C)}{P(A)}$$

La predicción será la clase que maximice lo siguiente:

$$Arg_c[Max[\frac{P(C)P(A_1|C)P(A_2|C)...P(A_n|C)}{P(A)}]]$$

Dado que $P(**A**)$ es una **constante** se puede eliminar:

$$Arg_c[Max[P(C)P(A_1|C)P(A_2|C)...P(A_n|C)]]$$

Esto se puede experesar en terminos de una función que varia monotonicamente con respecto a P(C|**A**):

$$Arg_c[Max[log(P(C)P(A_1|C)P(A_2|C)...P(A_n|C) )]]$$

$$Arg_c[Max[log(P(C))+log(P(A_1|C))+log(P(A_2|C))...+(logP(A_n|C))]]$$

Si **n** es grande, despues de multiplicar las **n** probabilidades condicionales, el valor resultante se aproximará rapidamente a cero.

- _Las computadores tienen un limiteen la representación de valores de punto flotante_

Es por eso que se opta por aplicar logaritmo para obtener una suma de logaritmos:
$$Arg_c[Max[log(P(C))+log(P(A_1|C))+log(P(A_2|C))...+(logP(A_n|C))]]$$