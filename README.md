# Tagging Script


## Antes de ejecutar

En el archivo config.yaml:
1. Asegúrate que el valor de current_index sea -1. Este índice se utiliza para guardar tu progreso cada vez que desees parar. El script ejecuta el Tweet que corresponda al valor de current_index + 1. No modifiques este parámetro a menos de que suceda algún error y desees reiniciar / retroceder tu progreso. 
2. Escoge la ruta en la que se encuentra tu archivo de origen (un .pkl) y escribíbela en la variable filename. Es importante que escribas el nombre del archivo sin la extensión. Ej. si el archivo es ```Persona_en_N0.pkl```, escribe solo ```Persona_en_N0```. Es más facil si ubicas el archivo y el script en la misma carpeta.
3. El idioma de origen, el API de Google lo detecta automáticamente pero puedes especificarlo si lo deseas con es para español, fr para frances o en inglés.
4. Tags corresponde a las etiquetas y al orden específico en el que serán mostradas dentro del Script. Este parámetro tampoco se debería cambiar.
5. Si deseas traducir los Tweets (por ejemplo de francés a español), asegurate que translate sea true, de lo contrario, déjala como false. Puedes configurar el idioma al que quieras traducir los Tweets con los mismos prefijos que para el idioma de origen.


En tu ambiente de ejecución:
1. Asegurate de tener instaladas las librerías utilizadas, sobretodo [deep_translator](https://pypi.org/project/deep-translator/) (la puedes instalar con ```pip install -U deep_translator``` ).
2. Si trabajas con una versión de Pyhton menor a 3.8, cambia en el script ```import pickle as pk``` a ```import pickle5 as pk```. Recuerda instalarlo en tu ambiente. 

## Al ejecutar


Para empezar a usar:
1. Ejecuta el script con ``` python tagger.py ```
2. Después de leer el Tweet, ingresa la categoría correspondiente (las puedes revisar en consola)
3. Si ingresas un parámetro inválido se repitirá el Tweet
4. Si quieres corregir una etiqueta, lo mejor es que detengas la ejecución y lo edites manualmente. Este será el ultimo Tweet escrito en el archivo .JSON taggeado. 

Para terminar de usar:
1. Solo deten la ejecución con ```ctrl-c``` y en el archivo .JSON quedará guardado tu progreso.


## Resultados

El archivo final será un .JSON que después podrás convertir a tu formato de preferencia. 

***

Realizado por Steven Tarazona - [StevenTarazona](https://github.com/StevenTarazona)
