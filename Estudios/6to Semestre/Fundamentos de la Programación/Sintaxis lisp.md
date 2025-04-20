---
Fecha de creación: Fecha inválida
Clase: Fun
---
21/Febrero/25
Usamos clisp, ejemplo:
```lisp
(set (quote ‘(2 (3) 4) ) )
(setq ‘(2 (3) 3) ) = set quote abreviado
(set (quote lista))
```

Si no agregamos “quote” nos da error de sintaxis, sin embargo, podemos usar ‘ (comilla, que equivale a la funcion _quote_). Por ejemplo podemos hacer lo siguiente:
```lisp
(set ‘lista ‘(1 2))_ y esto es valido.
```
La función básica de lisp es Eval, que se define desde el calculo lambda:

_**(Eval E-Exp)**_
Esta función evalúa la expresión E-Exp y se tiene que seguir la estructura. Funciones como cdr, set y quote siguen esta estructura.

Hay dos funciones clave para listas en LISP:

1. CAR: Función que devuelve el primer elemento de una lista
2. CADR: Función que devuelve el segundo elemento de una lista

Ejemplo tenemos la siguiente lista: (2 (3) 4). Para poder inicializarla hacemos lo siguiente:
```lisp
(set 'lista '(2 (3) 4))  
>(2 (3) 4) (retorno del programa)

( cons (cadr lista) '())
>((3)) (retorno)
 ``` 
Si por ejemplo queremos concatenar la misma lista dos veces (Ej. ( (2 (3) 4) (2 (3) 4) ) separando las listas concatenadas podemos hacer lo siguiente:
```lisp
(cons lista lista)  
> ((2 (3) 4) 2 (3) 4) 
;esto nos da un error, la lista que queremos concatenar la “deconstruye”  
```
La manera correcta sería:
```lisp
(cons lista (cons lista Nil ))  
>((2 (3) 4) (2 (3) 4)) 
;esto no deconstruye la lista original y la concatena dos veces)
```
