---
Fecha de creación: Fecha inválida
Clase: Fundamentos de la Programación
---
Se crearon las primeras funciones, _sumar, cuenta_ para visualizar como es la sintaxis de una 
función **recursiva**:
_Función cuenta_
```lisp
; definir una funcion que cuente el numero de elementos que tiene una lista
; lista = (a b c) a = 1, b = 1+1, c = 1+1+1`

(defun cuenta (lst)`
    (cond ( (null lst) 0)`
        (T (+ 1 (cuenta (cdr lst))))`
    )
)
```
_Función sumar elementos_
```lisp
(defun suma (lst)
    (cond ( (null lst) 0)
        (T (+ (car lst) (suma (cdr lst))))
    )
)
```
Ejemplo:
![[image 16.png]]