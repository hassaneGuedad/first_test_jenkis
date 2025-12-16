# CI/CD Pipeline for Spring Boot with Jenkins & Docker

Ce projet est un exemple de mise en place d'un pipeline CI/CD complet pour une application Spring Boot.

## Objectifs
- **Intégration Continue (CI)** : Compilation et tests automatiques à chaque push.
- **Livraison Continue (CD)** : Création d'une image Docker et déploiement d'un conteneur.

## Architecture du Pipeline
Le pipeline Jenkins est défini dans le fichier `Jenkinsfile` et comprend les étapes suivantes :
1.  **Git Clone** : Récupération du code source depuis GitHub.
2.  **Build** : Compilation avec Maven (`mvn clean install`).
3.  **Docker Build** : Création de l'image Docker de l'application.
4.  **Run** : Lancement automatique du conteneur.

## Prérequis
- Java JDK 17
- Maven
- Docker Desktop
- Jenkins (local)
- Ngrok (pour exposer Jenkins aux Webhooks GitHub)

## Configuration
1.  **Jenkins** : Nécessite le plugin `Maven Integration` et `Docker Pipeline`.
2.  **Webhook** : Configuré sur le dépôt GitHub pour déclencher le build via l'URL Ngrok.

## Auteur
Projet réalisé dans le cadre du TP Jenkins CI/CD.

## Screenshots

<img width="955" height="482" alt="cap1" src="https://github.com/user-attachments/assets/f8dbd50a-f8c1-4bef-ac9e-c976823257b6" />

<img width="955" height="482" alt="cap1" src="https://github.com/user-attachments/assets/5b0e291c-143f-4c70-a910-28a0efe41b8b" />

<img width="958" height="444" alt="CAP2" src="https://github.com/user-attachments/assets/97f7aade-fdfd-40a4-a0d0-e28503c036ca" />

