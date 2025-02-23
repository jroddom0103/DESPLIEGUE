# 9 \* Network traffic analysis

## Exercise 9.1

## Create a bash script called ping.sh with the following code,then run it. Press [Ctrl]+[z] to quit the program.

### Crear archivo .sh

![9.1.1 Crear archivo .sh](https://github.com/jroddom0103/DESPLIEGUE/blob/master/Slackware/09_network/Capturas/9.1.1CrearArchivoSH.png)

### Contenido archivo .sh

![9.1.2 Contenido archivo .sh](https://github.com/jroddom0103/DESPLIEGUE/blob/master/Slackware/09_network/Capturas/9.1.2ContenidoSH.png)

Lo que hace el script es hacer ping a cada una de las direcciones IP para
verificar si están activas o no. En otras palabras, para ver los dispositivos
que están conectados a la red.

## Exercise 10.1 User and system information

## Before attempting the questions below, you may wish to deliberately reboot the machine and create some failed

## login attempts so that you have some data to work with.

1. How many login attempts (successful and failed) occurred in the past 48 hours?
   ![10.1.1.1 Logins Exitosos](https://github.com/jroddom0103/DESPLIEGUE/blob/master/Slackware/09_network/Capturas/10.1.1.1LoginsExitosos.png)
   Son 8 logins exitosos.

   ![10.1.1.2 Logins Fallidos](https://github.com/jroddom0103/DESPLIEGUE/blob/master/Slackware/09_network/Capturas/10.1.1.2LoginsFallidos.png)
   Son 13 logins fallidos.
   9 por ssh y 4 por la terminal de la máquina virtual.

2. How many system reboots occurred in the past 48hours?
   ![10.1.2 Reboots](https://github.com/jroddom0103/DESPLIEGUE/blob/master/Slackware/09_network/Capturas/10.1.2Reboots.png)
   6 reinicios.

## Exercise 10.2 Symbolic and hard links

1. Create a file ~/unixstuff/extra_file and a symlink ~/unixstuff/links/extra_file_link which links to extra_file (you may need to create the links directory). Use ls -l whilst in ~/unixstuff/links/ to check that the symlink has been created.
   ![10.2.1 Crear Enlace](https://github.com/jroddom0103/DESPLIEGUE/blob/master/Slackware/09_network/Capturas/10.2.1CrearEnlace.png)

2. Edit extra_file and add some text to it. Now open extra_file_link by executing the following command: cat ~/unixstuff/links/extra_file_link. Do you see the changes you made?

   ![10.2.2 Añadir Contenido Al Enlace](https://github.com/jroddom0103/DESPLIEGUE/blob/master/Slackware/09_network/Capturas/10.2.2AñadirTextoAlEnlace.png)

3. Move extra_file to the backups directory (so its location is now ~/unixstuff/backups/extra_file).

   a) What happens to extra_file_link (if anything)? Hint: try opening the symlink using cat, what is the
   result? Execute ls -l whilst in ~/unixstuff/links/, do you notice anything different?

### No debería de funcionar el enlace.

![10.2.3.a.1 Intentar abrir el fichero](https://github.com/jroddom0103/DESPLIEGUE/blob/master/Slackware/09_network/Capturas/10.2.3.a.1IntentarAbrirArchivo.png)

### No me detecta el archivo, porque ya no está ahí.

![10.2.3.a.2 Enlace en rojo](https://github.com/jroddom0103/DESPLIEGUE/blob/master/Slackware/09_network/Capturas/10.2.3.a.2EnlaceEnRojo.png)

### Me lo pone en rojo, porque ya no está conectado.

b) Move extra_file back to the unixstuff directory – predict what happens to extra_file_link then test
your prediction.

### Que volverá a funcionar.

![10.2.3.b Devolver archivo](https://github.com/jroddom0103/DESPLIEGUE/blob/master/Slackware/09_network/Capturas/10.2.3.bDevolverArchivo.png)

4. Delete extra_file_link. What happens to extra_file (if anything – try opening it using cat)?

   ![10.2.4 Borrar enlace](https://github.com/jroddom0103/DESPLIEGUE/blob/master/Slackware/09_network/Capturas/10.2.4BorrarEnlace.png)

   ### Se puede abrir de forma normal. Porque el enlace es una referencia, no hace falta para que el archivo funcione de forma normal.

5. Recreate the extra_file_link symlink and delete extra_file. What happens to extra_file_link (if anything)?
   See the hint to question 3 (a) if you are stuck.

   ### No va a funcionar, porque el archivo al que hace referencia el enlace ya no existe.

   ![10.2.5 Borrar archivo al que apunta el enlace](https://github.com/jroddom0103/DESPLIEGUE/blob/master/Slackware/09_network/Capturas/10.2.5BorrarArchivoAlQueApuntaEnlace.png)

6. Delete extra_file_link and redo questions 1 – 5 above, but this time use hard links instead. Hence explain
   the differences between symbolic and hard links. You might also wish to do some research to explain why
   you see these differences.

   ![10.2.6 Enlace Fuerte](https://github.com/jroddom0103/DESPLIEGUE/blob/master/Slackware/09_network/Capturas/10.2.4BorrarEnlace.png)

   ### El enlace fuerte, a diferencia del enlace simbólico que apunta hacia la ruta; apunta al inodo, que es un identificador

   ### de los archivos en los sistemas UNIX. Por tanto, presentan el mismo inodo. Es por ello, que aunque se mueva o borre el

   ### archivo original, sigue funcionando.

   ![10.2.6 Mismo identificador](https://github.com/jroddom0103/DESPLIEGUE/blob/master/Slackware/09_network/Capturas/10.2.4BorrarEnlace.png)
