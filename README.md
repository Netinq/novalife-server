# Image docker pour la création d'un serveur Nova-Life: Ambroise

## Informations générales
L'image tourne à partir d'une image debian 10.9-slim. Elle utilise steamcmd pour installer le serveur de jeu.

## Installation de l'image
### Variables d'environement
`SERVER_NAME` (défaut : "Votre Serveur") : Le nom de votre serveur, qui doit être le même que le nom donné au répertoire dans /Servers/.` 

### Volume
Afin que vous puissiez lancer le serveur correctement, vous devez monter un volume Servers qui pointera vers le dossier `/home/steamuser/novalife/Servers`.
Dans ce volume monté, vous devez créer un dossier qui portera le nom du `SERVER_NAME`.
Dans le dossier `SERVER_NAME`, déposez les fichiers `life.db` et `config.json`.

Vous pouvez ensuite lancer votre image.

# Changelogs
## novalife1.57.1-1.1.0
- Ajout du gracefull shutdown

## novalife1.57.1-1.0.0
- Mise à jour du serveur vers la version 1.57.1 de Nova-Life

## novalife1.57-1.0.0
- Mise à jour du serveur vers la version 1.57 de Nova-Life