---
Fecha de creación: Fecha inválida
Clase: Fundamentos de la Programación
---
En las funciones del [[Funciones Basicas]] o [[Funciones de Alto Nivel]]:

![[image 32.png]]

Se encuentran los siguientes entornos de variables:

- Para la variable _**param**_, debido a que se **define dentro de add**, su entorno **no pasa más allá de la misma**. Esta variable dejará de existir después de que la función termine. Si intentamos acceder a ella después de la ejecución, su valor se habrá perdido.
    
    Específicamente, se trata de una **variable ligada** (cálculo lambda) que solo puede existir dentro de la función, ya que se define como parámetro de esta.
    

- En el caso de la variable _**result**_, como no está definida en la función y **solo se hace referencia a ella**, su **entorno es más alto a la función**. Por lo tanto, si accedemos a ella después de la ejecución de la función, su valor se mantendrá.
    
    Específicamente, esta es una **variable libre** (cálculo lambda) que existe más allá de la función, pues no se define dentro de ella.  
    
![[image 33.png]]
En el siguiente caso tenemos:
- Las variables _**p**_, _**q**_, _**result**_ y _**arg**_ se definen como **variables libres**. Sin embargo, al definir la función **add**, el **contexto** de p se **redefine**. Es decir, la **p** dentro de la función y la **p** que es una **variable global** son completamente distintas, y la función **prioriza el ambiente de las variables declaradas en ella misma**. Si accedemos a p antes de ejecutar la función, su valor será 10; cuando ejecutemos la función, el contexto cambia y la nueva **p tendrá un valor diferente a 10**.