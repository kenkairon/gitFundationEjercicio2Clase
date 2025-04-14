# git-hubFundation
Educativo y de Aprendizaje Personal

## Tabla de Contenidos
- [Requisitos](#requisitos)
- [Lista de Comandos](#Lista-de-Comandos)
---
## Requisitos

- Github-Foundation: 
---

## Lista de Comandos
1. listar archivos
   ```bash
   ls

2. Crear Directorios o Carpeta
    ```bash
    mkdir live

3. Ingresamos a la Carpeta Creada
    ```bash
    cd live

4. Para ver los archivos ocultos de git 
    ```bash
    ls -a

5. Crear archivos ejemplo index.html
    ```bash
    touch index.html

6. Para ver el estado o estatus de un archivo
    ```bash
    git status

7. Generamos el commit de confirmación
    ```bash
    git commit -m "Creamos el archivo index.html"

8. Verificamos el Historial de los commits Autor,Fecha, y la descripción del commit
    ```bash
    git log

9. Creamos otro Archivo commands.md 
    ```bash
    touch commands.md

10. Verificamos el estado de ese archivo
    ```bash
    git status

11. Agregamos el archivo unstage
    ```bash
    git add --all  o
    git add -A     o
    git add .

12. Generamos una confirmación o commit para el archivo commands.md
    ```bash
    git commit -m "Creamos el archivo commands.md"

13. sirve para mostrar las diferencias entre archivos en Git, cambios por confirmar, cambios entre commits
    ```bash
    git diff

14. Verificamos el Historial de los todos los commits con autor, fecha, descripción del commits
    ```bash
    git log

15. Para hacer mas comprimidos el historial de todos los commits
    ```bash
    git log --oneline

16. Para Mostrar los commit y la acciones dentro de ellos específicos 
    ```bash
    git log --oneline
    git show 264e719

17. Para saber que esta en staged
    ```bash
    git diff --staged

18. Guarda los cambios no confirmados (sin commit) en una "pila" (stash) y restaura tu área de trabajo al último    commit limpio.
    ```bash
    git stash

19. Verificar todas las pilas o stash
    ```bash
    git stash list

20. Para recuperar los cambios guardados 
    ```bash
    git stash apply stash@{0}

21. Cuando ya no necesitás ninguno de los cambios que habías guardado temporalmente con git stash, y querés limpiar la pila para evitar confusión o liberar espacio., Cuidado que es un comando irreversible
    ```bash
    git stash clear

22. Volver a un commit o revisarlo
Puedes usar el hash de un commit para ir temporalmente a ese punto del tiempo (modo "detached HEAD")
    ```bash
    git checkout 96ecfe2

23. Para cambiar de rama sirve le git checkout 
    ```bash
   git checkout nombre-de-la-rama
   git checkout main 

24. Crear y Cambiar una nueva rama 
    ```bash
    git checkout -b nueva-rama

25. Solo Crear una Rama 
    ```bash
    git branch nueva-rama o 
    git checkout nueva-rama

26. Poder Modificar la descripción de un commit
    ```bash
    git commit --amend -m "Nuevos cambios en el index.html"

27. ¿Qué es Git Flow?
    ```bash
    Git Flow define una serie de ramas principales y ramas de soporte para que el desarrollo sea organizado, predecible y fácil de mantener.
    🔁 Ramas principales
    main (o master):
    Contiene el código en producción.
    Siempre debe estar estable y listo para desplegar.
    develop:
    Contiene el código que está en desarrollo activo.
    Aquí se integran las nuevas funcionalidades antes de pasarlas a main.

28. Ramas de soporte
    ```bash
    feature/nombre:
    Se crean a partir de develop.
    Sirven para trabajar en nuevas funcionalidades.
    Al terminar, se integran a develop.
    git checkout -b feature/login develop

    release/nombre:
    Se crean a partir de develop cuando se quiere preparar una nueva versión.
    Aquí se hacen pruebas, correcciones menores y preparación del despliegue.
    Se fusionan tanto en main como en develop.
    git checkout -b release/v1.0 develop

    hotfix/nombre:
    Se crean a partir de main para arreglar errores críticos en producción.
    Luego se integran tanto en main como en develop.
    git checkout -b hotfix/corregir-login main

29. Creamos Ramas
    ```bash
    git checkout cevasquez-super-rama
    