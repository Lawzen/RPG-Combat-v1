# Application de Combat RPG

![RPG Battle](path_to_screenshot.png)

## Table des Matières

- [Introduction](#introduction)
- [Fonctionnalités](#fonctionnalités)
- [Technologies](#technologies)
- [Installation](#installation)
- [Configuration](#configuration)
- [Utilisation](#utilisation)
- [Structure du Projet](#structure-du-projet)
- [Licence](#licence)

## Introduction

Bienvenue dans **l'Application de Combat RPG**, un jeu de rôle dynamique et captivant développé avec **JavaFX** et **Spring Boot**. Cette application permet à deux personnages de s'affronter dans des combats épiques, équipés d'un système de sélection d'armes robuste, de personnalisations d'armures, et de mécaniques de combat stratégiques. De plus, elle utilise une API de skins Minecraft pour personnaliser les têtes des personnages, ajoutant une touche visuelle unique. Que vous soyez un développeur souhaitant explorer les intégrations JavaFX et Spring Boot ou un amateur de jeux cherchant une expérience RPG simple mais divertissante, ce projet a de quoi vous intéresser.

## Fonctionnalités

- **Combat à Deux Joueurs** : Engagez des batailles entre deux personnages personnalisables.
- **Système de Sélection d'Armes** : Choisissez parmi une variété d'armes pour améliorer les capacités de votre personnage.
- **Personnalisation des Armures** : Équipez vos personnages avec différentes armures pour augmenter la défense et modifier l'apparence.
- **Gestion des Personnages** : Créez, modifiez et gérez vos personnages facilement.
- **Scènes Dynamiques** : Interface utilisateur interactive et réactive construite avec JavaFX pour une expérience immersive.
- **Services Backend** : Backend robuste alimenté par Spring Boot pour gérer la logique du jeu et la gestion des données.
- **Configuration JSON** : Configuration et gestion des données simplifiées grâce aux fichiers JSON.
- **API de Skin Minecraft** : Utilisation d'une API de skins Minecraft pour personnaliser les têtes des personnages.

## Technologies

- **Java 17** : Langage de programmation principal utilisé pour le développement.
- **JavaFX** : Pour construire l'interface utilisateur riche et interactive.
- **Spring Boot** : Framework backend pour gérer les services et les dépendances.
- **Maven** : Outil de gestion de projet et d'automatisation de la construction.
- **SQLite** : Base de données légère pour le stockage des données du jeu.
- **JSON** : Pour la configuration et le stockage des données.
- **API de Skin Minecraft** : Pour récupérer et utiliser les skins des personnages.

## Installation

### Prérequis

- **Java Development Kit (JDK) 17** : Assurez-vous que Java est installé sur votre machine. Vous pouvez le télécharger depuis [Oracle](https://www.oracle.com/java/technologies/javase-jdk17-downloads.html) ou [OpenJDK](https://jdk.java.net/17/).
- **Maven** : Installez Maven pour la construction du projet. Téléchargez-le depuis le [Site Officiel de Maven](https://maven.apache.org/download.cgi).
- **Git** : Pour cloner le dépôt. Téléchargez depuis [Git SCM](https://git-scm.com/downloads).

### Étapes

1. **Cloner le Dépôt**

   ```bash
   git clone https://github.com/votreutilisateur/application-rpg-combat.git
   cd application-rpg-combat

2. **Construire le Projet**

   Naviguez vers le répertoire du projet et construisez-le en utilisant Maven :
  
   ```bash
   mvn clean install
   ```
3. **Configurer la Base de Données**

    Assurez-vous que le fichier de configuration JSON est correctement configuré pour utiliser SQLite. Voir la section Configuration pour plus de détails.

4. **Exécuter l'Application**

   Après une construction réussie, exécutez l'application en utilisant Maven :

   ```bash
   mvn spring-boot:run
   Alternativement, vous pouvez exécuter directement le fichier HelloApplication.java depuis votre IDE.

## Utilisation
1. **Lancer l'Application**
   
    Une fois l'application exécutée, la fenêtre principale apparaîtra, présentant des options pour créer ou sélectionner des personnages.

2. **Créer des Personnages**
   
    Naviguez vers la section de création de personnages.
    Personnalisez vos personnages en sélectionnant des attributs, des armes et des armures.

3. **Sélectionner Armes et Armures**
 
    Choisissez parmi un ensemble diversifié d'armes pour améliorer les capacités d'attaque.
    Équipez des armures pour augmenter la défense et modifier l'apparence du personnage.
  
4. **Démarrer le Combat**
 
    Initiez une bataille entre les deux personnages sélectionnés.
    Observez les mécaniques de combat alors que les personnages échangent des attaques jusqu'à ce que l'un d'eux soit victorieux.

5. **Gérer les Personnages**

    Modifiez les personnages existants ou créez-en de nouveaux pour les combats futurs.
    Enregistrez vos configurations en utilisant le système basé sur JSON pour une persistance des données.

   ```bash
   C:.
    │   HelloApplication.java
    │
    ├───arme
    │       Arme.java
    │
    ├───config
    │       JsonConfig.java
    │       LectureJson.java
    │
    ├───controller
    │       ArmeController.java
    │       CombatController.java
    │       DetailArme.java
    │       ModificationPersonnageController.java
    │       PersonnageController.java
    │       SceneController.java
    │
    ├───fx
    │       ArmeListCell.java
    │
    ├───models
    │       Partie.java
    │
    ├───personnage
    │       Personnage.java
    │
    ├───service
    │       ArmeService.java
    │
    └───services
            CombatService.java
            PersonnageService.java

**arme** : Contient les classes liées aux armes.

**config** : Classes de configuration et de gestion des fichiers JSON.

**controller** : Gère les interactions utilisateur et contrôle le flux de l'application.

**fx** : Composants personnalisés JavaFX.

**models** : Modèles de données représentant les entités du jeu.

**personnage** : Classes liées aux personnages.

**service** : Logique métier et services pour les armes.

**services** : Services supplémentaires tels que le combat et la gestion des personnages.


## Licence
Ce projet est sous licence MIT. Vous êtes libre d'utiliser, de modifier et de distribuer ce logiciel conformément aux termes de la licence.


