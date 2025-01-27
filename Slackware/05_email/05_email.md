# Exercise 6.3 Exploring mail
## You should complete this exercise as bob, not root.
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