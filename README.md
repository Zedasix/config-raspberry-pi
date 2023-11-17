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
Dans le inderx.php:
```<?php echo "Bonjour tout le monde"; ?›  ```
