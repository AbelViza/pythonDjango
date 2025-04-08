# pythonDjango
Apuntes sobre configuración y uso en windows

Preparación de entorno
Para la preparación del entorno voy a utilizar el bash de git el cual pueden descargar de la siguiente dirección:
https://git-scm.com/download/win <br>

$ py -m venv .env                                          -> Crea un entorno virtual <br>
$ source .env/Scripts/activate                             -> Activa el entorno virtual <br>
$ deactivate                                               -> Desactiva el entorno virtual <br>
$ pip install django -U                                    -> Instalar Django <br>
$ C:/Python39/python.exe -m pip install --upgrade pip      -> Actualizar pip <br>
$ pip freeze                                               -> Genera lista de bibliotecas instaladas<br>

# Iniciar Proyecto
$ django-admin startproject < nombre-proyecto > < ruta-creación ><br>
  Se crea carpeta con el<br>
  <br>
  < nombre-proyecto ><br>
  |_ __init__.py Declarar el proyecto como modulo de python<br>
  |_ asgi.py<br>
  |_ settings.py Define configuraciones del proyecto<br>
  |_ urls.py Punto de entrada para todas las peticiones<br>
  |_ wsgi.py Archivo usado en producción<br>
  manage.py Archivo interfaz sobre django admin
  
# manage.py
$ <b>py manage.py</b>  Muestra comandos<br>
$ py manage.py runserver<br>



# Iniciar una aplicación
$ py manage.py startapp < nombre-aplicación > <br>
Crea la carpeta<br>
< nombre-aplicación >
|_ __init__.py Declarar el proyecto como modulo de python<br>
|_ admin.py Se encarga de registrar los modelos
|_ apps.py Configuración de app
|_ models.py Definir modelos de datos
|_ tests.py Para pruebas
|_ views.py 
|_ [migrations] Modulo de python, se encarga de grabar los cambios en la base de datos
