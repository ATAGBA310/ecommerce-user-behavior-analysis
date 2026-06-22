# Analyse du comportement utilisateur et de la conversion e-commerce

## Contexte

Dans le secteur du e-commerce, attirer des visiteurs ne suffit pas. L'objectif principal est de comprendre comment les utilisateurs interagissent avec une plateforme afin d'identifier les leviers permettant d'améliorer la conversion.

Ce projet analyse les comportements utilisateurs à partir d'un dataset e-commerce comportant plusieurs centaines de milliers d'événements.

---

## Objectifs

Cette étude vise à répondre aux questions suivantes :

- Comment se répartissent les événements utilisateurs ?
- Où se situent les principales pertes dans le parcours d'achat ?
- Quels produits et catégories performent le mieux ?
- Quels profils utilisateurs sont les plus engagés ?
- Quel est l'impact du prix sur les achats ?

---

## Dataset

Le dataset est composé de 7 fichiers couvrant la période d'octobre 2019 à avril 2020.

Pour des raisons de mémoire, un échantillon de 100 000 lignes a été utilisé pour chaque mois.

Caractéristiques :

- 700 000 événements analysés
- 9 variables étudiées
- 3 types d'événements :
  - view
  - cart
  - purchase

Variables principales :

- event_time
- event_type
- product_id
- category_id
- category_code
- brand
- price
- user_id
- user_session

---

## Technologies utilisées

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Jupyter Notebook

---

## Méthodologie

### 1. Préparation des données

- Analyse des valeurs manquantes
- Remplacement des valeurs manquantes par "unknown"
- Conversion des dates au format datetime
- Création de variables dérivées

### 2. Analyse exploratoire

- Distribution des événements
- Analyse du funnel de conversion
- Analyse produit
- Analyse catégorie
- Analyse utilisateur
- Analyse prix

### 3. Visualisation

- Graphiques de distribution
- Segmentation utilisateur
- Heatmap
- Dashboard final

---

## Résultats principaux

### Funnel de conversion

- 668 576 vues
- 23 318 ajouts au panier
- 8 106 achats

Taux observés :

- View → Cart : 3,49 %
- Cart → Purchase : 34,77 %
- View → Purchase : 1,21 %

Le principal décrochage se situe entre la consultation du produit et l'ajout au panier.

![Funnel](images/funnel.png)

---

### Catégories à fort taux de conversion

L'analyse des catégories montre que certaines catégories convertissent mieux que d'autres malgré un volume de consultation parfois plus faible.

![Category Conversion](images/category_conversion.png)

---

### Segmentation utilisateur

Les utilisateurs ont été segmentés selon leur niveau d'activité :

- LOW : 1 à 5 événements
- MEDIUM : 6 à 20 événements
- HIGH : plus de 20 événements

La majorité des utilisateurs appartient au segment LOW.

![User Segmentation](images/user_segmentation.png)

---

### Dashboard de synthèse

Vue globale du comportement utilisateur, des catégories, de l'activité et des prix.

![Dashboard](images/dashboard.png)

---

## Recommandations métier

À partir des résultats obtenus, plusieurs pistes d'amélioration peuvent être proposées :

- Optimiser les fiches produits
- Améliorer les appels à l'action
- Faciliter l'ajout au panier
- Mettre en avant les catégories les plus performantes
- Réengager les utilisateurs peu actifs
- Fidéliser les utilisateurs fortement engagés

---

## Limites de l'étude

- Échantillon limité à 100 000 lignes par mois
- Certaines anomalies peuvent être dues à l'échantillonnage
- Absence de données démographiques utilisateurs
- Les résultats décrivent des corrélations et non des relations causales

---

## Compétences démontrées

- Data Cleaning
- Exploratory Data Analysis (EDA)
- Funnel Analysis
- User Segmentation
- Data Visualization
- Business Intelligence
- Data Storytelling
- Recommandations métier

---

## Auteur

Abidé TAGBA

Projet réalisé dans le cadre du Master Système d'Information et Management de la Data.