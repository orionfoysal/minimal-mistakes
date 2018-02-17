# Trasfering Files via SSH

Lets you want to copy a file/folder from **PC-A** to **PC-B** 

* **Install openssh on both computer**

~~~bash
sudo apt install openssh-server openssh-client
~~~

* **Find the Network route of PC-A**
![ ]({{ "/assets/images/route.png" | absolute_url }})

* **Find IP addresses PC-A under that route**
![ ]({{ "/assets/images/ifconfig.png" | absolute_url }})


* **Check if you can login PC-A from PC-B via SSH**
~~~bash
ssh username@ip_address
~~~
Use PC-A username, IP-Address and Password to login. Exit the connection with *logout* command.

* **Now to copy a file from the PC-A  use this command from PC-B terminal**
~~~bash
scp username@ip_address:/home/orion/test.txt .
scp -r username@ip_address:/home/orion/testfolder .
~~~
