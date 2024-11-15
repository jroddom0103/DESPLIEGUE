# VOLÚMENES

Iniciamos aqui el tema de la persistencia de datos:

1. Crear los siguientes volúmenes con la orden docker volume: volumen_datos y volumen_web
![](https://github.com/jroddom0103/DESPLIEGUE/blob/master/Docker/Parte-3/Capturas/DockerCreate.png)
2. Una vez creados estos contenedores:
    - Arrancar un contenedor llamado c1 sobre la imagen php:7.4-apache que monte el volumen_web en la ruta ***/var/www/html***
    ![](https://github.com/jroddom0103/DESPLIEGUE/blob/master/Docker/Parte-3/Capturas/C1.png)
    - Arrancar un contenedor llamado c2 sobre la imagen mariadb que monte el volumen_datos en la ruta ***/var/lib/mysql*** y cuya contraseña de root sea admin.
    ![](https://github.com/jroddom0103/DESPLIEGUE/blob/master/Docker/Parte-3/Capturas/C2.png)
3. Parar y borrar el contenedor c2 y tras ello borrar el volumen volumen_datos.
![](https://github.com/jroddom0103/DESPLIEGUE/blob/master/Docker/Parte-3/Capturas/BorradoVolumen.png)
## Requisitos
- Grabacion en asciinema