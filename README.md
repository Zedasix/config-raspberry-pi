# config-raspberry-pi
## Connexion au réseau wifi :
```sudo nano /etc/wpa_supplicant/wpa_supplicant.conf```
```
Country=FR 
network={ 
  ssid=”Wifi Saint Joseph TP” 
  scan_ssid=1 
  psk=”STjO2018BTSSN*” 
key_mgmt=WPA-PSK}
```
## Installation des paquets
### Mise à jour des dépots :
```sudo apt update```
### Installation d'Apache2 :
```sudo apt install apache2 -y``` </br>
Vérifier le fonctionnement dans une navigateur internet sur http://localhost/ ou votre IP. (peut être passé)
### Installation de PHP
```sudo apt install php  -y  ```
Test du PHP (peut être passé)
```
sudo cd /var/www/html 
sudo rm index.html
sudo nano index.php
```
Dans le index.php:
```<?php echo "Bonjour tout le monde"; ?›  ```
On redémarre le service ```sudo service apache2 restart ``` et on retourne sur notre http://localhost/ ou votre IP.
### Installation de MariaDB Server
```
sudo apt install mariadb-server php-mysql  -y
sudo service apache2 restart  
sudo mysql_secure_installation  
```
Faite la config demandé.
### Instalation de de hostapd et dnsmmasq
```sudo apt install hostapd dnsmasq ```
### Installation de PhpMyAdmin
```sudo apt install phpmyadmin  -y  ```
Sélectionne
