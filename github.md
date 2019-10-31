## Subir proyecto a repositorio
1. Agregamos repositorio remoto `git remote add origin nombre-direccion-de-repositorio`.
2. Empujamos archivos a el nuevo repositorio con `git push -u origin master`

## Podemos encontrar muchos errores en el camino.
`git config --list --local` comando que muestra las configuraciones de este directorio en particular.

`git checkout -b nombre-rama` comando para crear una nueva rama y saltar automáticamente.

## Pasos para aportar a otro repositorio.

1. Hacer Fork.
2. Clonar Repositorio.
3. Crear Rama local.
4. Realizar cambios a nueva rama local.
5. Confirmar cambios en local.
6. Empujar cambios con el comando. `git push oirgin nombre-rama`.
7. Crear pull request con la nueva rama del repositorio.
8. Esperar a que el administrador del repositorio original acepte cambios.