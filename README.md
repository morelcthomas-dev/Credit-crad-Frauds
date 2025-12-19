# 🛡️ Détection de fraude cartes bancaires – Analyse de données et contrôles

## 📌 Présentation du projet

Ce projet vise à analyser un jeu de données de transactions par carte bancaire afin de détecter les fraudes.
L’objectif final est de construire un modèle capable d’identifier si une transaction est :

* **0 → Légitime**
* **1 → Frauduleuse**

Le dataset contient des variables anonymisées (V1 à V28 issues d’une PCA), ainsi que les colonnes **Time** et **Amount**.

---

## 📂 Présentation du jeu de données

* **Time** → secondes écoulées depuis la première transaction
* **V1 à V28** → variables anonymisées issues d’une PCA
* **Amount** → montant de la transaction
* **Class** → variable cible (0 = normal, 1 = fraude)

⚠️ **Déséquilibre majeur :** les fraudes représentent une fraction très faible du dataset.

---

## 🎯 Objectif du projet
Ce projet a pour objectif d’analyser des transactions par carte bancaire afin de :
- détecter des comportements atypiques pouvant indiquer une fraude,
- proposer des règles de contrôle et des indicateurs de risque,
- assister les équipes métier dans la prévention et le suivi de la fraude.

---

## 🛠️ Outils & technologies
- **Python** : Pandas, NumPy, Matplotlib, Seaborn  
- **Machine Learning** : scikit-learn (modèles de classification)  
- **Analyse de données** : statistiques descriptives, analyse exploratoire  

---

## 🔍 Approche analytique et contrôles
L’approche adoptée repose sur une logique proche des processus de contrôle :

- Nettoyage et préparation des données (valeurs manquantes, variables aberrantes)
- Analyse exploratoire des comportements transactionnels
- Identification de schémas atypiques (montants élevés, fréquences anormales)
- Proposition de règles de contrôle simples (seuils, volumes, répétitions)
- Construction d’indicateurs de risque exploitables

---

## 📈 Résultats et enseignements
- Mise en évidence de différences significatives entre transactions normales et frauduleuses
- Identification de variables clés contributrices au risque de fraude
- Création d’indicateurs permettant de prioriser les transactions à analyser
- Amélioration de la lisibilité des données pour une exploitation opérationnelle

---

## 🤖 Utilisation du machine learning
Des modèles de classification ont été utilisés afin d’assister la détection des
transactions potentiellement frauduleuses.

Le machine learning intervient ici comme un **outil complémentaire** permettant :
- de prioriser les alertes,
- d’améliorer la détection des comportements à risque,
- de soutenir l’analyse humaine.

Il ne constitue pas une décision automatique, mais une aide à la prévention de la fraude.

---

## 🧑‍💻 Ce que ce projet démontre
- Capacité à analyser des données transactionnelles complexes
- Compréhension des enjeux de fraude, de contrôle et de gestion des risques
- Rigueur analytique et esprit critique
- Capacité à utiliser des outils de machine learning de manière encadrée et pertinente

---

## 🚀 Perspectives d’amélioration
- Intégration de nouvelles règles de contrôle métier
- Enrichissement des indicateurs de risque
- Tests de méthodes complémentaires de détection d’anomalies
- Adaptation à des volumes de données plus importants

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

