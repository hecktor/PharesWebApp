# PharesWebApp

## Prerrequisitos
  Para ejecutar la aplicación se requieren los siguientes componentes
   - Docker
   - Docker-Compose

```sh
sudo apt update && sudo apt install git docker docker-compose
```
Tras haber instalado los paquetes, posteriormente se realizará la instalación de la imagen desde el repositorio de docker

En una Terminal ingresar

```sh

docker pull hiardev/pharesapp

```

Automáticamente empezará la descarga de la aplicación, posteriormente teclearemos "docker images" para obtener la lista de las imagenes que tenemos actualmente

```sh
docker images
```
El resultado se verá algo así 

|REPOSITORY|TAG|IMAGE ID|CREATED|SIZE|
|------|------|-------|------|------|
hiardev/pharesapp|latest|c6b7adc42702|41 minutes ago|483MB|

De esta sección obtendremos el IMAGE ID correspondiente a la imagen hiardev/pharesapp y lo emplearemos para ejecutar el contenedor

```sh
docker run -d -p 8080:80 c6b7adc42702
```
Una vez que haya terminado la ejecución, se podrá acceder desde el navegador con la ruta localhost:8080
 
