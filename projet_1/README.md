# ✈️ Projet 01 - SQL : Analyse d'une base de réservations de vols

## 📌 Présentation

Ce projet correspond au premier exercice du cahier de vacances proposé par [Machine Learnia](https://github.com/MachineLearnia/Cahier-Vacances-2026).

L'objectif est de se mettre dans la peau d'un analyste travaillant pour un aéroport afin d'exploiter une base de données de réservations de vols et répondre à une problématique métier :

> Quelle destination faut-il renforcer avec un vol supplémentaire, et quels clients cibler en priorité ?

Ce projet m'a permis de pratiquer les bases essentielles de SQL à travers la création, l'interrogation et l'analyse d'une base relationnelle.

---

# 🛠️ Technologies utilisées

- 🐍 **Python**
- 🗄️ **SQLite** pour la gestion de la base de données
- 📊 **Pandas** pour l'affichage et l'analyse des résultats
- 📈 **Matplotlib** pour la visualisation
- 🔎 **SQL** pour l'interrogation des données
- 📓 **Jupyter Notebook** pour l'expérimentation

---

# 🗂️ Structure de la base de données

La base contient trois tables principales :

```
passengers
│
├── id
├── first_name
├── last_name
├── email
└── nationality


flights
│
├── id
├── flight_number
├── origin
├── destination
├── departure_time
├── arrival_time
├── aircraft
├── capacity
└── price_eur


bookings
│
├── id
├── passenger_id
├── flight_id
├── booking_date
├── seat_class
├── seat_number
└── status
```

La table `bookings` joue le rôle de table de liaison entre les passagers et les vols grâce aux clés étrangères.

---

# 📚 Concepts SQL mis en pratique

Durant ce projet, j'ai travaillé sur plusieurs notions importantes :

### 🔹 Création et gestion de bases de données

- Création de tables avec `CREATE TABLE`
- Définition des clés primaires
- Utilisation des clés étrangères (`REFERENCES`)
- Ajout de contraintes (`NOT NULL`, `UNIQUE`, `CHECK`)

### 🔹 Requêtes SQL fondamentales

- `SELECT`
- `WHERE`
- `ORDER BY`
- Filtrage des données

### 🔹 Analyse et agrégation

- `COUNT()`
- `SUM()`
- `AVG()`
- `GROUP BY`
- `HAVING`

### 🔹 Manipulation de plusieurs tables

- `INNER JOIN`
- `LEFT JOIN`

### 🔹 Requêtes avancées

- Sous-requêtes SQL
- Comparaison avec des statistiques globales

---

# 🔎 Analyse réalisée

L'étude a été réalisée en plusieurs étapes :

## 1. Analyse des réservations

J'ai commencé par analyser la répartition des réservations selon leur statut :

- réservations confirmées ;
- réservations annulées ;
- réservations en attente.

Cela permet d'identifier les données réellement exploitables pour l'analyse commerciale.

---

## 2. Analyse du chiffre d'affaires par destination

Les vols ont ensuite été regroupés par destination afin d'identifier les lignes générant le plus de revenus.

Critères étudiés :

- nombre de réservations confirmées ;
- chiffre d'affaires généré ;
- régularité de la demande.

---

## 3. Analyse des clients

Une analyse des passagers a permis d'identifier :

- les clients ayant déjà réservé plusieurs fois ;
- les clients n'ayant encore effectué aucune réservation ;
- le profil des voyageurs sur la destination principale.

---

## 4. Analyse du positionnement prix

Les prix des billets ont été comparés au prix moyen des vols afin de déterminer si les tarifs élevés représentaient un frein ou un positionnement adapté.

---

# 📊 Résultat final

L'analyse montre que la destination recommandée pour l'ajout d'un vol supplémentaire est :

## 🇺🇸 Nice → New York JFK

Cette recommandation repose sur plusieurs observations :

✅ Une forte génération de chiffre d'affaires  
✅ Une demande récurrente avec plusieurs réservations confirmées  
✅ Une clientèle prête à payer des tarifs élevés  
✅ La présence de voyageurs en classes premium (business et first)  

---

# 📈 Visualisation finale

Le projet se termine par une représentation graphique du chiffre d'affaires par destination afin de faciliter l'interprétation des résultats.

*(Ajouter ici une capture du graphique généré si souhaité)*

---

# 📁 Fichiers du projet

```
Projet_01/
│
├── projet_01.ipynb     # Notebook contenant mes solutions SQL
├── README.md           # Présentation du projet
└── images/             # Visualisations éventuelles
```

---

# 🎯 Compétences développées

À travers ce projet, j'ai renforcé mes compétences en :

- manipulation de bases de données relationnelles ;
- écriture de requêtes SQL ;
- analyse exploratoire de données ;
- utilisation de Python avec SQL ;
- transformation d'une question métier en analyse de données.
