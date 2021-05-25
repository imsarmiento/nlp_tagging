# Tagging Script


## Antes de ejecutar

En el archivo config.yaml:
1. Asegúrate que el valor de current_index sea -1. Este índice se utiliza para guardar tu progreso cada vez que desees parar. El script ejecuta el Tweet que corresponda al valor de current_index + 1. No modifiques este parámetros a menos de que suceda algún arror. 
2. Escoge la ruta en la que se encuentra tu archivo de origen (un .pkl) y escribíbela en la variable filename.
3. En el idioma de origen, el API de Google lo detecta automáticamente pero puedes especificarlo si lo deseas.
4. Tags corresponde a las etiquetas y al orden específico en el que serán mostradas dentro del Script. Este parámetro tampoco se debería cambiar.
5. Si deseas traducir los Tweets, asegurate que translate sea true, de lo contrario, déjala como false. Puedes configurar el idioma al que quieras traducir los Tweets.

En tu ambiente de ejecución:
1. Asegurate de tener instaladas las librerías utilizadas, sobretodo [deep_translator](https://pypi.org/project/deep-translator/) (la puedes instalar con ```pip install -U deep_translator``` ).

Para empezar a usar:
1. Ejecuta el script con ``` python tagger.py ```
2. Después de leer el Tweet, ingresa la categoría correspondiente (las puedes revisar en consola)
3. Si ingresas un parámetro inválido se repitirá el Tweet
4. Si quieres corregir una etiqueta, lo mejor es que detengas la ejecución y lo edites manualmente. 

Para terminar de usar:
1. Solo deten la ejecución con ```ctrl-c y en los archivos .JSON quedará guardado tu progresp


## Resultados

El archivo final será un .JSON que después podrás convertir a tu formato de preferencia. 


