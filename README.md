# Curso Git desde cero
Sistema de control de versionnes para el
mantenimiento eficiente y confiable de archivos.

## Zonas de Git
1. Directorio de trabajo
2. Area de Preparacion
3. Directorio Git

## Flujo de trabajo basico en Git
1. Modificas una serie de archivos en tu directorio de trabajo.
2. Preparas los archivos, añadiendolos a tu area de preparacion.
3. Confirmas los cambios, lo que toma los archivos tal y como estan  en el area de preparacion y almacena esa copa instantanea  de manera  permanente en tu directorio de Git.

## Configurando Git por primera vez
```
git config --global user.name "Lukhavi"
git config --global user.email lukhavi@example.com
git config --global core.editor “‘C:\Program Files\Sublime Text 3\subl.exe’ --wait”
git config --local core.editor “‘C:\Program Files\Sublime Text 3\subl.exe’ --wait”
git config --list 
```

## Configuracion SSH en Windows
1. Creamos una carpeta llamada `llaves-ssh` en el disco C para evitar problemas de rutas.

2. Ejecutamos el comando `ssh-keygen -t rsa -C "mi-correo@ejemplo.com"`.
El correo debe ser el mismo con el que nos registramos en GitHub para evitar posibles problemas.
Dejamos el passphrase vacio y damos enter.
Cuando nos pida la ruta escribimos `/c/llaves-ssh/github_rsa`. 

3. Iniciamos ssh-agent en background ejecutando el comando `eval "$(ssh-agent -s)"`.

4. Agregamos la llave ssh generada a ssh-agent ejecutando el comando `ssh-add /c/llaves-ssh/github_rsa`.

5. Desde ahora podemos hacer pull y push sin que GitHub nos este pidiendo los datos de acceso.