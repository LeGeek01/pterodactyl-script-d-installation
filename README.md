# Script d'installation de pterodactyl
Afin d'utiliser ce script correctement, suivez ces quelques étapes simples :
*PS : seul les distributions Linux suivantes sont supportées par ce script : Debian 9, 10 et Ubuntu 18.04, 20.04*

## Préparer votre distribution pour pouvoir exécuter le script.
Exécutez les commandes suivantes selon votre distribution :

Pour Debian et Ubuntu :
```sh
sudo apt-get install curl software-properties-common
curl -sL https://deb.nodesource.com/setup_15.x | sudo bash -
sudo apt-get install nodejs

#Une fois cela exécuté, vérifiez les version de NodeJS et npm avec les commandes suivantes (le résultat doit être le même que celui après le #) :
node -v #15.6.0
npm -v #7.4.0

#Nous allons maintenant télécharger le script :
#Si cela n'est pas déjà fait, vous devez installer wget avec la commande suivante :
sudo apt install wget
```
À ce stade, vote distribution est prête.

## Script pour le panel
Suivez ces commandes pour exécuter le script d'installation du panel :
```sh
mkdir ~/script-installation-ptero-panel-1.4/
cd ~/script-installation-ptero-panel-1.4/

wget https://github.com/LeGeek01/pterodactyl-script-d-installation/releases/latest/download/script-panel.zip
#Si unzip n'est pas installé, installez-le via la commande suivante :
apt install unzip

unzip script-panel.zip

sudo npm install
sudo node index.js
```
**__Le script doit obligatoirement être lancé avec le compte root !__**

## La partie wings arrivera bientôt !
