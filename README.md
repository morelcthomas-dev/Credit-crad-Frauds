# 🛡️ Détection de fraude par carte bancaire
Analyse de transactions financières afin d’identifier des comportements frauduleux,
avec une approche orientée **contrôle, indicateurs de risque et aide à la décision**.

---

## 🎯 Objectif du projet
Analyser un jeu de données de transactions par carte bancaire afin de :
- détecter des comportements atypiques pouvant indiquer une fraude,
- construire des **indicateurs de risque exploitables**,
- assister les équipes métier dans la prévention et le suivi de la fraude.

La variable cible permet de classer chaque transaction comme :
- `0` → transaction légitime  
- `1` → transaction frauduleuse  

⚠️ Le jeu de données présente un **déséquilibre majeur** : les fraudes représentent une très faible proportion des transactions.

---

## 📊 Données utilisées
- **Time** : secondes écoulées depuis la première transaction  
- **V1 à V28** : variables anonymisées issues d’une ACP (PCA)  
- **Amount** : montant de la transaction  
- **Class** : variable cible (0 = normal, 1 = fraude)  

Source : dataset public Kaggle – Credit Card Fraud Detection.

---

## 🛠️ Outils & technologies
- **Python** : Pandas, NumPy  
- **Visualisation** : Matplotlib, Seaborn  
- **Analyse de données** : statistiques descriptives, analyse exploratoire  
- **Machine Learning** : scikit-learn (modèles de classification)

---

## 🔍 Approche analytique
L’approche adoptée s’inspire des **processus de contrôle et de gestion des risques** :

- Nettoyage et préparation des données
- Analyse exploratoire des comportements transactionnels
- Identification de schémas atypiques :
  - montants élevés,
  - fréquences anormales,
  - répétitions suspectes
- Proposition de **règles de contrôle simples** (seuils, volumes, occurrences)
- Construction d’indicateurs de risque priorisant les transactions à analyser

---

## 🤖 Rôle du machine learning
Des modèles de classification sont utilisés comme **outil d’aide à la décision** afin de :
- prioriser les alertes,
- améliorer la détection des comportements à risque,
- soutenir l’analyse humaine.

Le machine learning **ne constitue pas une décision automatique**, mais un support à la prévention de la fraude.

---

## 📈 Résultats et enseignements
- Différences significatives observées entre transactions normales et frauduleuses
- Identification de variables fortement contributrices au risque
- Création d’indicateurs facilitant la priorisation des contrôles
- Amélioration de la lisibilité des données pour une exploitation opérationnelle

---

## 🚀 Ce que ce projet démontre
- Capacité à analyser des données transactionnelles complexes
- Compréhension des enjeux de **fraude, contrôle et gestion des risques**
- Rigueur analytique et esprit critique
- Utilisation raisonnée du machine learning dans un cadre métier

---

## 📌 Perspectives d’amélioration
- Intégration de règles de contrôle métier supplémentaires
- Enrichissement des indicateurs de risque
- Tests de méthodes complémentaires de détection d’anomalies
- Passage à des volumes de données plus importants

---

## 📥 Jeu de données  
Le dataset utilisé dans ce projet provient du **Bank Marketing Dataset**, disponible publiquement sur Kaggle :  
👉 https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud  

---

## 👤 Auteur

**Thomas Morel** – Data Analyst & Machine Learning Enthusiast

* GitHub : [github.com/morelcthomas-dev](https://github.com/morelcthomas-dev)
* LinkedIn : [linkedin.com/in/thomasmorelcheron](https://www.linkedin.com/in/thomasmorelcheron)

✨ *"Détecter les anomalies pour sécuriser les transactions : le Machine Learning au service de la lutte contre la fraude."*

