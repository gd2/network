
# Détecter les machines de son réseau local

# Un petit éditeur de texte

nano /etc/hosts

# sudo

A revoir :

Pour une connexion de toto en tant que root sans mot de passe à taper il faut éditer/créer sous root le fichier /etc/sudoers.d/10-nopasswd et placer la ligne :

**toto doit être remplacé par le nom de l'utilisateur autorisé à se connecter root sans mot de passe**.

```
toto ALL=(ALL) NOPASSWD: ALL
```

exit pour sortir de sudo.



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
# Authentification ssh par clés

Générer un couple de clés ssh de type rsa
```
ssh-keygen -t rsa 
```
Garder les choix par défaut et pas de passphrase (vide)
micro-1

Copier la clé publique sur la machine à joindre :
```
ssh-copy-id -i ~/.ssh/id_rsa.pub roberto@micro-1
```

Par la suite un ssh roberto@micro-1 se fera sans authentification par mot de passe.

# IA

groq.com

Avec un compte sur groq plus de possibilités sur :

https://console.groq.com/playground

