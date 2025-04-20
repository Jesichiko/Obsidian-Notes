---
Fecha de creación: Fecha inválida
Clase: Mineria de Datos
---
![[image 17.png]]

![[image 18.png]]

![[image 19.png]]

**Ejemplo 1:**

- Consideremos el lanzamiento de dos dados y los siguientes eventos:
    - **A1 = “resultado del primer dado es dos”**
    - **A2 = “El resultado del segundo es tres”**

La probabilidad marginal de cada uno de ellos es:
$P(A) = 1/6$
$P(B) = 1/6$

La probabilidad conjunta es:
$1/6 * 1/6 = 1/36$

**Ejemplo 2:**
- Consideremos el lanzamiento de dos dados y los siguientes eventos:
    
    - **B1 = “El resultado del primer dado es dos”**
    - **B2 = “La suma de los resultados de los dos dados es cinco”**
    
    La probabilidad marginal de cada uno de ellos es:
    
    $P(B1) = 1/6$
    $P(B2) = 4/36 = 1/9$

    La probabilidad conjunta es:
    $P(B_1 \cap B_2) = \frac{1}{36}$
    
En este caso los eventos **no son estadisticamente independientes**.
![[image 21.png]]

**Ejemplo 3:**
- Calculando las probabilidades condicionales del ejemplo 1, podemos verificar los siguientes resultados:
    - $P(A1|A2) = (P(A2|A1) * P(A1) )/P(A2)$
        $⇒(P(A2|A1) * 1/6) /1/6$
        $⇒ P(A2|A1)$
        $⇒ 1/6$
        
	- $P(A2|A1) = (P(A1|A2) * P(A2) )/P(A1)$
        $⇒ (P(A1|A2) * 1/6) /1/6$
        $⇒ P(A1|A2)$
        $⇒ 1/6$

En este caso podemos usarlo con la formula siguiente:

$P(A|B) = P(A intersecc B)/ P(B)$
$⇒P(A1|A2)$
$⇒ P(A intersecc B) / P(B)$
$⇒ \frac{\frac{1}{36}}{\frac{1}{6}}$
$⇒ 1/6$

**Ejemplo 4:**
- Al calcular las probabilidades condicionales del ejemplo 2, tenemos que:
    - **P(B1|B2)**  
          
        ⇒ **P(B1 intersecc B2) / P(B2)**
        
        ⇒ **1/36 / 4/36**
        
        ⇒ **1/4** (correcto)
        
    - **P(B2|B1)**  
          
        ⇒ **P(B2 intersecc B1) / P(B1)**
        
        ⇒ **1/36 / 1/6**
        
        ⇒ **1/6** (correcto)
        

Podemos ver que la simetría no se cumple aquí debido a que **no son estadisticamente independientes.**

  

**Ley de probabilidad total**

Utilizando el esquema de _probabilidades condicionales_, si no se conoce directamente la probabilidad de ocurrencia de un evento A:

- La misma puede obtenerse utilizando la _ley de la probabilidad total._
- La cual determina la probabilidad de un evento por medio de las probabilidades conjuntas del mismo con otros eventos mutuamente excluyentes y colectivamente exhaustivos.

Sea **A** un evento de un espacio muestral **S** y sea **Dj (j =** 1, 2, …, n) una partición del espacio muestral, es decir que los **Dj** son mutuamente excluyentes y colectivamente exhaustivos.

Entonces la _probabilidad total_ del evento **A** está dada por:

![[image 22.png]]

  

**Demostración:**

Si **Dj (j** = 1, 2, …, n) son eventos mutuamente excluyentes y colectivamente exhaustivos, entonces tenemos que:

![[8b5f4aa9-ea3b-4f75-9519-f751feaaec69.png]]

![[image 23.png]]

![[image 24.png]]

![[image 25.png]]

Esta fórmula puede comprobarse simplemente inspeccionando la siguiente figura:

![[image 26.png]]

**Ejemplo**:

Consideremos una bolsa con cubitos y bolitas de madera de dos colores (**rojo y verde**). Se sabe que:

- El 20% de las piezas rojas son bolitas, es decir, **P(forma = b | color = r) = 0.2**
- El 40% de las verdes son bolitas, es decir, **P(forma = b | color = v) = 0.4**
- Además se conoce que el 70% de las piezas son rojas, **P(color = r) = 0.7**

¿Cual es la probabilidad de extraer una bolita, **P(forma = b)**

![[image 27.png]]

**P(color):**

**P(color = r) =0.7**  
**⇒ P(color = v) = 0.3**  
(por 1 - P(r) )

**P(forma | color):**

Si forma = bolita tenemos:

**sumatoria P (forma = b intersecc color j)**
**⇒ P(b intersecc r) + P(b intersecc v)**
**⇒ P(b | r) * P(r) + P(b | v) * P(v)**
**⇒ 0.2 * 0.7 + 0.4 * 0.3**
**⇒ 0.14 + 0.12**
**⇒ 0.26** (correcto)

![[image 28.png]]

Tengamos en cuenta que:
$$P(A | B) = \frac{P(A \cap B)}{P(B)}$$

Despejando tenemos:
$$P(A \cap B) = P(A | B) * P(B)$$
**Ejemplo:**
Considere que en total hay 250 piezas en la bolsa. Usando los datos anteriores, llene la siguiente tabla:
![[image 29.png]]