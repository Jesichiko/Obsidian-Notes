---
Fecha de creación: Fecha inválida
Clase: Sistemas Operativos 2
---
El Sistema Operativo se divide generalmente en:

- Kernel
- Gestor de Procesos
    - Procesos
    - IPC
    - (RPC, Sockets)
- Memoria
- _**Sistema de Archivos**_
- E/S

El **Sistema de Archivos** se encarga de almacenar datos largos, rastrearlos y ordenarlos. En Linux se trabaja con un modelo de Á_rbol_ el cual permite saber información valiosa de los archivos/directorios.

  

Los archivos son los elementos principales en la mayoría de aplicaciones y estos archivos **pueden tener propiedades como**:

- Long-Term existencia
- Compartibles entre procesos
- Estructura predeterminada

  

El Sistema de Archivos también contiene un **gestor de archivos (File Management)** que gestiona copiado de archivos, creación de archivos, eliminación de archivos, etc. También el Sistema de archivo provee de funciones **primitivas** como:

- Create
- Delete
- Open
- Close
- Read
- Write

Esto nos da como resultado que **un archivo puede ser de lectura, escritura o de ejecución**.

**Términos**

Hay 4 términos comunes al hablar de SF:

- Field
    - Elemento básico de dato
    - Contiene solo un valor
    - Tiene un tamaño y un tipo de dato
- Record
    - Colección de Fields relacionados
    - Tratado como una unidad
- File
    - Tiene nombre
    - Es una colección de Records
    - Tratado como una sola entidad
    - Puede implementar mecanismos de control de acceso
- Database
    - Colección de datos relacionados
    - Existencia de relaciones entre estos elementos
    - Consiste de uno o mas archivos

Tarea: Investigar sistema de archivos de cloud computing