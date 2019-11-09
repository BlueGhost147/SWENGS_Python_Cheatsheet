# SWENGS_Python_Cheatsheet
Useful commands for Python and Django (beginner level)

## Local enviroment 
Requirments
````bash
pip install virtualenv
````
### Create local enviroment
````bash
virtualenv venv
````
### Activate the local enviroment
````bash
cd venv\Scripts\
activate.bat
````

### Helpfull script (for VS code users)
Create the VEnv and copy the following command in a .bat file
````bash
cd <YourPythonProjectFolder>
cmd /k C:\Python\venv\Scripts\activate.bat
````

## Django
### Install django in your local enviroment
````bash
pip install django
````

### Create a new project
````bash
django-admin startproject <ProjectName>
cd <ProjectName>
````

### SQL Datenbank erstellen
````bash
python manage.py migrate
````

### Superuser erstellen
````bash
python manage.py createsuperuser
````

### Start server
````bash
python manage.py runserver
````

## Database Model Commands
### Änderungen für eine Datenbankmigration vorbereiten und übernehmen
(Verwendet die Datenbank welche im settings.py definiert ist)
````bash
python manage.py makemigrations
python manage.py migrate
````

### Zeigt den aktuellen Migrationssatus an (wie git status)
````bash
python manage.py showmigrations
````

### Bestehende Datenbank in DjangoModels umwandeln
````bash
python manage.py inspectdb
````

## Other - Requirements.txt
The requirements.txt specivies the dependencies a project needs (libraries).
### Generate a requirements.txt from the current virtual environment
````bash
pip freeze > requirements.txt
````
### Install the dependencies from a requirements.txt in a new virtual environment
````bash
pip install -r requirements.txt
````

