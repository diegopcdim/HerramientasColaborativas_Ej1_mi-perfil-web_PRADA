# Crear y saltar a una rama de funcionalidad
git checkout -b feature/habilidades

# Registrar avances en la nueva rama (tras editar archivos)
git add .
git commit -m "feat: añadida sección de habilidades"

# Crear un alias personalizado para borrar ramas (ejercicio de la práctica)
git config --global alias.adios "branch -d"
# Crear y saltar a una rama de funcionalidad
git checkout -b feature/habilidades

# Registrar avances en la nueva rama (tras editar archivos)
git add .
git commit -m "feat: añadida sección de habilidades"

# Crear un alias personalizado para borrar ramas (ejercicio de la práctica)
git config --global alias.adios "branch -d"
# Regreso a la rama principal para correcciones urgentes
git checkout master

# Registro del arreglo (ej. cambio de color en style.css)
git add style.css
git commit -m "fix: corrección de color en el header"

# Subida inmediata de la corrección al servidor
git push origin master
# Traer cambios de master a la rama de trabajo
git checkout feature/habilidades
git merge master

# Provocar la integración en master (donde saltará el conflicto)
git checkout master
git merge feature/habilidades

# Tras editar el archivo para limpiar las marcas (<<<<, ====, >>>>):
git add index.html
git commit -m "Resolución de conflicto: Integración de perfil y tagline"
# Guardar cambios actuales en el área temporal
git stash

# Listar los estados guardados
git stash list

# Recuperar y aplicar los cambios guardados más tarde
git stash pop
# Visualización del historial gráfico y compacto
git log --graph --oneline --all

# Ver diferencias en un archivo modificado antes de confirmar
git diff style.css

# Buscar cuándo se añadió una palabra específica (ej. "Ninja")
git log -S "Ninja"
# Crear etiqueta anotada (v1.0)
git tag -a v1.0 -m "Primera versión oficial del perfil"

# Crear etiqueta ligera (v1.1) tras una mejora estética
git add .
git commit -m "style: mejora de sombras"
git tag v1.1

# Subir todas las etiquetas al servidor GitHub
git push origin --tags

# Viajar en el tiempo a una versión y volver al presente
git checkout v1.0
git checkout main
# 1. Renombrar la rama local master a main
git branch -m master main

# 2. Subir nueva rama y establecer seguimiento (upstream)
git push -u origin main

# 3. Eliminar la rama antigua 'master' en el servidor
git push origin --delete master

# 4. Corregir el último mensaje de commit si es necesario
git commit --amend -m "mensaje corregido"

# 4. Imágenes
![alt text](<img/ej1 1_3_2.png>) ![alt text](<img/ej1 1_3_5.png>) ![alt text](<img/ej1 1_4_5.png>) ![alt text](<img/ej1 1_5_1.png>) ![alt text](<img/ej1 1_6_4.png>) ![alt text](<img/ej1 1_7_5.png>) ![alt text](img/Ej1_1.png)