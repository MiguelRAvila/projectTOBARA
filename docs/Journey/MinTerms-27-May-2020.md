# [27 de Mayo del 2020]

## [Modificaciones del algoritmo del proyecto]

+ Se aprovechó a seguir una idea para hacer más claro el proceso del algoritmo: 

    * Tenemos dos matrices, la original que nunca se modificará y un detector de puntos. El original nos servirá para hacer más copias para detectar los cuadrados sin inteferir en colisiones.

    * El detector de puntos (active) Servirá para marcar cuales son las formas que se han encontrado hasta ahora, la idea es capturar a los términos incompletos mediante la búsqueda de rectángulos que cumplan las condiciones:

        1. El rectángulo debe ser potencia de 2.
        2. El rectángulo más grande será el termino principal.

    * En si, al desmarcar los activos en el detector de puntos, nos quedarán los posibles rectángulos que no se han formado en las anteriores búsquedas, sea del tamaño que sea.

    * Para la captura de los rectángulos se guardaran mediante 4 coordenadas que indican el tamaño del rectángulo.

    * Todas estas serán guardadas en una lista llamada MinTerms [] que serán las expresiones mínimas de la función.

    * Una vez sacados todos los minTerms, podemos pasar a la interpretación de los rectángulos, pero eso sera apenas se termine y compruebe el funcionamiento de la función reduceKmap().

+ Se realizó la bitácora correspondiente.
