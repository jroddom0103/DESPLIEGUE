# 04_daemons

# Exercise 4.1 Exploring currently running processes
## Using ps aux and top (and any other commands you feel would be useful), find out the total number of processes that are currently running. Identify the 10 most CPU-intensive processes and give a brief (one sentence) description of what each of them do. Hint: you can use ps aux | less to scroll through the list and man command to find out more about a command.

## 4.1 Uso de PS aux y top para entender procesos
![4.1 Uso de PS aux y top para entender procesos](https://github.com/jroddom0103/DESPLIEGUE/blob/master/Slackware/04_daemons/Capturas/4.1PSAuxTop.png)

- Xorg es un servidor de pantalla de código abierto que implementa el protocolo X11. Es el responsable de mostrar la interfaz gráfica de usuario en la pantalla.
- lxterminal es un emulador de terminal de código abierto que se utiliza para ejecutar comandos en un sistema operativo basado en Linux.
- parcellite es un portapapeles ligero y fácil de usar que se utiliza para copiar y pegar texto en un sistema operativo basado en Linux.
- lxpanel es un panel de escritorio de código abierto que se utiliza para mostrar información sobre el sistema y lanzar aplicaciones en un sistema operativo basado en Linux.
- systemd es un sistema de inicio y administración de servicios de código abierto que se utiliza para controlar los procesos y servicios en un sistema operativo basado en Linux.
- kworker/0:2-eve es un trabajador del kernel de Linux que se utiliza para realizar tareas en segundo plano en un sistema operativo basado en Linux.
- openbox es un gestor de ventanas de código abierto que se utiliza para gestionar las ventanas y la interfaz gráfica de usuario en un sistema operativo basado en Linux.
- pcmanfm es un administrador de archivos de código abierto que se utiliza para navegar por el sistema de archivos en un sistema operativo basado en Linux.
- kworker/1:3-eve es un trabajador del kernel de Linux que se utiliza para realizar tareas en segundo plano en un sistema operativo basado en Linux.

# Exercise 4.2 Exploring network processes
## Execute the command nmap localhost. Write down all the processes returned and explain their purpose

## 4.2 Uso de nmap localhost para explorar procesos de red
![4.2 Uso de nmap localhost para explorar procesos de red](https://github.com/jroddom0103/DESPLIEGUE/blob/master/Slackware/04_daemons/Capturas/4.2NMapLH.png)

- ssh: El protocolo SSH (Secure Shell) es un protocolo de red que se utiliza para acceder de forma segura a un sistema remoto.
- domain: El protocolo DNS (Domain Name System) es un protocolo de red que se utiliza para traducir nombres de dominio en direcciones IP.
- http: El protocolo HTTP (Hypertext Transfer Protocol) es un protocolo de red que se utiliza para transferir datos entre un servidor web y un cliente web.
- ipp: El protocolo IPP (Internet Printing Protocol) es un protocolo de red que se utiliza para imprimir documentos en una impresora de red.

# Exercise 4.3 Exploring UNIX signals
## Execute the command kill -l. Explain what this command does and use a table to summarise the results (signal number, signal name, short description). You only need to consider signal numbers 1 – 9, and five more of your choice between signal numbers 10 and 31. Please remember to cite any sources that you use to answer this exercise using a recognised academic referencing system (see http://libweb.anglia.ac.uk/referencing/referencing.htm).
## 4.3 Uso de kill -l para explorar señales UNIX
![4.3 Uso de kill -l para explorar señales UNIX](https://github.com/jroddom0103/DESPLIEGUE/blob/master/Slackware/04_daemons/Capturas/4.3KillL.png)
