# Projet Cyber-IDS : Détection d'Intrusions Réseau avec Machine Learning (UNSW-NB15)

## Présentation

Ce dépôt regroupe les travaux réalisés dans le cadre d'un projet de détection d'intrusions réseau basé sur le dataset UNSW-NB15.

L'objectif est de concevoir un modèle de Machine Learning capable d'identifier avec précision les différents types de trafic réseau, qu'ils soient légitimes ou malveillants.

Ce projet sert également de terrain d'entraînement pour l'expérimentation de techniques avancées de Feature Engineering, d'analyse de données et d'optimisation de modèles de classification.

Métrique principale d'évaluation : Accuracy.

---

## Organisation de l'équipe

Le travail a été réparti afin d'accélérer les expérimentations et d'exploiter au mieux les compétences de chaque membre.

### Analyse Exploratoire des Données

Responsabilités :

* Étude de la distribution des classes
* Analyse du déséquilibre entre trafic normal et attaques
* Identification des variables les plus informatives
* Analyse des erreurs de prédiction
* Étude des matrices de confusion

### Feature Engineering

Responsabilités :

* Nettoyage et préparation des données
* Encodage des variables catégorielles
* Création de nouvelles variables discriminantes
* Réduction du bruit dans les données
* Amélioration de la séparation entre les classes

### Machine Learning et Optimisation

Responsabilités :

* Mise en place de la validation croisée
* Gestion du déséquilibre des classes
* Entraînement des modèles
* Optimisation des hyperparamètres
* Génération des fichiers de soumission

Modèles testés :

* CatBoost
* LightGBM
* XGBoost

---

## Structure du projet

```text
Cyber-IDS/
│
├── data/
│   ├── train.csv
│   ├── test.csv
│   └── validation.csv
│
├── notebooks/
│   ├── 1_eda_proportions.ipynb
│   ├── 2_feature_generation.ipynb
│   └── 3_ml_accuracy_opt.ipynb
│
├── src/
│   └── utils.py
│
└── README.md
```

---

## Pipeline de travail

1. Exploration et compréhension des données
2. Nettoyage et préparation des variables
3. Création de nouvelles caractéristiques
4. Validation croisée et expérimentation
5. Optimisation des modèles
6. Génération des prédictions finales
7. Analyse des performances

---

## Technologies utilisées

* Python
* Pandas
* NumPy
* Scikit-Learn
* CatBoost
* LightGBM
* XGBoost
* Matplotlib
* Seaborn
* Jupyter Notebook

---

## Objectifs techniques

* Comprendre les caractéristiques du trafic réseau
* Détecter efficacement les activités malveillantes
* Réduire les erreurs de classification
* Construire un pipeline reproductible
* Améliorer les performances grâce au Feature Engineering
* Comparer plusieurs algorithmes de Machine Learning

---

## Résultats

Les expérimentations portent principalement sur :

* L'impact du Feature Engineering
* La gestion du déséquilibre des classes
* La comparaison entre CatBoost, LightGBM et XGBoost
* L'amélioration progressive de l'Accuracy

Les résultats obtenus et les meilleures configurations seront documentés au fur et à mesure des expérimentations.
