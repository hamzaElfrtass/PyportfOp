
# Optimisation de Portefeuille avec les Données de Quandl

Ce Jupyter Notebook démontre comment réaliser une optimisation de portefeuille en utilisant des données boursières obtenues de Quandl. Le notebook couvre le chargement des données, l'analyse exploratoire, le calcul des rendements et l'optimisation de portefeuille en utilisant diverses techniques.

## Installation

Pour exécuter ce notebook, vous devez installer les bibliothèques Python suivantes :

- pandas
- numpy
- matplotlib
- seaborn
- quandl
- scipy

Vous pouvez installer ces bibliothèques en utilisant pip :

```bash
pip install pandas numpy matplotlib seaborn quandl scipy
```

## Données

Les données utilisées dans ce notebook sont obtenues via l'API de Quandl. Les tickers boursiers utilisés sont Apple (AAPL), Amazon (AMZN), Google (GOOGL) et Facebook (FB). La période de temps pour les données va du 1er janvier 2016 au 31 décembre 2017.

## Contenu du Notebook

### 1. Importer les Bibliothèques

La première étape consiste à importer toutes les bibliothèques nécessaires pour la manipulation des données, la visualisation et l'optimisation. Ces bibliothèques incluent `pandas` pour la gestion des données, `numpy` pour les calculs numériques, `matplotlib` et `seaborn` pour les visualisations, `quandl` pour l'accès aux données financières, et `scipy` pour l'optimisation.

### 2. Charger les Données depuis Quandl

Configurer la clé API de Quandl et charger les données boursières pour les tickers spécifiés et la période définie. Les données récupérées incluent les prix de clôture ajustés pour chaque ticker. Cette étape assure que vous avez les données nécessaires pour les analyses suivantes.

### 3. Préparation des Données

Formater les données pour l'analyse en définissant la date comme index et en pivotant les données pour obtenir les prix de clôture ajustés pour chaque ticker. Cela permet de structurer les données de manière appropriée pour les étapes d'analyse et d'optimisation.

### 4. Analyse Exploratoire des Données

Visualiser les prix des actions au fil du temps pour chaque ticker afin de comprendre la tendance générale du marché. Ensuite, calculer les rendements quotidiens des actions, ce qui permet d'évaluer la performance quotidienne des actions et de mesurer la volatilité.

### 5. Optimisation de Portefeuille

Définir des fonctions pour calculer la performance annualisée du portefeuille en termes de rendement et de volatilité. Générer des portefeuilles aléatoires avec différentes allocations d'actifs pour trouver le portefeuille optimal qui maximise le ratio de Sharpe ou minimise la volatilité. Utiliser l'optimisation de scipy pour trouver la meilleure combinaison d'allocations d'actifs.

### 6. Afficher les Résultats

Afficher la frontière efficiente, qui montre les portefeuilles offrant le meilleur rendement pour un niveau de risque donné. Identifier et visualiser les portefeuilles avec le ratio de Sharpe maximum et la volatilité minimale. Ces visualisations aident à comprendre comment différents portefeuilles se comportent en termes de risque et de rendement.

### 7. Conclusion

Ce notebook démontre comment optimiser un portefeuille en utilisant des données boursières de Quandl. En suivant les étapes décrites, vous pouvez analyser les prix historiques des actions, calculer les rendements, et déterminer l'allocation d'actifs optimale pour maximiser les rendements et minimiser les risques. Cette approche peut être appliquée à d'autres ensembles de données et périodes pour des analyses similaires.
