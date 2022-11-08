# Devoir surveillé

Ce projet est une application spring boot (1.3.1) écrite en Java.

## Travail demandé

### Gitlab

Créer un projet Gitlab public et cloner dessus le projet du DS.

### Dockerfile

Générer un fichier Dockerfile qui doit exécuter l'application:
1) La source doit être une image très légère de openjdk en version 7 et en mode JRE uniquement
2) L'application est déjà compilée et doit être copiée à partir du dossier "target"
3) Le script "run.sh" doit être copié et doit avoir un droit d'accès en exécution.
4) Le port 8080 doit être exposé.
5) La commande de démarrage du container est simplement une exécution de "run.sh"

### Jenkinsfile

Générer un fichier Jenkinsfile qui permet de réaliser les étapes suivates:
1) Auth: s'authentier sur Dockehub
2) Build: créer une image Docker publiable sur Dockerhub
3) Push: mettre l'image nouvellement créée sur Dockerhub
4) CleanUp: se déconnecter de DockerHub et effacer les images Docker locales précedemment créées

## Travail à rendre

Dans Google Classroom, rendre un fichier word avec votre lien DockerHub et votre lien GitLab public contenant le Jenkinsfile et le Dockerfile.
Ajouter aussi les captures d'écrans de l'execution de vos pipelines sur Jenkins.
