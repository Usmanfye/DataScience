# <center>Panongbene Sawadogo</center>

📩 **Contact** : amet1900@gmail.com

🌐 **Linkedin** : [Linkedin Panongbene](https://www.linkedin.com/in/panongbene-jean-mohamed-sawadogo-33234a168/)

🗓️ **Dernière modification** : 14 juillet 2025

# **Exploration et Manipulation des Données Tabulaire avec Python, NumPy et Pandas**

## I. Introduction

Dans un monde de plus en plus guidé par les données, savoir les manipuler efficacement est devenu une compétence essentielle. Que ce soit pour comprendre les tendances d’un marché, évaluer la performance d’une entreprise ou encore analyser des résultats scientifiques, les données tabulaires sont partout. Elles constituent le format le plus couramment utilisé dans l’analyse de données : des feuilles Excel aux bases de données, en passant par les fichiers CSV ou JSON.

Ce cours a été conçu pour vous guider pas à pas dans l’exploration et la manipulation de ces données, à l’aide de **Python**, l’un des langages les plus utilisés en science des données. Vous y découvrirez deux bibliothèques fondamentales :

* **NumPy**, pour le traitement rapide et efficace des tableaux numériques.
* **Pandas**, pour la manipulation intuitive de tableaux étiquetés, comme ceux que l’on retrouve dans les tableurs classiques.

À travers des explications claires, des exemples concrets et un projet pratique, vous apprendrez à :

* Charger des jeux de données à partir de fichiers externes,
* Nettoyer et transformer les données pour les rendre exploitables,
* Explorer et extraire des insights pertinents à partir de vos données,
* Et enfin, exporter vos résultats pour une réutilisation ou une présentation professionnelle.

Ce cours ne nécessite pas de connaissances avancées en programmation, mais une familiarité de base avec Python sera un atout. Il s’adresse aussi bien aux débutants qu’aux professionnels souhaitant renforcer leurs compétences en traitement de données.

## II. Introduction aux Données Tabulaire

### **1. Définition**

Les données tabulaires sont organisées en lignes et en colonnes, similaires à une feuille de calcul ou une table de base de données. Chaque colonne représente une variable, et chaque ligne représente une observation.


|    | Date       | Produit | Catégorie | Quantité | Prix Unitaire (€) | Magasin | Stock Initial | Remise (%) | Vendeur | Client Fidèle |
| -: | ---------- | ------- | --------- | -------- | ----------------- | ------- | ------------- | ---------- | ------- | ------------- |
|  0 | 2024-01-01 | Stylo   | Papeterie | 5        | 0.8               | A       | 50            | 0          | Alice   | True          |
|  1 | 2024-01-02 | Cahier  | Papeterie | 12       | 2.5               | A       | 100           | 5          | Bob     | True          |
|  2 | 2024-01-03 | Gomme   | Papeterie | 7        | 0.6               | B       | 30            | 0          | Alice   | False         |
|  … | …          | …       | …         | …        | …                 | …       | …             | …          | …       | …             |


**Exemples de données tabulaires**

- Fichiers CSV (Comma-Separated Values)
- Feuilles de calcul Excel
- Tables SQL
- Index Elasticsearch

### **2. Pourquoi utiliser Python pour les données tabulaires ?**

Dans le domaine de l’analyse de données, le choix des outils est crucial pour être efficace, rapide et précis. Python s’est imposé comme un langage de référence, notamment pour la manipulation des données tabulaires.

#### **Flexibilité**

Python est un langage **généraliste et polyvalent** qui s’adapte à une grande variété de besoins :

* Il permet de travailler aussi bien sur des petits fichiers locaux (CSV, Excel) que sur des bases de données volumineuses ou des flux en temps réel.
* Python peut gérer différents formats de données (texte, JSON, XML, bases relationnelles, NoSQL, fichiers binaires…).
* Sa syntaxe claire et intuitive facilite la lecture et la maintenance du code, ce qui est important pour manipuler et transformer des jeux de données complexes.
* On peut facilement intégrer Python dans des pipelines d’automatisation, du simple script à des applications web ou des systèmes d’analyse avancés.

#### **Bibliothèques puissantes : NumPy et Pandas**

La force de Python dans le traitement des données vient principalement de ses **bibliothèques spécialisées** :

* **NumPy** fournit une structure de données appelée `ndarray` qui permet de stocker et manipuler efficacement des tableaux numériques multidimensionnels. Ses fonctions vectorisées optimisent les calculs, évitant les boucles lentes en Python natif.

* **Pandas** repose sur NumPy et introduit les objets `Series` et `DataFrame`, conçus spécialement pour les données tabulaires. Pandas propose des outils complets pour :

  * Charger et exporter des données,
  * Nettoyer et filtrer les valeurs manquantes,
  * Sélectionner, transformer et agréger des colonnes,
  * Réaliser des jointures complexes entre tables,
  * Travailler avec des séries temporelles.

Ces bibliothèques sont optimisées, maintenues par une grande communauté, et adaptées à la manipulation de données de taille moyenne à grande.

#### **Connectivité**

Python facilite l’accès à presque toutes les sources de données, ce qui est un atout majeur dans un environnement où les données proviennent souvent de systèmes hétérogènes :

* Connexion aux bases de données relationnelles (MySQL, PostgreSQL, SQLite, SQL Server…) via des bibliothèques comme `SQLAlchemy`, `psycopg2` ou `sqlite3`.
* Accès aux bases NoSQL (MongoDB, Cassandra) et moteurs de recherche comme **Elasticsearch** grâce à des APIs ou bibliothèques dédiées.
* Interaction avec des API REST pour récupérer des données web ou des services cloud.
* Intégration avec des outils Big Data (Hadoop, Spark) via des connecteurs Python.

Cette **interopérabilité** permet de centraliser l’analyse, le traitement et la visualisation des données dans un seul environnement cohérent.

#### **Communauté active et ressources**

Python bénéficie d’une **communauté mondiale très dynamique** autour de la data science :

* Des milliers de développeurs et scientifiques des données contribuent à l’enrichissement des bibliothèques.
* De nombreuses ressources pédagogiques gratuites ou payantes (tutoriels, livres, MOOCs, forums, GitHub).
* Des outils et frameworks complémentaires (Matplotlib, Seaborn pour la visualisation, Scikit-learn pour le machine learning, TensorFlow/PyTorch pour le deep learning) s’intègrent naturellement.
* Un écosystème open source permettant de bénéficier d’améliorations constantes et d’une prise en charge rapide des nouveautés.

Cette communauté facilite la résolution de problèmes, l’apprentissage continu, et garantit la pérennité des projets développés en Python.

## III. Numpy et Pandas

### 1.  Numpy

**NumPy** est une bibliothèque fondamentale pour les calculs numériques en Python. Elle est particulièrement adaptée à la manipulation de tableaux multidimensionnels (arrays).

#### **Installation**
```bash
pip install numpy
```

#### **Concepts de base**
- **Arrays** : Structures de données principales de NumPy, similaires à des listes mais optimisées pour les calculs.
- **Opérations vectorisées** : Permettent d'effectuer des calculs sur des tableaux entiers sans boucles explicites.

#### **Exemple**
```python
import numpy as np

# Créer un array
data = np.array([1, 2, 3, 4, 5])
print("Array:", data)

# Opérations sur l'array
print("Moyenne:", np.mean(data))
print("Somme:", np.sum(data))
print("Carré:", data ** 2)

# Array 2D (matrice)
matrix = np.array([[1, 2, 3], [4, 5, 6]])
print("Matrice:\n", matrix)
print("Transposée:\n", matrix.T)
```

#### Cas pratique : Calculs statistiques
```python
# Générer des données aléatoires
np.random.seed(42)
data = np.random.randn(1000)  # 1000 nombres aléatoires suivant une distribution normale

# Statistiques
print("Moyenne:", np.mean(data))
print("Écart-type:", np.std(data))
print("Valeur max:", np.max(data))
```

### 2. Introduction à Pandas

**Pandas** est une bibliothèque construite sur NumPy, spécialisée dans la manipulation et l'analyse de données tabulaires. Elle introduit deux structures principales : **Series** et **DataFrame**.

#### Installation
```bash
pip install pandas
```

#### Structures de données
- **Series** : Tableau unidimensionnel avec des index.
- **DataFrame** : Tableau bidimensionnel avec des colonnes et des index, similaire à une feuille de calcul.

#### Exemple : Création d'une Series et d'un DataFrame
```python
import pandas as pd

# Créer une Series
s = pd.Series([10, 20, 30, 40], index=['a', 'b', 'c', 'd'])
print("Series:\n", s)

# Créer un DataFrame
data = {
    'Nom': ['Alice', 'Bob', 'Charlie'],
    'Âge': [25, 30, 35],
    'Ville': ['Paris', 'Lyon', 'Marseille']
}
df = pd.DataFrame(data)
print("\nDataFrame:\n", df)
```

---

## IV. Exploration des Données avec Pandas
L'exploration des données consiste à comprendre la structure, le contenu et les caractéristiques des données avant de les manipuler.

### 1. Charger des données
Pandas permet de lire des fichiers de divers formats (CSV, Excel, JSON, etc.).
```python
# Lire un fichier CSV
df = pd.read_csv('exemple.csv')

# Afficher les premières lignes
print(df.head())

# Informations sur le DataFrame
print(df.info())

# Statistiques descriptives
print(df.describe())
```

### 2. Sélection et filtrage
```python
# Sélectionner une colonne
ages = df['Âge']

# Sélectionner plusieurs colonnes
subset = df[['Nom', 'Ville']]

# Filtrer les lignes
adultes = df[df['Âge'] > 30]
print("Adultes:\n", adultes)
```

### 3. Gestion des données manquantes
```python
# Vérifier les valeurs manquantes
print(df.isna().sum())

# Remplacer les valeurs manquantes
df['Âge'] = df['Âge'].fillna(df['Âge'].mean())
```

---

### 4. Lecture de Données à partir de Bases de Données SQL et Elasticsearch
Pandas facilite l'intégration avec des bases de données relationnelles (SQL) et des moteurs de recherche comme Elasticsearch pour charger des données tabulaires.

#### a. Lecture depuis une base de données SQL
Pour lire des données depuis une base de données SQL (comme MySQL, PostgreSQL ou SQLite), nous utilisons la bibliothèque **SQLAlchemy**.

##### Installation
```bash
pip install sqlalchemy
```

##### Exemple : Connexion à une base SQLite
```python
from sqlalchemy import create_engine

# Créer une connexion à une base SQLite (exemple en mémoire)
engine = create_engine('sqlite:///:memory:')

# Supposons une table 'clients' dans la base
# Créer un DataFrame à partir d'une requête SQL
query = "SELECT * FROM clients"
df_sql = pd.read_sql(query, engine)
print("Données SQL:\n", df_sql)

# Alternative : Charger une table entière
df_sql_table = pd.read_sql_table('clients', engine)
print("Table clients:\n", df_sql_table)
```

##### Exemple avec MySQL
```python
# Connexion à une base MySQL
engine = create_engine('mysql+mysqlconnector://user:password@localhost/database_name')

# Lire une requête
df_mysql = pd.read_sql("SELECT nom, age FROM clients WHERE age > 25", engine)
print("Données MySQL:\n", df_mysql)
```

#### b. Lecture depuis Elasticsearch

Pour interagir avec Elasticsearch, nous utilisons la bibliothèque **elasticsearch-py** et l'intégration avec Pandas.

##### Installation
```bash
pip install elasticsearch
```

##### Exemple : Connexion à Elasticsearch
```python
from elasticsearch import Elasticsearch

# Connexion au cluster Elasticsearch
es = Elasticsearch(['http://localhost:9200'])

# Définir une requête pour récupérer des données
query = {
    "query": {
        "match_all": {}
    }
}

# Exécuter la recherche
result = es.search(index='mon_index', body=query, size=1000)

# Convertir les résultats en DataFrame
data = [hit['_source'] for hit in result['hits']['hits']]
df_es = pd.DataFrame(data)
print("Données Elasticsearch:\n", df_es)
```

##### Remarques
- Assurez-vous que le serveur Elasticsearch est en cours d'exécution et accessible.
- La structure des données dans Elasticsearch peut être moins rigide (JSON). Pandas convertit les résultats en colonnes automatiquement.
- Pour des requêtes complexes, utilisez le DSL (Domain Specific Language) d'Elasticsearch.

---

## V. Manipulation des Données avec Pandas

Pandas offre des outils puissants pour transformer et restructurer les données.

#### Ajout et suppression
```python
# Ajouter une nouvelle colonne
df['Âge_plus_10'] = df['Âge'] + 10

# Supprimer une colonne
df = df.drop('Âge_plus_10', axis=1)
```

#### Regroupement et agrégation
```python
# Regrouper par ville et calculer l'âge moyen
age_moyen_ville = df.groupby('Ville')['Âge'].mean()
print("Âge moyen par ville:\n", age_moyen_ville)
```

#### Fusion de DataFrames
```python
# Créer un second DataFrame
data2 = {
    'Ville': ['Paris', 'Lyon', 'Toulouse'],
    'Population': [2161000, 513275, 471941]
}
df2 = pd.DataFrame(data2)

# Fusionner les DataFrames
df_merged = pd.merge(df, df2, on='Ville', how='left')
print("Fusion:\n", df_merged)
```

---

## VI. Cas Pratique
Prenons un exemple avec un jeu de données fictif sur les ventes d'une entreprise.

#### Étape 1 : Charger les données
```python
# Exemple de fichier CSV
data = {
    'Produit': ['Pomme', 'Banane', 'Orange', 'Pomme'],
    'Prix': [1.2, 0.5, 0.8, 1.1],
    'Quantité': [100, 150, 200, 80],
    'Date': ['2023-01-01', '2023-01-01', '2023-01-02', '2023-01-02']
}
df = pd.DataFrame(data)
df.to_csv('ventes.csv', index=False)

# Charger le fichier
df = pd.read_csv('ventes.csv')
```

#### Étape 2 : Exploration
```python
# Résumé statistique
print(df.describe())

# Vérifier les types de données
print(df.dtypes)

# Valeurs uniques dans 'Produit'
print(df['Produit'].unique())
```

#### Étape 3 : Manipulation
```python
# Ajouter une colonne 'Revenu'
df['Revenu'] = df['Prix'] * df['Quantité']

# Regrouper par produit
revenu_par_produit = df.groupby('Produit')['Revenu'].sum()
print("Revenu par produit:\n", revenu_par_produit)
```

## VII. Visualisation des Données
Pour visualiser les données, nous pouvons utiliser **Matplotlib** ou **Seaborn** en complément de Pandas.

#### Installation
```bash
pip install matplotlib seaborn
```

#### Exemple : Graphique
```python
import matplotlib.pyplot as plt
import seaborn as sns

# Graphique en barres
sns.barplot(x='Revenu', y='Produit', data=df.groupby('Produit').sum().reset_index())
plt.title('Revenu par produit')
plt.show()
```

* [*Panongbene*](https://panongbene.com/Menu/Cours%20Ouverts)
---

### **Documentation officielle**

* [NumPy](https://numpy.org/doc/) : Guide complet, tutoriels, références d'API
* [Pandas](https://pandas.pydata.org/docs/) : Guide utilisateur, cookbook, documentation API

---


### **Livres recommandés**

* [*MACHINE LEARNING WITH PYTHON COOKBOOK PATRICAL SOLUTION FROM PREPROCESSING TO DEEP LEARNING*](https://panongbene.com/Menu/Biblioth%C3%A8que/bc641ed79d07381648e8ec142308803e7169189883e8f783f638ab4e1de9b84a) 
* [*INTRODUCTION TO SCIENTIFIC PROGRAMMING WITH PYTHON*](https://panongbene.com/Menu/Biblioth%C3%A8que/b8df40bb8dfb7df49a4cccf04fdf162311e12589bf8d2dc38cdf9300b6bb62b7) 

---

### **Environnements de pratique**

* [Google Colab](https://colab.research.google.com/) – Notebooks Python dans le cloud, gratuit
* [Jupyter Notebook](https://jupyter.org/) – Environnement interactif local
* [Anaconda](https://www.anaconda.com/) – Distribution Python complète pour la data science
