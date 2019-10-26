# Curso git desde 0
Sistema de control de versiones para el mantenimiento eficiente y confiable de archivos

## Zonas de git
1. Directorio de trabajo
2. Área de preparación
3. Directorio Git

## Configurando git por primera vez 
git config --global user.name "John Doe"
git config --global user.email johndoe@example.com
git config --global core.editor nano
git config --list

## git log
Este comando muestra el historial de commits, para salir solamente presionamos la tecla q.

## git diff
Compara directorio de trabajo con el área de preparación.

## .gitignore
Archivos que git ignorará.

## git commit --amend
Comando con el cual podemos modificar el comentario de git más reciente, utilizando el editor preconfigurado.

## git commit -a -m
Con este comando agregamos y realizamos el commit. Válido para archivos que ya estamos rastreando.

## git rm
Comando que elimina archivos de nuestro repositorio y de nuestro directorio de trabajo.