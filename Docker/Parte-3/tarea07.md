# VOLÚMENES

Iniciamos aqui el tema de la persistencia de datos:

1. Crear los siguientes volúmenes con la orden docker volume: volumen_datos y volumen_web
![](/Capturas/DockerCreate.png)
2. Una vez creados estos contenedores:
    - Arrancar un contenedor llamado c1 sobre la imagen php:7.4-apache que monte el volumen_web en la ruta ***/var/www/html***
    ![](/Capturas/C1.png)
    - Arrancar un contenedor llamado c2 sobre la imagen mariadb que monte el volumen_datos en la ruta ***/var/lib/mysql*** y cuya contraseña de root sea admin.
    ![](/Capturas/C2.png)
3. Parar y borrar el contenedor c2 y tras ello borrar el volumen volumen_datos.
![](/Capturas/BorradoVolumen.png)
## Requisitos
- Grabacion en asciinema