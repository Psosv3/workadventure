<!-- lancer le build local pour play -->
 docker build --memory=8g --memory-swap=8g --progress=plain -t workadventure-play:latest -f play/Dockerfile .