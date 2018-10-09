**Esto es un tutorial que contiene comandos para ramas y GitHub**

# Ramas 

## Comandos ramas 1

* Ver listado de ramas: `git branch`
* Crear una rama: `git branch nombre_rama`
* Cambiarnos a una rama: `git checkout nombre_rama`
* Crear una rama y movernos en un paso: `git checkout -b nombre_rama`
* Comparar ramas: `git diff nombre_rama..nombre_rama`

## Comandos ramas 2

* Ver ramas identicas a la actual: `git branch --merged` 
* Renombrar ramas: `git branch .m nombre_antiguo nombre_nuevo`
* Eliminar ramas: `git branch -d nombre_rama`,`git branch -D nombre_rama`
* Integrar ramas a la actual: `git merge nombre_rama` 
* Resolver conflictos: `git merge --abort`

## Comandos ramas 3

* Almacenar cambios temporales: `git stash save "Mensaje"`
* Listar cambios: `git stash list`
* Ver contenido de un cambio temporal: `git stash show -p nombre_stash`
* Eliminar un cambio temporal: `git stash drop nombre_stash`
* Aplicar cambio del *stash*: `git stash apply nombre_stash`,`git stash pop nombre_stash` 

# GitHub

## Comandos GitHub 1

* Añadir repositorio remoto: `git remote add origin (url)` 
* Ver repositorios remotos: `git remote -v`
* Eliminar repositorio remoto: `git remote rm origin`
* Añadir cambios del repositorio local al remoto: `git push -u origin master`
* Añadir cambios del repositorio remoto al local: `git pull`

## Comandos GitHub 2

* Ver *branches* remotos: `git branch -r`
* Ver todos los *branches*: `git branch -a`
* Clonar un repositorio remoto: `git clone (url)`

## Dar seguimiento a *branches* remotos

* LOCAL->REMOTO
	1. Cambios en el repositorio local.
	2. Commit de cambios. 
	3. Añadir cambios a repositorio remoto: 
	* `git push`
* REMOTO->LOCAL
	* Sincronizacion y union: `git fetch origin`,`git merge origin/master`
	* En un solo paso: `git pull`

## Operaciones con *branches* remotos

* Creacion: 
	1. Crear branch local.
	2. Hacer cambios en dicho branch.
	3. Hacer commit.
	4. Copiar branch al repositorio remoto.
	* `git push -u origin branch_remoto`
* Copia: `git checkout -b local remoto`
* Eliminacion: `git push origin --delete branch_remoto`
