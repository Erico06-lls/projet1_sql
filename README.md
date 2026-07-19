# 📚 Cahier de vacances Machine Learnia - Mes Solutions

Bienvenue dans mon dépôt personnel regroupant mes solutions et expérimentations réalisées dans le cadre du cahier de vacances proposé par [Machine Learnia](https://github.com/MachineLearnia/Cahier-Vacances-2026).

Chaque semaine, un nouveau mini-projet est publié avec pour objectif de pratiquer progressivement différents domaines de la Data Science et de l'Intelligence Artificielle : analyse de données, Machine Learning classique, RAG, graphes, etc.

Ce dépôt me permet de :
- 📝 conserver mes notebooks complétés ;
- 💻 centraliser mon code et mes expérimentations ;
- 📊 documenter mes résultats et mes analyses ;
- 📈 suivre ma progression au fil des projets.

---

# 📂 Structure du dépôt

Chaque projet possède son propre dossier contenant les ressources associées :

- 📓 Notebook complété avec mes solutions ;
- 📁 Données utilisées pour les expérimentations ;
- 📝 Un fichier `README.md` présentant le projet et mes résultats ;
- 🖼️ Les éventuelles images ou visualisations générées.

Structure générale :

```
cahier-de-vacances/
├── Projet_01/
│   ├── projet_01.ipynb
│   └── README.md
│
├── Projet_02/
│   └── ...
│
├── pyproject.toml
└── README.md
```

---

# ⚙️ Configuration de l'environnement

Afin de garder un environnement propre et reproductible pour mes notebooks, ce dépôt utilise un environnement Python isolé géré avec **uv**.

`uv` permet de gérer automatiquement :
- la version de Python utilisée ;
- l'environnement virtuel ;
- les dépendances nécessaires aux différents projets.

---

## 📋 Prérequis

Avant d'utiliser ce dépôt, il est nécessaire d'avoir installé :

- 🐙 **Git**
- 🐍 **Python** (si nécessaire)
- 💻 **VS Code** avec les extensions :
  - 🐍 Python
  - 📓 Jupyter

---

# 🚀 Installation de uv

## 🐧 Linux / macOS / WSL

```shell
curl -LsSf https://astral.sh/uv/install.sh | sh
```

## 🪟 Windows (PowerShell)

```powershell
powershell -ExecutionPolicy ByPass -c "irm https://astral.sh/uv/install.ps1 | iex"
```

Vérification de l'installation :

```shell
uv --version
```

---

# 🏗️ Création de l'environnement virtuel

Depuis la racine du dépôt :

```shell
uv sync
```

Cette commande permet de :

✅ Installer la version de Python configurée dans le projet  
✅ Créer l'environnement virtuel `.venv`  
✅ Installer toutes les dépendances nécessaires  
✅ Préparer l'environnement pour exécuter les notebooks  

---

# 📓 Utilisation avec VS Code

Pour exécuter les notebooks :

1. Ouvrir le dépôt dans VS Code.
2. Ouvrir le notebook du projet souhaité (`.ipynb`).
3. Sélectionner **Select Kernel**.
4. Choisir l'environnement Python situé dans :

```
.venv
```

L'environnement est maintenant prêt pour lancer les cellules de code.

---

# 📦 Ajouter une dépendance

Lorsqu'un projet nécessite une nouvelle bibliothèque Python :

```shell
uv add nom_de_la_bibliothèque
```

Exemple :

```shell
uv add pandas
```

La dépendance sera automatiquement enregistrée dans :

```
pyproject.toml
```

---

# 🔄 Synchroniser l'environnement

Après une modification des dépendances :

```shell
uv sync
```

Cette commande permet de remettre l'environnement en cohérence avec la configuration du projet.

---

# 🔃 Récupérer les nouveaux projets

Le cahier de vacances étant mis à jour régulièrement, les nouveaux projets peuvent être récupérés avec :

```shell
git pull
```

Les nouveaux dossiers seront ajoutés sans modifier les solutions déjà réalisées.

---

# 🚀 Prêt à expérimenter !

L'environnement est maintenant configuré pour continuer mes expérimentations autour de la Data Science et de l'Intelligence Artificielle.

Bon apprentissage et bonnes explorations 🤖📊