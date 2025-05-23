# INSTALLATION
## cloner le projet
``` git clone https://github.com/Psosv3/workadventure.git ``` 
NB: votre compte github doit être connecté en tant que Patsa sy Ovy

Configurer votre ".env" 


# DOCKER HUB
lancer les commandes suivantes à la racine du projet
 ## se connecter
 ``` docker login ```
 ## builder l'image play localement
 ```docker build -t workadventure-play:latest -f play/Dockerfile .```
 ## initier l'image dans le local (comme git init) 
 ```docker tag workadventure-play:latest onexus/workadventure-play:latest```

 ## pusher l'image sur dockerhub 
 ```docker push onexus/workadventure-play:latest```


# PRODUCTION
d'abord, faire un pull pour le différentes mise à jour
## lancer le projet en production 
 ```docker-compose -f docker-compose-production.yaml up -d```
