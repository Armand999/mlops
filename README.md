# mlops

# USE CASE : EVALUATION D'UN MODELE

Ce repository contient un projet utilisant L'apprentissage automatique continu pour la mise en œuvre de l'intégration et du déploiement continues (CI/CD) en mettant l'accent sur les MLOps. 
Lorsqu'une demande d'extraction est effectuée dans ce référentiel, les événements suivants se produisent :
- GitHub déploiera une machine d'exécution avec un environnement d'apprentissage automatique continu Docker spécifié
- L'exécuteur exécutera un workflow pour former un modèle ML (`python train.py`)
- Un rapport visuel d'apprentissage automatique continu sur les performances du modèle sera renvoyé sous forme de commentaire dans la demande d'extraction

Le fichier clé permettant ces actions est `.github/workflows/main.yaml`.

## Secrets and variables environnement 
La seule variable d'environnement définie dans `.github/workflows/main.yaml` est `GITHUB_TOKEN`, qui est configurée par défaut dans chaque référentiel GitHub. Aucun secret ne doit être défini par l'utilisateur. 

# Créer un pipeline CI/CD pour Amazon ECS avec GitHub Actions et AWS CodeBuild Tests
