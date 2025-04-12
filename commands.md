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
    ```
    git diff