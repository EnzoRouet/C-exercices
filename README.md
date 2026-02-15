# ⚡ C-Programming Mastery - Low-Level Fundamentals

**Dépôt académique** regroupant une série de projets et exercices réalisés en langage C durant mon Bachelor Full Stack.
Ce projet illustre la transition vers la programmation système, mettant l'accent sur la gestion de la mémoire, la manipulation de pointeurs et la structure de fichiers.

## 🎯 Contexte & Objectifs Pédagogiques

Le passage au langage C a été une étape clé pour comprendre les concepts de bas niveau souvent masqués par les langages de plus haut niveau. L'objectif était de construire des outils robustes et de comprendre comment l'ordinateur interagit avec les données brutes.

**Objectifs validés :**

- Maîtrise de la **syntaxe du C** et du typage statique.
- Gestion manuelle de la mémoire et utilisation des **pointeurs**.
- Manipulation de fichiers (Lecture, écriture, calcul de longueur).
- Structuration de données complexes avec les **`struct`**.
- Compilation via **GCC** et compréhension du cycle de vie d'un programme exécutable.

## 🛠️ Stack Technique

- **Langage :** C (Standard C99/C11).
- **Compilation :** GCC (GNU Compiler Collection).
- **Outils :** CLI (Interface en ligne de commande).

## ✨ Focus sur les Projets Réalisés

Le dépôt est organisé par modules fonctionnels, chacun explorant une facette spécifique du langage :

### 1. Mini RPG Engine (Structure & Logique)

Développement d'un moteur de jeu textuel utilisant des structures pour définir les entités (joueurs, monstres) et leurs statistiques.

- **Challenge :** Gérer les combats et l'évolution des états via des passages de paramètres par adresse (pointeurs).

### 2. Gestionnaire d'Annuaire (`gestion_annuaire.c`)

Implémentation d'un système de stockage et de recherche. Ce projet valide la capacité à structurer des données utilisateur et à les manipuler au sein d'un tableau dynamique ou de listes.

### 3. Analyse de Fichiers (`len_file.c`, `counter.c`)

Création d'utilitaires système pour scanner le contenu de fichiers.

- **`len_file` :** Calcul de la taille d'un fichier en octets.
- **`counter_words` :** Algorithme de comptage de mots et de caractères, essentiel pour comprendre la gestion des flux (`FILE*`) et des buffers.

### 4. Manipulation d'Images Brutes (`image.ppm`)

Génération et lecture de fichiers au format PPM. Un exercice parfait pour comprendre comment les couleurs sont représentées par des triplets de données binaires.

## 🏗️ Architecture Technique

Chaque dossier contient son propre fichier source (`main.c` ou équivalent) permettant une compilation isolée.

- Utilisation de la bibliothèque standard (`<stdio.h>`, `<stdlib.h>`, `<string.h>`).
- Focus sur la prévention des fuites de mémoire (Memory Leaks).

## 🧠 Challenges Techniques Résolus

### La rigueur de la gestion des pointeurs

Contrairement au Python, le C demande de gérer explicitement l'emplacement des données en mémoire.

- **Le problème :** Risques de "Segmentation Fault" lors de l'accès à des zones mémoires non allouées.
- **Solution :** Utilisation systématique des adresses mémoire pour modifier les variables à l'intérieur des fonctions, garantissant une empreinte mémoire optimisée.

### Manipulation des Strings (Tableaux de char)

En C, une chaîne de caractères n'est qu'un tableau de caractères se terminant par `\0`.

- **Solution :** Réimplémentation de logiques de parcours de tableaux pour compter les mots ou inverser des chaînes, renforçant la compréhension des index et des terminaisons de fichiers.

## ⚙️ Utilisation

1. **Cloner le projet :**

```bash
git clone [https://github.com/EnzoRouet/C-exercices]
```

2. **Compiler un module :**

```Bash
gcc counter_words.c -o counter
```

3. **Exécuter :**

```Bash
./counter
```
