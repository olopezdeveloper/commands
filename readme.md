Comandos GIT

Clonar un repo:
git clone https://github.com/nombre_de_repo/

Actualizar repo del remoto al local:
git pull https://github.com/nombre_de_repo/

Revisar cambios pendientes:
git status
 
------------------------------------
Agregar archivos agregados y modificados
----------------------------------
git add .

--------------------------------
agregar archivos removidos y modificados
--------------------------------
git add -u

--------------------------------------------------
Prepara la eliminacion del archivo para el commit
---------------------------------------------------
git rm archivo.php

Commit rapido:
git commit -m "Creada carpeta de traducciones y añadida la española" -a


Actualizar delo local al remoto:
git push https://github.com/nombre_de_repo/


-----------------------------------------
Sigo la rama del server y la creo en mi local sincronizando
-----------------------------------------
$ git fetch (makes sure you have remote branch in local repository).
git branch --track branch-name origin/branch-name  
(creates local branch which tracks remote branch. It assumes that your remote name is origin)

------------------------------------
Crear rama local y cambiar a la misma:
------------------------------------
git checkout -b primera-rama


Agregar de la rama local nombre-rama a la del repo con el mismo nombre:
git push origin nombre-rama

Borrar rama del servidor
git push origin :nombre-rama

Configuracion global correo y nombre de usuario
git config --global user.email "you@example.com"
  git config --global user.name "Your Name"


-------------------
Agregar remoto
------------------
git remote add origin https://github.com/user/repo.git

---------------------------
ver la url remota del repo
--------------------------
 git remote -v

----------------------------
reasignar url remota
----------------------------

git remote set-url origin git://new.url.here

-----------------------------------------------------------
Si tienes más de un remoto, este comando los lista todos. 
----------------------------------------------------------

$ cd grit
$ git remote -v

-------------------------------------------
Traigo los cambios de remoto y fuciono dos proyectos de historiales distintos
--------------------------------------------
git pull origin master —allow-unrelated-histories

-------------------------------------
RAMIFICAR Y FUSIONAR:
-------------------------------------
Lista todas las branches escribiendo:
-------------------------------------
 git branch

----------------
crear rama
---------------
git branch <nombre_rama>


--------------------
Para cambiar de rama
-----------------------
git checkout <rama>

--------------------------------------------------------------
Para crear una nueva rama y saltar a ella, en un solo paso
--------------------------------------------------------------
 git checkout -b <rama>



-------------------------------------------
Cambio a master y fusiono hotfix a master
--------------------------------------------
git checkout master
git merge hotfix

--------------------------
Borrar rama
------------------------
git branch -d <nombre_rama>


----------------------------------------
Para volver en el tiempo y ver ese estado
-----------------------------------------
git checkout <commit>

--------------------------
Borrar cambios en stagging
-------------------------
git reset --hard

-------------------------
Ver commits anteriores 
-------------------------
git log

---------------------------------------------------------------------------------------------
Sincronizar ramas locales con ramas remotas (no baja cambios, solo le indica que hay nuevo) 
--------------------------------------------------------------------------------------------

git fetch

--------------------------------
retornar a un commit anterior
--------------------------------
git reset --hard (hash del commit)

 
 --------------------------------
Ignorar Archivo
--------------------------------
 git rm —cached <file>
 ir a .gitignore y tipear la ruta del archivo <file>
 

