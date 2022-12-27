# PRACTICE TEAM WORKFLOW WITH GIT AND GITHUB


## 2022-12-21 PRACTICE

### Exercise one

For this exercise, practice will focus on how to update a forked repository when changes are made in the original one. For this purpose, git fetch and git merge will be used widely. Olso, it will consist on settling the steps to follow in the process of working with a forked repository.

#### Steps:
+ make a commit with this file filled with the wording for this exercise.
+ on the other computer, fetch the changes made to the original repository on zuleta13, review the changes and, finally, merge them into the cloned repository.
+ do the first two steps a couple more times.

#### Add modifications here from branch Rodri
1. My first commit from branch Rodri.
2. My second commit from branch Rodri.

#### Exercise final notes
+ when fetching a branch from another repository this is the command:
git fetch repository-address branch-name
example: git fetch https://--------.git main
+ once you fetched the branch, it is available to checkout in FETCH_HEAD:
git checkout FETCH_HEAD
+ after checking it out, if you want to merge your branch with that one:
git merge FETCH_HEAD

#### One more thing before closing this exercise
I would like to check if it still works when the original repository is more than one commits ahead. What I want to be sure of is if this process will add all of the commits to the other repository.



## 2022-12-27 PRACTICE

### Exercise one

En este ejercicio, Liz llevará a cabo una tarea en el otro ordenador y realizará commits en su rama de trabajo. Cuando haya terminado, creará un pull request. Rodri le pedirá que haga algunos cambios y mantendrán una conversación en el pull request. Cuando Liz haya cumplido los requerimientos del proyecto, Rodri mezclará la rama de trabajo de Liz con la rama principal del proyecto.

#### Pasos
+ borrar el repositorio clonado del otro ordenador
+ volver a clonarlo
+ crear una rama de trabajo que se llamará Liz
+ en esa rama, realizar las tareas y hacer commits
+ hacer un pull request
+ revisar el pull request y pedir cambios
+ realizar los cambios y pedir una nueva revisión
+ aceptar los cambios y combinar el trabajo de Liz en la rama main del repositorio original
+ cerrar el pull request

#### Espacio reservado para el trabajo de Liz
1. Hola, soy Liz y este va a ser mi primer commit.
2. Soy yo de nuevo, vengo a hacer mi segundo commit.
