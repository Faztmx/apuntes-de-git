# Curso git desde 0
Sistema de control de versiones para el mantenimiento eficiente y confiable de archivos

## Zonas de git
1. Directorio de trabajo
2. Área de preparación
3. Directorio Git

## Configurando git por primera vez 
```
git config --global user.name "John Doe"
git config --global user.email johndoe@example.com
git config --global core.editor nano
git config --list
```

## git log
Este comando muestra el historial de commits, para salir solamente presionamos la tecla q.
```
git log --pretty=format:"%h - %an, %ar : %s"
cdb9608 - Efra Rz, 17 minutes ago : Explicar comando mv
```

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

## git checkout "nombre de archivo"
Comando para regresar archivos eliminados.

## Pasos para creación de alias
1. 'editor ~/.bashrc'
2. alias nombrealias = 'comando'
3. Reinicia sesión o 'source ~./bashrc'

## git mv
comando para eliminar un archivo de la ubicación vieja y crearlo en una ubicación nueva
```
git mv oldname.ext newname.ext
```
Esto equivale a:
1. `git rm` eliminar el viejo archivo con nombre.
2. `git add` agregar nuevo archivo con nombre.