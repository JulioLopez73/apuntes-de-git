## ¿Qué es Git?
Sistema de control de versiones para el mantenimiento eficiente y confiable de archivos.

### Zonas de Git
1. Directorio de trabajo
2. Area de preparación
3. Directorio Git

### Flujo de trabajo básico en Git
1. Modificas una serie de archivos en tu directorio de trabajo.
2. Preparas los archivos, añadiendolos a tu área de preparación.
3. Confirmas los cambios, lo que toma los archivos tal y como están en el área de preparación y almacena esa copia instantánea de manera permanente en tu directorio de Git.

### Cofigurando Git por primera vez
```
git config --global user.name ""
git config --global user.email 
git config --global core.editor vim
git config --list

```
## Aportes desde otra cuenta
Este texto fue aportado desde la cuenta danielromeroauk

## Varios repositorios remotos
Podemos configurar un mismo proyecto para sincronizar cambios con varios repositorios remotos.

## Configuración SSH
1. Creamos una carpeta llamada `llaves-ssh` en la ruta de nuestro directorio principal de linux
2. Ejecutamos el comando `ssh-keygen -t rsa -C "mi-correo@ejemplo.com"`.
El correo debe de ser el mismo con el que nos registramos en Github para evitar posibles problemas.
Dejamos el passphrase vacío y damos enter.
Cuando nos pida la ruta escribimos `/home/usuario/llaves-ssh/github_rsa`.
3. Iniciamos ssh-agent en background ejecutando el comando `eval "$(ssh-agent -s)"`.
4. Agregamos la llave ssh generada a ssh-agent ejecutando el comando `ssh-add /home/usuario/llaves-ssh/github_rsa`.
5. Usar el comando `cat /home/usuario/llaves-ssh/github_rsa.pub`.
Con este comando vemos el contenido del archivo, copiamos todo el texto que nos muestra.
6. Ir a las configuraciones de nuestro perfil de Github y agregar una nueva llave SSH con el contenido que hemos copiado de `github_rsa.pub`.
