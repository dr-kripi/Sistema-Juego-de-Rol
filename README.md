# Sistema-Juego-de-rol
Siestema basado y credo con el framework de Python Django en su version 4.0.5,  django-environ en su version 0.9.0 , Pillow en su version 9.2.0.


El sistema se basa en un sistema web en el cual se pueden generar usuarios los cuales pueden crear jugadores con sus respectivas caracteristicas (Tambien pose un usuario de tipo juegador, ya que existen 2 tipos de usuario) y el usuario gameMaster(staff) el posee ciertos requerimientos y no puede realizar ciertas acciones.



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

  
  
 
5- Requerimientos implicitos del sistemas dados por la empresa ficcticia inifiti creations
  La empresa Infinity Creations, ha decidido llevar a una pequeña aplicación uno de los más populares juegos de rol. Para eso ha solicitado que se genere una aplicación que permita:

1. Crear un personaje a través de una plantilla

a. En los datos del personaje, se debe considerar:

i. Nombre del jugador (real)

ii. Nombre del personaje

iii. Raza

iv. Nivel

v. Estado (vivo, muerto, congelado)

b. Se deberá poder ingresar a lo menos 8 habilidades

c. Se deberá poder ingresar a lo menos 8 equipamientos de personaje

d. Se deberá poder ingresar a lo menos 4 poderes.

2. Todo personaje comienza con el nivel en 1

3. Todo personaje puede ingresar la primera vez:

a. 2 habilidades

b. 1 equipamiento

c. 1 poder

d. En estado vivo.

4. Existirá un perfil de GM (game master) quien podrá modificar las fichas de los personajes, con las siguientes restricciones:

a. No podrá eliminar las dos habilidades, el equipamiento y el poder ingresado por el jugador.

b. Podrá completar las habilidades faltantes o editar las que él ha ingresado.

c. Podrá completar el equipamiento faltante.

d. Podrá agregar o reemplazar poderes (solo reemplaza los que él haya ingresado).

e. Podrá subir el nivel de algún personaje, pero no bajarlo.

f. Podrá cambiar el estado de un personaje (de vivo a congelado, etc.)

5. El GM podrá ver un informe en donde vea los personajes de la partida, detallándose:

a. Nombre del personaje

b. Raza

c. Nivel

d. Estado

6. Las habilidades deberán estar en un listado, separado por raza.

7. Los poderes deberán estar contendidas en un listado, separados por raza.

8. Los equipamientos serán iguales para todos los jugadores.

9. No se podrá asignar una habilidad o un poder a una raza que no lo tenga.

10. El GM podrá agregar habilidades o poderes al listado identificando:

a. Nombre del poder

b. Detalle

c. Raza a la que pertenece.

11. Podrá editar poderes y habilidades en cuanto al detalle de éstas, pero no cambiar la raza a la que pertenecen.

12. El GM podrá agregar nuevas razas al sistema, pero no modificar las que ya existen.

13. El GM podrá agregar equipamiento al sistema, y modificar solo el nombre de éstos. No podrá eliminar equipamiento del sistema que se encuentren en uso.

14. Para ingresar al juego, se deberá ingresar a través de un usuario y contraseña.

a. El sistema deberá identificar si corresponde a un GM o jugador.

15. No puede existir un jugador que sea a la vez GM.

16. Un jugador podrá crear múltiples personajes y podrá ver los que él a creado en una tabla resumen, que indique:

a. Nombre del personaje

b. Raza

c. Nivel

d. Estado

17. El jugador podrá modificar el equipamiento de su personaje, si solo si este no se encuentra muerto.

18. Existen dos estados base del juego: Vivo y Muerto

19. El GM podrá agregar más estados al sistema, sin embargo, no podrá modificar los dos estados base.

20. Se deberá tener cuidado en la eliminación de cualquier estado, raza, habilidad o poder. No podrán ser eliminados si algún personaje lo tiene en uso o asociado.
            


                          
