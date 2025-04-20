La formulación del **Clasificador Bayesiano** se basa en la aplicación del [[Teorema de Bayes]] para estimar la probabilidad de cada clase dados los atributos:
(1)$$P(C|A_1, A_2, ..., A_n) = \frac{P(C)P(P_A1, A_2, ..., A_n | C)}{P(A_1,A_2,...,A_n)}$$
Lo cual se puede escribir de forma más compacta como:
(2)$$P(C |A) = \frac{P(C)P(A|C)}{P(A)}$$
El problema de clasificación, basado en la ecuación (2), se puede formular como:
(3)$$Arg_c[Max[P(C|A) = \frac{P(C)P(A|C)}{P(A)}]]$$