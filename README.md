<h1 style="text-align:center; font-size:42px; margin-top:20px;">
Rapport d'Analyse du paysage technologique 2024 – Stack Overflow Developer Survey
</h1>

## 📌 Présentation du projet

Ce projet propose une **analyse approfondie du paysage technologique mondial en 2024**, basée sur les résultats du **Stack Overflow Developer Survey 2024**.

L’objectif est de :

- comprendre le **profil des développeurs**
- analyser l’**usage**, la **demande** et la **rémunération** des technologies
- explorer l’**écosystème technologique global** (langages, frameworks, bases de données, plateformes, outils)

Le projet est implémenté sous **Power BI**, avec un **modèle analytique structuré** et des **visualisations interactives**.

---

## 📊 Pages du rapport & axes d’analyse

### 1️⃣ Profil global des développeurs

Cette page met en évidence les caractéristiques démographiques et professionnelles des répondants :

- répartition géographique des développeurs
- niveau d’expérience (*junior / senior / débutant*)
- niveau d’éducation
- rôle principal dans le développement
- distribution de la satisfaction professionnelle

👉 **Objectif :** contextualiser les tendances technologiques par le profil des répondants.

---

### 2️⃣ Langages de programmation

Analyse comparative des langages:

- langages les plus utilisés
- langages les plus demandés
- langages les mieux rémunérés (*salaire moyen*)
- usage dominant par tranche d’âge
- adoption par secteur d’activité

👉 **Objectif :** mettre en évidence les écarts entre **popularité**, **demande marché** et **rémunération**.

---

### 3️⃣ Écosystème technologique

Vue globale des outils et plateformes utilisés par les développeurs :

- bases de données
- frameworks web
- systèmes d’exploitation
- plateformes cloud
- outils collaboratifs et IDE
- usages liés à l’IA

👉 **Objectif :** comprendre l’environnement technologique réel des développeurs en 2024.

---

## 🧩 Dataset & pipeline de données

Le projet s’appuie sur une version **nettoyée et préparée** du **Stack Overflow Developer Survey 2024**, issue d’un travail préalable réalisé en **Python**.

- **Dataset final :** `survey-data_V3_final.csv`
- **Source GitHub :**  
  https://github.com/salma91AFG/Technology-Trends-Analytics/blob/main/Data/Survey/processed

Le chargement des données dans Power BI est réalisé **via un script Python**, directement depuis GitHub.

---

## 🏗️ Modélisation des données

Le modèle Power BI repose sur :

- une **table source unique**
- plusieurs **tables de faits** (*usage, souhaits, plateformes, salaires, etc.*)
- des **tables de dimensions** (*respondant, langages*)

Les tables intermédiaires servant de références sont **désactivées du chargement** afin d’optimiser :

- la **taille du modèle**
- les **performances**
- la **lisibilité du schéma**

Le modèle suit une **approche en étoile**, adaptée à l’analyse BI.

---

## 📐 Mesures & logique analytique

L’analyse repose exclusivement sur des **mesures DAX**, sans multiplication inutile de **colonnes calculées**.

Les mesures permettent notamment de :

- calculer des **pourcentages d’utilisation** (*par langage, outil, plateforme*)
- agréger des **salaires moyens** selon différents axes
- comparer **usage vs demande**
- neutraliser certains filtres pour obtenir des **valeurs globales cohérentes**
- garantir la **cohérence des indicateurs** sur l’ensemble des pages

👉 Les mesures sont conçues pour être **réutilisables**, **robustes au contexte de filtre** et **alignées avec le modèle relationnel**.

*(Le code DAX n’est pas détaillé dans le README afin de préserver la lisibilité, mais il est disponible dans le fichier Power BI.)*

---

## ⚙️ Outils & technologies

- **Power BI Desktop**
- **DAX** (*mesures analytiques*)
- **Python** (*préparation amont + chargement des données*)
- **GitHub** (*versioning et documentation*)

---

## 🎯 Points clés du projet

- **Pipeline analytique complet** (*Python → Power BI*)
- **Modélisation BI structurée**
- **Utilisation avancée du contexte de filtre**
- **Analyse orientée marché & décision**
- **Rapport interactif** pensé pour un public non technique

---

## 👤 Auteur

**Salma Djaid – Data Analyst**  
Conception du pipeline, nettoyage, EDA, visualisations et recommandations.
