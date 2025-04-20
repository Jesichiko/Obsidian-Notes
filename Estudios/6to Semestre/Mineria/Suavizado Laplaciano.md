---
id: Suavizado Laplaciano
aliases: []
tags: []
---

Hay situaciones en las que una combinación podría no encontrarse en el conjunto de datos, dando una **frecuencia** de 0.

Los 0’s causan problemas en los modelos probabilistas, por lo que deben ser evitados.

Una forma de removerlos es usar un suavizado Laplaciano:

- _El suavizado laplaciano consiste en sumar una unidad a todas las **frecuencias**_

Ejemplo:

Suponga una variable **A** (que toma valores $a_1,a_2$) y una variable **B**($b_1, b_2$). Al intentar estimar $P(A|B)$ se obtienen las siguientes frecuencias:

|     |     |     |
| --- | --- | --- |
|     | b1  | b2  |
| a1  | 0   | 2   |
| a2  | 0   | 3   |

Sin **suavizado laplaciano**

|     |     |     |
| --- | --- | --- |
|     | b1  | b2  |
| a1  | 0+1 | 2+1 |
| a2  | 0+1 | 3+1 |

|     |     |       |
| --- | --- | ----- |
|     | b1  | b2    |
| a1  | 0.5 | 0.429 |
| a2  | 0.5 | 0.57  |

Con **suavizado laplaciano**

Ejemplo de tabla (Whatsapp):
**Fase de entrenamiento:**
$$P(Play) = [5/14(NO) 9/14(YES)]$$

$P(Outlook | Play)$:
|          | NO  | YES |
| -------- | --- | --- |
| Overcast | 0   | 4/9 |
| Rainy    | 2/5 | 3/9 |
| Sunny    | 3/5 | 2/9 |

$P(Temperature | Play)$:
| | NO | YES |
| ------ | --- | --- |
| low | 1/5 | 3/9 |
| medium | 2/5 | 4/9 |
| high | 2/5 | 2/9 |

$P(Temperature|Play):$
| | NO | YES |
| ------ | --- | --- |
| normal | 1/5 | 6/9 |
| high | 4/5 | 3/9 |

$P(Windy|Play)$:
| | NO | YES |
| ----- | --- | --- |
| False | 2/5 | 6/9 |
| True | 3/5 | 3/9 |
