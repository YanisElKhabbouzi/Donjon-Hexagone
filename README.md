# 🏰 Donjon Hexagone

![Java](https://img.shields.io/badge/Java-11%2B-ED8B00?style=flat&logo=java)
![Status](https://img.shields.io/badge/Status-In%20Development-yellow.svg)
![Level](https://img.shields.io/badge/Academic%20Level-2nd%20Year-blue.svg)

---

## 📖 À propos

**Donjon Hexagone** est un jeu **rogue-like en mode texte** développé en **ASCII art**, créé en début de deuxième année d'études informatiques. Ce projet vise à explorer les concepts fondamentaux de la **Programmation Orientée Objet (POO)** tout en développant un jeu interactif et immersif.

Le joueur doit progresser à travers 6 étages remplis de monstres, acquérir des équipements, maîtriser des compétences et affronter des boss redoutables pour terminer son aventure.

### 🎯 Contexte Académique

- **Année d'étude** : Début de 2e année (BAC + 1)
- **Objectif** : Valider les modules de **Programmation Orientée Objet** et de **Conception Logicielle**
- **Méthodologie** : Agile (Sprints de développement itératif)

---

## ✨ Fonctionnalités Clés

### 🎮 Gameplay
- ✅ **Mode roguelike** : Progression à travers 6 étages progressivement complexes
- ✅ **Combat au tour par tour** : Affrontements stratégiques contre des monstres et des boss
- ✅ **Système de classe** : 4 classes jouables avec stats et compétences uniques
  - Guerrier (force brute et endurance)
  - Archer (vitesse et précision)
  - Mage (puissance magique et mana)
  - Voleur (agilité et ruse)

### ⚔️ Mécanique de Jeu
- ✅ **Gestion d'inventaire** : Collecte et utilisation d'équipements et consommables
- ✅ **Système d'équipement** : Armes, armures et accessoires améliorant les stats
- ✅ **Compétences spéciales** : Attaques variées et pouvoirs uniques par classe
- ✅ **Coffres et butin** : Récompenses aléatoires et loot stratégique
- ✅ **Système de sauvegarde** : Persistance de la progression du joueur

### 🎨 Expérience Utilisateur
- ✅ **Interfaces ASCII art** : Menus, cartes, combats et HUD stylisés
- ✅ **Sprites ASCII** : Représentations visuelles des entités et environnements
- ✅ **Gestion dynamique de cartes** : Génération de salles et exploration en temps réel
- ✅ **Dialogues de boss** : Cinématiques narratives avant les affrontements

---

## 🛠️ Technologies & Stack

| Composant | Détails |
|-----------|---------|
| **Langage** | Java 11+ |
| **Paradigme** | Programmation Orientée Objet (POO) |
| **Architecture** | Modèle en couches |
| **Persistance** | Sérialisation Java |
| **Build** | Build manuel (compilation directe) |

---

## 📋 Structure du Projet

```
Donjon-Hexagone/
├── src/main/java/                 # Code source principal
│   ├── Main.java                  # Point d'entrée du jeu
│   ├── Interface.java             # Gestion des interfaces utilisateur
│   ├── ChoixClasse.java          # Sélection des classes
│   ├── Sauvegarde.java           # Système de sauvegarde
│   ├── OutilsDev.java            # Utilitaires de développement
│   ├── carte/                     # Gestion de la carte et des salles
│   ├── classes/                   # Hiérarchie des classes joueur
│   ├── entite/                    # Entités (Joueur, Monstre, Boss)
│   ├── competence/                # Système de compétences
│   ├── equipement/                # Gestion d'équipements
│   ├── consommable/               # Objets consommables
│   └── enums/                     # Énumérations (Stats, Types)
├── res/                           # Ressources du jeu
│   ├── sprites/                   # ASCII art (boss, monstres, interfaces)
│   ├── maps/                      # Cartes des étages (format CSV)
│   ├── interfaces/                # Textes des interfaces
│   ├── dialogue/                  # Dialogues narratifs
│   └── classe/                    # Descriptions des classes
├── doc/                           # Documentation
│   ├── sprint-*/                  # Sprints itératifs (0-9)
│   └── ressource/                 # Burn-up charts et radiateurs
├── bin/                           # Fichiers compilés
└── README.md                      # Ce fichier
```

---

## 🚀 Installation & Utilisation

### Prérequis

- **Java Development Kit (JDK)** version 11 ou supérieure
- **Git** (pour cloner le repository)

### Étapes d'Installation

#### 1️⃣ Cloner le repository

```bash
git clone https://github.com/yourusername/Donjon-Hexagone.git
cd Donjon-Hexagone
```

#### 2️⃣ Compiler le projet

```bash
# Compilation manuelle
javac -d bin/main/java src/main/java/*.java src/main/java/*/*.java

# Ou utiliser un IDE (IntelliJ IDEA, Eclipse, VS Code)
```

#### 3️⃣ Lancer le jeu

```bash
# Via la ligne de commande
cd bin/main/java
java Main

# Ou depuis la racine du projet (selon configuration)
java -cp bin/main/java Main
```

### 🎮 Guide de Jeu

1. **Démarrage** : Le jeu affiche un menu principal avec options
2. **Sélection de classe** : Choisissez parmi 4 classes disponibles
3. **Exploration** : Naviguez dans les étages du donjon
4. **Combat** : Engagez-vous dans des affrontements tactiques
5. **Progression** : Améliorez votre équipement et vos compétences
6. **Boss final** : Affrontez le boss au dernier étage

---

## 📚 Concepts Techniques Validés

Ce projet démontre la maîtrise des concepts suivants :

### 🏗️ Programmation Orientée Objet
- ✅ **Héritage** : Hiérarchie `Entite → Joueur/Monstre/Boss`
- ✅ **Polymorphisme** : Implémentation de méthodes spécialisées
- ✅ **Encapsulation** : Gestion des attributs privés et accesseurs
- ✅ **Abstraction** : Classes abstraites et interfaces

### 🎯 Design Patterns
- ✅ **Factory Pattern** : Création d'entités (monstres, équipements)
- ✅ **Strategy Pattern** : Compétences et types d'attaques
- ✅ **Observer Pattern** : Gestion d'état de jeu

### 🧩 Structures de Données
- ✅ **Collections** : ArrayList, HashMap pour inventaire et statistiques
- ✅ **Sérialisation** : Persistance de sauvegarde
- ✅ **Énumérations** : Types et statistiques structurées

### 🎨 Architecture Logicielle
- ✅ **Séparation des responsabilités** : Logique métier vs présentation
- ✅ **Modulabilité** : Composants indépendants et réutilisables
- ✅ **Maintenabilité** : Code bien structuré et documenté

---

## 📁 Points d'Entrée Importants

| Fichier | Description |
|---------|------------|
| [Main.java](src/main/java/Main.java) | Boucle principale et orchestration du jeu |
| [Interface.java](src/main/java/Interface.java) | Rendu des interfaces utilisateur |
| [Joueur.java](src/main/java/entite/Joueur.java) | Classe représentant le joueur |
| [Monstre.java](src/main/java/entite/Monstre.java) | Classe des ennemis réguliers |
| [Boss.java](src/main/java/entite/Boss.java) | Classe des boss d'étage |
| [Sauvegarde.java](src/main/java/Sauvegarde.java) | Système de persistance |

---

## 📊 Progression Agile

Le projet a été développé en **10 sprints** (Sprint 0 à 9) suivant une méthodologie agile :

- **Sprint Planning** : Définition des user stories et estimation
- **Daily Standups** : Synchronisation d'équipe
- **Sprint Reviews** : Démonstration des livrables
- **Retrospectives** : Amélioration continue (PDCA)

📈 Burn-up charts et radiateurs d'information disponibles dans [`doc/ressource/`](doc/ressource/)

---

## 🤝 Auteurs

- Yanis El Khabbouzi
- Maxence Antoine
- Lony Michaux
- Gaspard Catry
- Andy Samyn
- Antoine Domisse