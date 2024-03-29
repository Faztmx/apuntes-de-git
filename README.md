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
--oneline  Muestra en una linea
--all Muestra todas las ramas
--decorate 
cdb9608 - Efra Rz, 17 minutes ago : Explicar comando mv
```
Mostrar historial a partir de una fecha determinada
```
git log --after="2019-10-26 19:00" --- Muestra lo que hay después de esta fecha y hora
git log --before="2019-10-26 19:00" --- Muestra lo que hay antes de esta fecha y hora

```
`git log --pretty --oneline --decorate --all --graph` Este comando nos muestra el historial una sola línea por commit.

## git diff
Compara directorio de trabajo con el área de preparación.
`git dif apuntador apuntador`
Muestra diferencia entre los cambios de un commit y otro.

## .gitignore
Archivos que git ignorará.

## git commit --amend
Comando con el cual podemos modificar el comentario de git más reciente, utilizando el editor preconfigurado.
También sirve por si agregamos más información al último cambio y no queremos hacer un nuevo commit.

## git commit -a -m "comentario" (Salta el área de preparación)
Con este comando agregamos y realizamos el commit. Válido para archivos que ya estamos rastreando. Es lo mismo escribir `git commit -am "comentario"`.

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

## git clone
Comando para clonar un repositorio por medio de HTTPS o SSH.
`git clone url`

## git checkout
`git checkout apuntador`
Puedes viajar en la historia del proyecto.
`git checkout master`
Regresas al punto más reciente.

## git tag
Sobre etiquetas, son puntos en la historia que queremos resaltar creando un alias para no tener que escribir completa la suma de comprobación.
1. `git tag nombre-etiqueta` Comando para crear una nueva etiqueta ligera el checksun actual.
2. `git tag` comando para ver las etiquetas creadas.
3. `git tag -a nombre-etiqueta -m` Comando para crear etiquetas anotadas, que basicamente son etiquetas con commits.
4. `git show` comando para mostrar etiqueta o checsum(commit) específico.
5. `git tag -l "v1.*"`Filtrar etiquetas por un patron específico.
6. `git tag nombre-etiqueta checksum` Comando para crear una nueva etiqueta ligera el checksun que elijamos.
## git show
Comando para mostrar etiqueta o checsum(commit) específico.

Esta línea fue creada en la rama master.