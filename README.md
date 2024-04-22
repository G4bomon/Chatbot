# chatbot

Este proyecto tiene la funcion de responder las preguntas mas comunes de un usuario con respecto a la universidad maritima del caribe, tiene respuestas pregeneradas pero en mi labor social de la universidad estoy trabajando en agregarle un modelo de lenguaje.

la forma en la que funciona es que al mandarle un mensaje separa las palabras en distintos prompts y los compara con las palabras clave de la base de datos, despues de eso envia la respuesta asociada con la mayor coincidencia de palabras clave, ademas tiene una columna para determinar si alguna palabra clave es necesaria para contar esa respuesta, vease por ejemplo la palabra clave pensum es necesaria para las respuestas con relacion al mismo

el proyecto fue realizado en django y puesto en linea durante un corto periodo con un servidor en ubuntu, sin embargo tambien funcina en windows, para ejecutar el proyecto necesitara descargar el requirements.txt y instalar los paquetes necesarios con "pip install -r requirements.txt" en python

una vez hecho eso necesita descargar el contenido de este github asegurese de que la carpeta donde lo descarga tenga el nombre de "intento". El archivo de "respuestas.sql" son los comandos para crear la base de datos en el sistema sql de su conveniencia, debe determinar los nuevos datos de su base de datos en "settings.py" dentro de la carpeta "intento", en la linea 76-84 y en "chat.py" dentro de la carpeta "no", en la linea 5-10

una vez configurado esto podra ejecutar el ayudante virtual en su computador con el comando "py manage.py runserver"
