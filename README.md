# Minikube_TP3

Environnement : Windows 10
Outils : Minikube, kubectl, kompose

Afin de pouvoir utiliser les exe de minikube et kubectl, j'ai tout d'abord créé des Alias qui sont minikube et kubectl avec la commande suivvante : 
 - alias -p nom_alias="./nom_exe" soit : alias -p minikube="./minikube.exe" & alias -p kubectl="./kubectl.exe"
 
 Par la suite on démarre minikube avec la commande start minikube, cela va générer un vm automatiquement.
 
 J'ai ensuite à l'aide de kompose transormé mon fichier docker compose en un fichier de ressource pour kubernetes
 
 Après cela on créer des fichier de deploiement pour le website, la bdd ainsi que minio avec les commandes suivantes :
 - kubectl create -f db-deployment.yaml
 - kubectl create -f website-deployment.yaml 
 - kubectl create -f minio-deployment.yaml
