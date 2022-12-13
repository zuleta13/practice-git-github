# PRACTICE GIT AND GITHUB COMMANDS AND WORKFLOW


## 2022-11-30 PRACTICE STARTS HERE

### Primer ejercicio

Primera modificación que realizo en README para comprobar el funcionamiento de los diferentes comandos.

Primer commit en este punto.

Segundo commit en este punto.


### Segundo ejercicio

Pasos a seguir:
+ Hacer un commit con el mensaje "Inicio del segunde ejercicio"
+ Crear un branch con el nombre ej2
+ Realizar dos modificaciones (en el espacio reservado) y hacer commit con cada una de ellas
+ Sin hacer push del branch ej2, intentar hacer merge con main
+ si no funciona, hacer push de ej2 y hacer merge con main

#### Realiza aquí las modificaciones

Modificación 1: miau!

Modificación 2: miau miau!

#### Notas

+ Efectivamente, se puede hacer merge sin hacer push. Push es para actualizar el repositorio remoto (el que está en GitHub).
+ En este caso, estábamos imaginando que trabajábamos solo con un repositorio local (aunque, en realidad, este repositorio sí tiene una copia remota).
+ Desde que hice el push del branch today (del ejercicio anterior), no deja de aparecer en los logs como origin/today, aunque no es importante (tiene sentido que un branch se quede retrasado cuando deja de usarse). El realmente importante es origin/main: este debe actualizarse siempre y estar en la cabeza o relativamente cerca.
+ Cuidado con los push de branches secundarios: ten en cuenta dónde estás trabajando, en qué repositorio. Es el principal? Es tu copia donde, si la cagas, no pasa nada?



## 2022-12-12 PRACTICE STARTS HERE

### Primer ejercicio

Pasos a seguir:
+ hacer un commit-push para que este enunciado quede como el último commit tanto en el repositorio local como en el remoto.
+ tomando este commit como origen, crear un branch para Liz.
+ ir al branch de Liz y hacer un commit para indicar que es el primer commit de ese branch
+ hacer un push para sincronizar este repositorio con el remoto (tendría que aparecer el branch de Liz)
+ realizar más cambios en el espacio designado para ella. Hacer tres commits.
+ hacer push
+ finalmente, hacer un merge

##### Nota: Según se desarrolle el ejercicio, revisar los logs para tener una respresentación del flujo de trabajo.

#### Realizar las acciones de Liz aquí
Hola, soy Liz. Este es mi primer commit en esta rama.

    Esta es una pruba de indentación en Markdown. Y será, también, el segundo commit. Gracias.

| Esto   | debería |
|--------|---------|
| ser    | una     |
| tabla  | .       |

*No se puede subrayar texto usando reglas de Markdown. Podría hacerse con HTML. En cambio, pongo el texto en cursiva.*



## 2022-12-13 PRACTICE STARTS HERE

### Primer ejercicio

En este ejercicio, vamos a practicar la creación y copia de branches locales en el repositorio remoto. Asimismo, estudiaremos las posibilidades para conectar esos branches de manera que al hacer un push del branch actual en el local, los cambios aparezcan reflejados en el branch del remoto.

Pasos a seguir:
+ creación de un branch local con main como base
+ mediante el commando git push -u origin nombre, crear el branch en GitHub y sincronizarlos de modo que las siguientes veces que quieras hacer un push, no tengas que especificar dónde quieres que se produzca.
+ hacer un commit y usar el comando git push para copiar el commit en el remoto
+ crear otro branch local
+ en GitHub, crear un branch con el mismo nombre manualmente
+ en Git, realizar algún commit y hacer un git push origin nombre-del-branch para comprobar que se puede hacer así
+ enlazar los branches local y remoto con git push -u origin nombre-del-branch
+ hacer otro commit y hacer git push para comprobar que ahora están enlazados y que no hace falta añadir la información del branch remoto

*Empezar el ejercicio despúes de esta línea*

+ cambio con el que realizaré el commit para luego hacer un push con el comando git push sin añadir más opciones porque las ramas local y remota ya están enlazadas.
