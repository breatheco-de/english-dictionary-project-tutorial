<!--hide-->
# Urban Dictionary Terminal App
<!--endhide-->

![Urban Dictionary Terminal App](https://github.com/breatheco-de/english-dictionary-project-tutorial/blob/master/preview.gif?raw=true)

El [Urban Dictionary](https://www.urbandictionary.com/) es un recurso increíble para los amantes del inglés; tiene definiciones precisas de palabras, no como otros servicios como Wikipedia, Oxford, etc. 😅

En este proyecto, creará un diccionario basado en la terminal (CLI).

### Antes de empezar

1. Créate una cuenta en[RapidAPI.com](https://rapidapi.com/) y solicita tu key para la [urban dictionary API](https://rapidapi.com/community/api/urban-dictionary).
2. Ve este video de 15 minutos para comprender [pipenv](https://www.youtube.com/watch?v=6Qmnh5C4Pmo), the python package manager.
3. Ve este video de 10 minutos para comprender [qué son las API Keys y las credenciales](https://www.youtube.com/watch?v=InoAIgBZIEA).


## 🌱  Cómo iniciar este proyecto

1. Este proyecto viene con los archivos necesarios para empezar a trabajar, pero tienes dos opciones para empezar:

a) Abrir este link con Gitpod (recomendado) en tu navegador: https://gitpod.io#https://github.com/breatheco-de/urban-dictionary-project-tutorial) 

b) Clonar este repositorio localmente en tu computador:
```sh
$ git clone https://github.com/breatheco-de/urban-dictionary-project-tutorial) (recomended)
```

2. Instala las dependencias de la aplicación (solo una vez):

```bash
$ pipenv install
```
3. Ejecuta la aplicación escribiendo (cada vez):

```bash
$ pipenv run python app.py
```

### 📝 Features that the application must have

1. Saludar al usuario.
2. Preguntarle al usuario cuál es el término que quiere buscar, usa el input o la entrada de la función de python `input("What term do you want to look for?")`.
3. Usa el paquete de solicitudes de python para codificar tu solicitud GET en la API Urban Dictionary 

Supongamos que estamos buscando la definición de la palabra `computador`. La especificación de la API dice que debes realizar una solicitud GET a la siguiente URL:

```python
url = "https://mashape-community-urban-dictionary.p.rapidapi.com/define?term=computer"
```
No olvides añadir los `headers` con las credenciales de la API, please refer to [ejemplo de la API en la documentación](https://rapidapi.com/community/api/urban-dictionary/endpoints).

4. Procesa el response body, entiéndelo y obtén la definición de la palabra en response body entrante. 
5. Muestra la definición en la terminal.
6. Guarda la definición en un archivo JSON (JSON file).

### 🤠 ¿Te sientes con seguro?

Los siguientes requisitos no son obligatorios, pero puedes intentar completarlos si se siente seguro:

1. Sistema de caché: si el usuario vuelve a pedir la misma palabra, en lugar de volver a llamar a la API, debería tener las respuestas anteriores almacenadas en un `dict`.
2. Busca varias palabras separadas por comas.
3. Usa `sys.argv` para permitir que el usuario solicite una definición como esta:

```python
# "enjoy" es la palabra que el usuario está buscando
$ pipenv run python app.py enjoy
```

Pistas: [como usar sys.argv](https://www.pythonforbeginners.com/system/python-sys-argv)



