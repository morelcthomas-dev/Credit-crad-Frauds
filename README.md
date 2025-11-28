# 🛡️ Détection de Fraude Carte Bancaire — Projet de Machine Learning

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

## 🎯 Objectifs du projet

* Analyser le dataset et comprendre la distribution des transactions légitimes et frauduleuses.
* Traiter le déséquilibre très important des classes (fraudes = minorité).
* Mettre en place un pipeline d’apprentissage supervisé pour prédire les fraudes.
* Entraîner et comparer plusieurs modèles :

  * Régression Logistique
  * Decision Tree Classifier
  * Random Forest Classifier
  * Gradient Boosting Classifier
* Utiliser des métriques adaptées pour un problème déséquilibré :

  * Précision
  * Recall
  * F1-score
  * Matrice de confusion
* Identifier les variables les plus importantes pour le meilleur modèle (Random Forest).
* Fournir une analyse finale des performances et insights.

---

## 🔧 Pipeline du projet

1. **Exploration des données (EDA)**

   * Analyse des colonnes (`info()`, statistiques descriptives)
   * Visualisation de la distribution de la classe
   * Analyse du montant des transactions
   * Vérification des valeurs manquantes

2. **Préparation des données**

   * Séparation X / y
   * Découpage train / test
   * Standardisation éventuelle (ex: Amount)
   * Utilisation de métriques adaptées au déséquilibre des classes

3. **Entraînement des modèles**

   * Logistic Regression
   * Decision Tree Classifier
   * Random Forest Classifier
   * Gradient Boosting Classifier
   * Comparaison des performances via un tableau

4. **Sélection du meilleur modèle**

   * **Random Forest** → meilleur compromis précision / rappel
   * Analyse des importances des variables (V14, V12, V10 ressortent comme essentielles)

---

## 📈 Résultats principaux

* Les modèles simples (LogReg, Decision Tree) donnent des résultats corrects mais limités.
* **Random Forest** → meilleur compromis précision / rappel.
* Gradient Boosting performant mais légèrement inférieur au Random Forest.
* Quelques composantes PCA dominent le signal de fraude.

---

## 📊 Insights importants

* L’**accuracy** seule n’est pas suffisante pour un dataset déséquilibré.
* Le **recall** est clé : mieux vaut détecter plus de fraudes même avec quelques faux positifs.
* Certaines variables anonymisées sont nettement plus importantes que d’autres.
* Random Forest → modèle robuste et interprétable.

---

## 🧪 Technologies utilisées

* Python
* Pandas, NumPy
* Matplotlib, Seaborn
* Scikit-learn
* Jupyter Notebook

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

