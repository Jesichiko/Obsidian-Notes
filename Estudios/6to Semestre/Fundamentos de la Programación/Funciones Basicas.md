---
Fecha de creación: Fecha inválida
Clase: Fun
---
Hay funciones como reverse que invierten una lista dada:

![[image 1.png]]

Asi cosas que tengan que ver con listas se vuelven mas faciles:  
Por ejemplo, devolver el ultimo como lista o elemento:

- Como elemento:
    
    ![[image 2.png]]
    
- Como lista:
    
    ![[image 3.png]]
    
      
    

Si por ejemplo queremos los elementos 6 7 podemos hacer la siguiente **E-Expresión**:

![[image 4.png]]
  
**Función length**

Sintaxis: ( Length lista)

Ejemplo:

![[image 5.png]]

**Función last**
Esta función evita que tengamos que poner **E-Expresiones** con _inverse y list_ para sacar el ultimo elemento, sin embargo last **devuelve una lista con el ultimo elemento**

Sintaxis: (last lista)

Ejemplo:
![[image 6.png]]
Si queremos sacar el primer elemento:
![[image 7.png]]

**Función subst**
Esta funcion sustituye un elemento _b_ por un elemento _a_ en una _lista_ dada.

Sintaxis: (subst _a b Exp_), donde _a,b_ son expresiones simbolicas. Exp no necesariamente tiene que ser una lista explicita.

Ejemplo:

![[image 8.png]]

![[image 9.png]]

En esta función **no importa el nivel de la letra a sustituir, siempre la encontrará**.

**Función eval**

Esta función evalua la **E-Expresión** dada como parametro. Esta sirve para evaluar sobre todo funciones (que son expresiones evaluables)

Sintaxis: (eval E-expr)

Ejemplo:
![[image 10.png]]
En este caso ‘ se usa para no evaluar (o tomar literal) funciones. Ignora que el primer elemento es una función, sin embargo **debido a que estamos usando eval esta fuerza la función aunque se quiera tomar literal**.

**Funciones**

La estructura de toda función es:

Sintaxis: _(defun fn (arg 1 arg2 … argn)_

_E-Exp1_

_E-Exp2_

_E-Exp3_

.

.

.

_E-Expm_

)

_El resultado que devuelve la fn es el valor de la ultima E-Exp que evalue, es decir, **Valor(E-Expiesima) evaluada**_  

Ejemplo:

![[image 12.png]]

Si queremos que ultimo solo regrese el elemento, entonces se agrega _(car (last lst)):_
![[image 13.png]]-
# Funciones
1. #eq
	(**eq** atom0 atom2)
	    
	    Si atom1 = atom2 devuelve **T, sino Nil**. Solo pueden ser átomos, no listas.
	    
- (**atom** var)
    
    Si una var es un átomo, devuelve **T, sino Nil.**
    
- (**equal** exp1 exp2)
    
    Si la expresión 1 es igual a expresión 2 devuelve **T, sino Nil.** Si las expresiones son atomos le deja el trabajo a **eq**
    
- (**null** var)
    
    Si la variable var es una lista vacia devuelve **T, sino Nil.**
    
- (**Member** elem lista) busca elemento elem en una lista, devuelve **una lista apartir del elem encontrado**.