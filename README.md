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

---

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

---

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

+ dos: primer cambio para actualizar el branch remoto mediante el comando git push origin nombre

+ tres: segundo cambio para actualizar el branch remoto mediante git push (a secas)

---

## 2022-12-17 PRACTICE STARTS HERE

### Primer ejercicio

Quiero probar qué secede cuando creas una rama a partir de main y, después, creas otra a partir de la primera y, después, haces un rebase de la primera. Qué pasa con la segunda? Se queda como estaba? También se ejecuta el rebase en ella por estar hecha con respecto a la primera?

Interesante cuestión. Averigüemos la respuesta!

Hoy solo voy a trabajar localmente. Al finalizar el ejercicio, sincronizaré el repositorio remoto.

1. Este va a ser el primer commit. A partir de este crearé "uno", la primera rama partiendo de main.

2. Las ramas "uno" y "dos" ya están hechas. Decidí crearlas desde el mismo commit (Do first part of exercise one) porque, en realidad, no necesito que "dos" empiece desde un commit más avanzado de "uno" con respecto a main. Si la cosa funciona, funciona independientemente de en qué commit de cada rama se haya generado la otra rama.

3. Ahora voy a hacer un commit en main para hacer que las otras dos queden por detrás. Haré el rebase de "uno" y veré si ese rebase afecta a "dos".

4. Notas importantes:
  + el comando de rebase es: git rebase la-otra-rama
  + como sospechaba, el que haya hecho un rebase de "uno" no afecta en nada a "dos": son dos ramas independientes. Si son ramas pertenecientes a personas diferentes, cada uno debe hacer con la suya lo que estime oportuno para estar al día con main. 

---

## 2022-12-20 PRACTICE STARTS HERE

### Primer ejercicio

El objetivo será realizar las mismas acciones que en el ejercicio que se encuentra en la carpeta "rebase". Se trata de crear dos ramas a partir de la principal para que dos personas trabajen sobre el mismo archivo por separado. Por qué? Un ejemplo de mierda. La cuestión es aprender a solucionar las situaciones confusas y conflictos que se pueden crear cuando algo así ocurre.

Pasos:
+ se hará un commit con el enunciado.
+ se crearán las dos ramas a partir de ese commit: las ramas tendrán nombres Liz y Rodri.
+ Liz realizará algunos commits, hará push de su rama de trabajo y hará merge, comprobando antes que no se han producido cambios en la rama principal para evitar conflictos.
+ Rodri trabajará y hará commits locales. Después, al darse cuenta de que se han producido cambios en la rama principal, hará un rebase para poner su rama al día, y hará push y merge.

Notas:
+ a lo largo del camino, con toda probabilidad, habrá que solucionar conflictos, hacer fetch y merge en diferentes momentos, comprobar las diferencias entre el archivo en el directorio de trabajo y el mismo archivo en el repositorio remoto o en la rama de trabajo de la otra persona (esto último se puede hacer? Probablemente no, a menos que la otra persona haya hecho un push de su rama de trabajo al repositorio remoto. Comprobarlo).

#### Cambios generados por Liz
1. My first commit.
2. My second commit.

#### Cambios generados por Rodri
