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

<img width="960" height="442" alt="cap3" src="https://github.com/user-attachments/assets/77185b9e-a8d3-4be5-8166-4a22866eaa37" />


<img width="955" height="482" alt="cap1" src="https://github.com/user-attachments/assets/bedceff8-a91d-4109-a54c-88f5f4d11005" />


<img width="958" height="444" alt="CAP2" src="https://github.com/user-attachments/assets/1398d376-f171-4525-a3fc-8281ccf35dbf" />

