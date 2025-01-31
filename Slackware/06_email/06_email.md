# 6 * Email under Linux

# Exercise 6.1 Sending email using mail
1. Create a file called message.txt with some text, then redirect it to mail using the syntax above to send it to
bob.
![6.1.1.1 Crear mensaje con nano](https://github.com/jroddom0103/DESPLIEGUE/blob/master/Slackware/06_email/Capturas/6.1.1.1CrearMensaje.png)
![6.1.1.2 Escribir mensaje](https://github.com/jroddom0103/DESPLIEGUE/blob/master/Slackware/06_email/Capturas/6.1.1.2EscribirMensaje.png)
![6.1.1.3 Envío del correo](https://github.com/jroddom0103/DESPLIEGUE/blob/master/Slackware/06_email/Capturas/6.1.1.3EnvioCorreo.png)

2. Explain what the following command does:
echo "Welcome to Network Computer Systems" | mail -s "Hello world"
bob@anglia.bryant -c smith@anglia.bryant -b root@anglia.bryant

Mediante echo y la tubería se pasa el mensaje al comando mail, cuyo asunto es Hello world. El destinatario principal es bob@anglia.bryant. Se envía a smith@anglia.bryant, y todos pueden ver que se lo enviaron a él (copia visible). En cambio, a root@anglia.bryant se lo enviaron pero sólo él sabe que se lo pasaron (copia oculta).

# Exercise 6.2 Checking email
Log in as bob (you can execute su bob, then exit when you are finished) and check that all emails sent to bob
are present. If they are not, check that sendmail is running. (If sendmail is not running, the emails are saved in /var/spool/mqueue/ and will be sent once you start the daemon.)
![6.2 Revisión correo Bob](https://github.com/jroddom0103/DESPLIEGUE/blob/master/Slackware/06_email/Capturas/6.2RevisionCorreo.png)

# Exercise 6.3 Exploring mail
## You should complete this exercise as bob, not root.
![6.3.0 Uso de bob y no root](https://github.com/jroddom0103/DESPLIEGUE/blob/master/Slackware/06_email/Capturas/6.3.0CambioBob.png)
1. Describe, using appropriate screenshots, how to do the following in mail: read, reply, send, delete, list and
save messages. Hint: to display help in mail, type [?].

2. What is contained in /var/spool/mail/? What are the security implications of this?
3. From your Windows host machine, telnet to your virtual machine on port 25 (telnet ip_address 25)
and send a message to bob@localhost from your_name @localhost by talking to the SMTP server. The
message body text and subject can be anything you like. Hint: follow the example SMTP session on page
33.
4. Enable POP3. Hint: look in /etc/inetd.conf. Also, you should remember that you need to do something
after saving changes to a configuration file to make those changes take effect... (refer to Lab 4 on page 23)
5. From your Windows host machine, telnet to your virtual machine on port 110. Explore talking to the
POP3 server. Hint: follow the example POP3 session on page 33.
6. What ports are used by SMTP and POP3?

# Exercise 6.4 Optional exercises
1. What is IMAP? List the differences between POP3 and IMAP.
2. What is PGP encryption? How does it work?