
# Détecter les machines de son réseau local

# sudo

Le fichier de conf 

```
Pour éviter le mdp


#
# This file MUST be edited with the 'visudo' command as root.
#
# Please consider adding local content in /etc/sudoers.d/ instead of
# directly modifying this file.
#
# See the man page for details on how to write a sudoers file.
#
Defaults	env_reset
Defaults	mail_badpass
Defaults	secure_path="/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin"

# Host alias specification

# User alias specification

# Cmnd alias specification

# User privilege specification
root	ALL=(ALL:ALL) ALL

# Allow members of group sudo to execute any command
%sudo	ALL=NOPASSWD: ALL

# See sudoers(5) for more information on "#include" directives:

#includedir /etc/sudoers.d

```

exit pour sortir de sudo.

# Un petit éditeur de texte

nano /etc/hosts

# /etc/hosts

Correspondances entre IP nom

```
192.168.1.63 dell
192.168.1.20 micro-1

```


# ssh

Commande de base
ssh toto@machine

Option -X pour accepter les fenetres

exit pour quitter ssh

# scp

Comme la commande cp <source> <destination>
```
scp roberto@micro-1:test.txt .
```
Le : signifie le home distant
Le . signifie le répertoire courant

```
scp roberto@micro-1:test.txt  doc.txt
scp essai.txt roberto@micro-1:
```

# IA

groq.com


