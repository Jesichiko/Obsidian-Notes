---
Fecha de creación: Fecha inválida
Clase: M.Datos
---
Cada uno definirá su propia lista de stopwords

**Transformación de los datos**:

- Bas-of-words (Bolsa de palabras)”
    
    Es una técnica fundamental en el procesamiento del lenguaje natural (NLP) que se utiliza para representar texto en un formato comprensible para algoritmos y de aprendizaje automático.
    
    Su nombre **“Bolsa de palabras”**, refleja su **esencia**:
    
    En esta técnica, el orden y la gramática de las palabras se ignora y solo se considera la frecuencia o presencia de las palabras en un documento.
    
      
    

¿Cómo funciona el **BOW**?

- Creacion del vocabulario:
    
    Se recopilas todas las palabras **únicas** presentes en los documentos que se desean analizar, eliminando duplicados.
    
    Por ejemplo, considere los siguientes docs:
    
    **Doc1**: “Me gusta el aprendizaje automático autmático”
    
    **Doc2**: “El aprendizaje automático es interesante”
    
    El **vocabulario** del ambos docs sería:
    
    **Vocabulario**: “me”, “gusta”, “el”, “aprendizaje”, “automático”, “es”, “interesante”
    
- Vectorización
    
    Cada documento se converte en un **vector** que indica la **frecuencia** o **presencia** de cada palabra del vocabulario
    
    Ejemplo de vectorización por frecuencia:
    
    **Doc1:** “Me gusta el aprendizadje automático automático”
    
    [ 1, 1, 1, 1, 1, 0, 0]
    
    **Doc2:** “El aprendizaje automático es interesante”
    
    [0, 0, 1, 1, 1, 1, 1]
    

Con **Bow** obtenemos una matriz de tamaño **num_de_documentos** * **tamalo_del_vocabulario**:

1 1 1 1 1 0 0

0 0 1 1 1 1 1

Esto lo podemos almacenar como un archivo csv y caargarlo como una **matriz**

**Puntos negativos de BoW**

- Pierde el contexto y el orden de las palabras, lo que limita su capacidad para capturar el significado profundo del texto
- Puede generar vectorese **muy grandes** si el vocabulario es amplio