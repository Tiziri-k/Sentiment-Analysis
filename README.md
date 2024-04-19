# Sentiment-Analysis

# Introduction

Ce projet vise à développer un système capable de prédire les sentiments exprimés dans les textes avec précision, en utilisant des techniques avancées de traitement du langage naturel et d'apprentissage automatique. Le but est d'adapter et d'améliorer continuellement le modèle avec de nouvelles données, en intégrant des techniques d'augmentation des données pour accroître sa capacité à gérer une large variété de textes et améliorer sa généralisation.
Configuration du Projet
Technologies et Bibliothèques Utilisées

    TensorFlow: Utilisé pour les modèles de réseaux de neurones.
    Numpy: Pour les opérations sur les matrices.
    Keras: Pour les modèles de deep learning.
    Scikit-learn: Pour la manipulation et la division des données.
    NLTK: Pour le traitement du langage naturel.
    Tweepy: Pour accéder à l'API Twitter.
    Matplotlib & Seaborn: Pour la visualisation des données.

# Données

Nous avons fusionné trois grands ensembles de données disponibles sur internet :

    Reddit_Data.csv : Sentiments classés en négatif (-1), neutre (0), et positif (1).
    Twitter_Data.csv : Même classification des sentiments.
    Apple-Twitter-Sentiment-DFE.csv : Classification sur une échelle où 1 est négatif, 3 neutre, et 5 positif.

Ces ensembles de données fusionnés offrent une richesse et une variété essentielles pour l'entraînement de notre modèle.
Analyse Exploratoire des Données

    Visualisation : Utilisation de graphiques à secteurs et de nuages de mots pour visualiser la distribution des sentiments et identifier les mots fréquemment associés à chaque catégorie de sentiment.

# Nettoyage et Prétraitement du Texte

    Fonction de Nettoyage : Suppression des éléments non pertinents du texte et standardisation.
    Tokenisation et Elimination des Stopwords : Division en mots et filtration basée sur leur pertinence informative.

# Préparation des Features pour la Modélisation

    Vectorisation du Texte : Conversion des textes nettoyés en séquences numériques, suivie d'un padding pour uniformiser la longueur des entrées.

# Construction et Entraînement des Modèles

    Modèle Word2Vec : Génération de vecteurs de mots pour capturer le contexte sémantique.
    Architecture de Deep Learning : Modèle séquentiel incluant embedding, convolution, LSTM, et dropout.

# Visualisation des Performances

    Évaluation du Modèle : Utilisation de la matrice de confusion pour évaluer les prédictions.
    Graphiques de Performance : Visualisation de l'évolution de la précision et de la perte au fil des époques.

# Amélioration par Augmentation des Données

    Techniques d'Augmentation : Insertion aléatoire de mots, suppression aléatoire, et remplacement par des synonymes pour enrichir notre ensemble de données de 1 000 à 25 000 lignes.

# Évaluation

Analyse détaillée de la matrice de confusion et discussion des améliorations potentielles basées sur les performances du modèle.
