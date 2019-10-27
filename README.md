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
--pretty=format:"%h - %an, %ar : %s"
--graph  Con esta opción muestra el historial en gráfica
cdb9608 - Efra Rz, 17 minutes ago : Explicar comando mv
```
Mostrar historial a partir de una fecha determinada
```
git log --after="2019-10-26 19:00" --- Muestra lo que hay después de esta fecha y hora
git log --before="2019-10-26 19:00" --- Muestra lo que hay antes de esta fecha y hora

```

## git diff
Compara directorio de trabajo con el área de preparación.

## .gitignore
Archivos que git ignorará.

## git commit --amend
Comando con el cual podemos modificar el comentario de git más reciente, utilizando el editor preconfigurado.
También sirve por si agregamos más información al último cambio y no queremos hacer un nuevo commit.

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