---
Fecha de creación: Fecha inválida
Clase: M.Datos
---
Basado en la [[Probabilidad Condicional]] y la ley de la _probabilidad total_, el reverendo **Thomas Bayes** expuso el siguiente teorema:

Dado un evento **A** y **n eventos mutuamente excluyentes y colectivamente exhaustivos B1, B2, … Bn,** entonces la probabilidad de cualquiera de los eventos **Bi,** condicionado al evento **A** puede calcularse como:
2.$$P[A_n/B] = \frac{P[B/A_n]*P[A_n]}{\sum P[B/A_i]*P[A_i]}$$
De acuerdo con la definición de la probabilidad condicional tenemos que:
3.$$P(B/A) =  \frac{P(A \cap B)}{P(A)}$$
o bien, considerando un evento cualquiera **Bj**, condicionado a otro evento **A**, la fórmula precedente se puede escribir como:

Por otro lado, si consideramos el evento **A** condicionado a **Bj**, tenemos que:
Siendo **$P(B_i) > 0$**:

A su vez, como: $P(Bj A) = P(A Bj)$, podemos reemplazar la expresión (3) en el numerador de (2):
4.$$P(Bj | A) = (P(A|Bj)P(Bj))/P(A)$$
Luego si Bj pertenece a un grupo de eventos mutuamente excluyentes y colectivamente exhaustivos, y de acuerdo con la ley de la probabilidad total, tenemos que la probabilidad del evento $A$ se puede escribir como:
5.$$P(A) = \sum P(A|Bi)P(Bj)$$
Finalmente reemplazando (5) en el denomiador de (4), se obtiene el **Teorema de Bayes**:
$$P(Bj|A) = (P(A|Bj)P(Bj))/(P(A|Bi)P(Bi))$$

**Fase de prueba:**
**Rainy; High; High; True;**

Tenemos:
$$P(NO)P(Rainy|NO)P(High|NO)P(High|NO)P(True|NO)$$
$$= (5/14)(2/5)(2/5)(4/5)(3/5)=\frac{0.0274}{0.0274+0.0053}=0.83$$
$$P(YES)P(Rainy|YES)P(High|YES)P(High|YES)P(True|YES)$$
$$=(9/14)(3/9)(2/9)(3/9)(3/9) = \frac{0.0053}{0.0274+0.0053}=0.17$$