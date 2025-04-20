---
Fecha de creación: Fecha inválida
Clase: M.Datos
---
![[image 34.png]]

![[image 35.png]]

Nosotros veremos algunas tecnicas de preprocesamiento usadas principalmente para:

- Textos
- Clasificación

Aunque las técnicas no están limitadas a estas

**Limpieza de datos**.

Caracteres especiales. Los caracteres especiales osn simbolos o signos que no forman parte del conjunto estándar de letras y números. Estos caracteres tienen funciones especificas y se utilizan en distintos contextos.

![[image 36.png]]
Para nuestra tarea:

- ¿ Nos sirven los caracteres especiales?
    - ,.()={}[]’#$
- ¿ Nos sirven los números?
    - 1, 90, 202122889
- ¿Nos sirven las “palabras” alfanuméricas?
    - Correo3, d45as5

Si no nos sirven, podemos eliminarlos.

Ejemplo:

¡VAMOS A LOGRARLO! \#ÉXITO

VAMOS A LOGRARLO ÉXITO (limpiado)

![[image 37.png]]

Para nuestra tarea de clasificación de textos:

¿ Nos sirven la diferenciación de las mayúscula y minúsculas?

Las codificaciones de las letras mayúsculas y minúsculas es diferente, por lo que palabras como “Hola” y “hola” son diferentes.

Para nuestra tarea de clasificación de textos podemos quitar las mayúsculas

En este caso que no sea necesario mantener mayúsculas y minúsculas podemos optar por mantener solo una de ellas, comúnmente, minúsculas:

- !VAMOS A LOGRARLO! \#ÉXITO
- !vamos a lograrlo! \#éxito
  

**[[Stop Words]]**

Las [[Stop Words]] son palabras comunes y frecuentes en un idioma que, por lo general, no aportan mucho significado o valor semántico en el análisis de texto y, por ende, suelen ser eliminadas durante el preprocesamiento en tareas de Procesamiento del Lenguaje Natural (NLP, por sus siglas en inglés).

Ejemplos de stopwords:

Articulos: “el”, “la”, “los”, “las”

Preposiciones: “a”, “de”, “en”, “por”, “para”

Conjunciones: “y”, “o”, “pero”, “que”.

Pronombres: “yo”, “tú”, “él”, “ella”, “nosotros”.

  

Las stopwords suelen ser eliminadas por diferentes razones, algunas de ellas son:

- **Reducción del ruido:** Estas palabras se repiten mucho en los textos, pero no ayuan a diferenciar el contenido ni el contexto.
- **Optimización de recursos:** Eliminarlas reduce el tamaño del texto a procesar, lo que mejora el rendimiento de los algoritmos.
- **Mejor enfoque**: Permite que el modelo se concentre en palabras más significativas que realmente representan el contenido del contexto.

  

Ejemplo

- vamos a lograrlo éxito
- vamos lograrlo éxito
  

**¿Siempre se deben eliminar las stopwords? No**

En _análisis de sentimiento_, palabras como “No” (en frases negativas) son críticas

En _traducción automática_, todas las palabras, incluso las frecuentes, son relevantes

![[image 38.png]]

Aparte de las **Stop Words** existen otras tecnicas para preprocesamiento como el [[Suavizado Laplaciano]].