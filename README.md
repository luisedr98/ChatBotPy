# Proyecto de Chatbot mediante RASA Python 

El presente proyecto presenta el desarrollo de un chatBot mediante el uso del framework RASA para el lenguaje de programación python

## Especificaciones 

- Desarrollado en lenguaje python v3.7.9
- Es necesario para su funcionamiento la creación de un entorno virtual y descarga de dedpendecias.

## Preparacion del entorno virtual y paquetes necesarios

Para el uso es necesario seguir el siguiente procedimiento. Ingresar a la carpeta donde se encuentra la carpeta "hospital" y mediante el el uso del comand prompt construir un entorno virtual mediante la ejecución de los siguientes comandos:

    python -m venv nombre_del_entorno
    .\nombre_del_entorno\Scripts\activate
    python -m pip install rasa

## Ejecución del ChatBot

Para la ejecución del ChatBot es necesario ejecutar los siguientes comandos en la carpeta donde se encuentra el entorno virtual y el proyecto

    .\nombre_del_entorno\Scripts\activate
    cd hospital
    rasa train
    
Luego de la ejecución del comando ***rasa train*** se generará las carpetas **.rasa** y **models** en la ultima se encuentra el resultado del entrenamiento. Una vez generado directorios es necesario ejecutar

    rasa run actions 
    rasa run shell