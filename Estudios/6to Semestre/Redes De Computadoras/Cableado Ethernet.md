---
Fecha de creación: Fecha inválida
Clase: Redes
---
Los cables Ethernet se pueden clasificar en 3 categorías:

1. Para enviar
2. Para recibir
3. Para enviar y recibir

Estas categorías se definen por el tipo de cableado que tenga.

![[c326a831-f87b-49ce-9c54-9e63c8af034f.png]]

Ademas, dependiendo del tipo de cable el _trenzado_ variara. En este caso la separación de los colores es de la siguiente manera:

![[image.png]]

1. Blanco con anaranjado
2. Verde claro con azul marino
3. Azul claro con verde oscuro
4. Café claro con café

Esta configuración es la B (configuración B). Los cables deben cortarse al mismo nivel antes de insertarlos en el Jack.

![[95dcda99-6cdd-400f-a8eb-ea3e1abfd58f.png]]

El Jack tiene que estar de esta forma para que funcione en la configuración B. Verificamos que este correctamente alineado los cables y que no haya salido nada mal en los pasos anteriores y procedemos a ponchar el cable.

![[6fe66bea-9c5b-4d59-a421-1d1e5eb75f51.png]]

El ponchado del cable es la parte donde se ajustan (se aprietan) los cables junto con el Jack de forma que este no se salga. SI todo salió bien, ya tenemos nuestro cable ponchado correctamente listo para poder usarse. Se repite el proceso dos veces para la punta de cada cable y se verifica conectandolo a un router/modem.

![[4255b176-e952-4702-b728-95347b55238a.png]]

El resultado nos deja con un cable Ethernet que puede ser usado para poder conectarse a una red.

![[8fd29540-7ae5-410d-bb9b-593ec8eee1e1.png]]

  

**Interfaces - Redes de computadoras 13/Feb/25**

Las interfaces son los puntos de interacción entre las diferentes capas. Cada capa tiene una interfaz bien definida que le permite comunicarse con la capa superior e inferior. Estas interfaces especifican como se deben intercambiar los datos y qué servicios se van a dar.

  

**Funciones**

1. Encapsulación y desencapsulación de datos: Cuando los datos se transmiten desde una capa a otra se encapsulan en un formato especifico para esa capa. La interfaz de ambas capas se encarga de desencapsular los datos para que puedan ser procesados
2. Control de flujo: Las interfaces tambien se encargan el flujo de datos entre las capas. Esto evita que una capa abruma a otra con una cantidad excesiva de información.
3. Manejo de errores: Las interfaces pueden incluir mecanismos para detectar y corregir errores que puedan ocurrir durante la transmisión de datos.
4. Multiplexación y demultiplexación:

**Encapsulación**

Proceso de añadir información adicional a los datos originales a medida que estos descienden por las capas del modelo de red (como el modelo OSI o TPC/IP). Esta información adicional que se añade en forma de encabezados y a veces colas, permite que cada capa realice sus funciones específicas

La **desencapsulación** es el proceso inverso a la encapsulación. El receptor pasa por todas las capas de manera inversa para poder saber el mensaje o paquete.