---
Fecha de creación: Fecha inválida
Clase: Prog. Concurrente
---
Programación para memoria compartida

  

En los sitemas de multiprocesadores, cada procesador puede acceder a toda la memoria, es decir, hay un espacio de direccionamiento compartido.

Todo los los procesadores se encuentran igualmente comunicados con la memoria principal y pueden acceder por medio de un ducto común.

En está configuración se debe asegurar que los procesadores no accedan de manera simultánea a las regiones de memoria de tal manera que se provoque un error.

Por ejemplo, si dos o más procesadores desean actualizar una variable compartida se deben establecer procedimientos que permitan acceder a los datos compartidos como exclusión mutua.

**Cluster**: Conjunto de procesadores conectados mediamente que comparten memoria