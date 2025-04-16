# Ordonnancement - Théorie des Graphes

## Description

Ce projet consiste à implémenter un programme permettant d’analyser un ensemble de tâches et leurs contraintes de précédence afin d’optimiser leur ordonnancement. L'objectif est de construire un graphe à partir de ces données, d'en vérifier les propriétés, et d'en extraire un calendrier de réalisation optimal incluant les chemins critiques.

---

## Objectifs

- Lire un tableau de contraintes depuis un fichier `.txt`
- Construire un graphe orienté pondéré basé sur les contraintes
- Vérifier l’absence de circuits et de valeurs négatives
- Calculer :
  - Le **rang** de chaque tâche
  - Le **calendrier au plus tôt** et **au plus tard**
  - Les **marges**
  - Le ou les **chemins critiques**
- Afficher graphiquement le graphe
- Générer des **traces d'exécution détaillées**

---

## Structure du projet

### 1. Fichiers principaux

- `main.py` : Programme principal en mode interactif utilisateur
- `main_trace.py` : Version avec génération de **traces détaillées** dans des fichiers `.txt`
- `Graphe.py` : Classe principale contenant tous les traitements liés au graphe, aux calculs et à l’affichage

---

### 2. Répertoires de données

- `Fichiers_Tests/` : Contient les fichiers de contraintes à tester (`table 1.txt`, `table 2.txt`, ...)
- `Fichiers_Traces/` : Contient les fichiers de sortie (traces) générés par `main_trace.py`

---

### 3. Fonctionnalités implémentées

- **Lecture et affichage du tableau de contraintes**
- **Création du graphe** (matrice d'adjacence et matrice de valeurs)
- **Vérification des propriétés du graphe** :
  - Un seul point d’entrée et de sortie
  - Absence de circuits
  - Absence d’arcs à valeurs négatives
- **Calculs** :
  - Rangs des tâches
  - Dates au plus tôt / au plus tard
  - Marges
  - Chemins critiques
- **Affichage graphique** avec `matplotlib` et `networkx`
- **Génération de traces** pas-à-pas (dans `main_trace.py`)

---
