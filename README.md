# Sistema-Juego-de-rol
Siestema basado y credo con el framework de Python Django en su version 4.0.5,  django-environ en su version 0.9.0 , Pillow en su version 9.2.0.


El sistema se baasa en un administrador y creador de perfiles de usuarios Jugador y gameMaster(staff) el cual es un usuairo con ciertos permisos ya que es el perfil de tipo administrador en este caso de sitioo web.



Para su utulizacion son requeridos los parametros necesarios como Pytohn y su gestor de paquetes pip:

Instalacion:




1- Instalamos virtualenv:    Windows: python -m pip install virtualenv
                          Ubuntun/Debian: sudo apt-get install virtualenv (Para generar el PATH automaticamente,y no tener que configurarlo.)
                          
                          
                          
                                
2- Creamos entorno virtual:  Windowns: python -m virtualenv <nombre del entorno>
                             Ubuntu /Debian: virtualenv <nombre del entorno>
                             
                             
                             
3- Activamos entorno virtual:  Windows: en la ruta donde se creo el entorno con virtualenv | <nombre del entorno>/Scripts/activate
                               Ubuntu/Debian: en la ruta donde se creo el entorno con virtualenv | source <nombre del entorno>/bin/activate
                             
                             
                             
3- Instalamos dependencias:  Windows: python -m pip install -r requerimientos.txt (Si tiene instalado Python2 utilize python3 -r ...)



4- *COMANDOS DE UTILIZACION: 
              Pueden borrar la base de datos que se encuentra rolgame/rolgame/db.sqlite3 para tener una base de datos limpia.
              ** Para realizar verificar todas las migraciones : python manage.py makemigrations
              ** Para realizar migraciones: python manage.py migrate
              ** Para ejecutar el servidor python manage.py runserver
              **para la creacion de super usuarios (Administradores con todos los privilegios) utilice:  django-admin createsuperuser
               (Posterior mente, pidira los campos del modelo abstracto creado en los modelos de la aplicacion.)
5- 
            


                          
