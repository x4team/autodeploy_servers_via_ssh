# autodeploy_servers_via_ssh


## First you need to install sshpass.

Ubuntu/Debian: ``apt-get install sshpass``
Fedora/CentOS: ``yum install sshpass``
Arch: ``pacman -S sshpass``

**Example:**

```
sshpass -p "YOUR_PASSWORD" ssh -o StrictHostKeyChecking=no YOUR_USERNAME@SOME_SITE.COM
```

**Custom port example:**

```
sshpass -p "YOUR_PASSWORD" ssh -o StrictHostKeyChecking=no YOUR_USERNAME@SOME_SITE.COM:2400
```

Notes:

sshpass can also read a password from a file when the -f flag is passed.
Using -f prevents the password from being visible if the ps command is executed.
The file that the password is stored in should have secure permissions.
