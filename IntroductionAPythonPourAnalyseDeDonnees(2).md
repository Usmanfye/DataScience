# **INTRODUCTION À PYTHON POUR L’ANALYSE DE DONNÉES**

## **I. Introduction**  

Aujourd’hui, la maîtrise des outils d’analyse de données est devenue indispensable dans de nombreux domaines, que ce soit en science, en finance, en marketing ou en intelligence artificielle. **Python** s’est imposé comme l’un des langages les plus populaires pour le traitement et l’analyse de données, grâce à sa simplicité, sa flexibilité et sa richesse en bibliothèques spécialisées.  

Ce cours fait partie de la formation [https://panongbene.com/Menu/Formations/e0ef6b91c5d0c1ab8c1620bfde4e7112cf67d95cbb42ca0cedb58ad9f8248de5](PYTHON POUR DATA SCIENTISTS) et vous propose une **initiation pratique à Python** dans le contexte de l’analyse de données. Vous découvrirez les bases du langage, ainsi que les bibliothèques essentielles comme **NumPy** pour le calcul numérique, **Pandas** pour la manipulation de données structurées, et **Matplotlib/Seaborn** pour la visualisation.  

Que vous soyez étudiant, professionnel ou simplement curieux, ce cours vous donnera les **bases solides** pour exploiter Python dans vos projets data. 

Ce cours sert de **fondation** pour utiliser Python dans le domaine de l’analyse de données. Il permet de comprendre les bases du langage, son utilité en Data Science, et comment manipuler efficacement des données grâce à ses structures et fonctions clés.  

---

## **II. Qu’est-ce que Python en Data Analysis ?**  

Python s'est imposé comme **le langage de référence** pour l'analyse de données et la Data Science. Open source, polyvalent et soutenu par une communauté active, Il offre des outils performants pour le traitement, l’analyse et la visualisation de larges volumes de données. 

### **1. Python : Un langage puissant et accessible**  

Python est un **langage interprété, généraliste et polyvalent**, conçu dès ses origines pour être **lisible, concis et accessible**, même aux débutants. Sa syntaxe épurée, proche du langage naturel, le rend **moins verbeux** que des langages comme R, Java ou C++, tout en conservant une grande expressivité.

Il bénéficie d’un **typage dynamique**, ce qui permet d’écrire du code rapidement sans avoir à déclarer explicitement les types de variables, tout en conservant une bonne flexibilité dans la manipulation des données.

Python est un **langage multiplateforme**, compatible avec les principaux systèmes d’exploitation (Windows, macOS, Linux), et peut être exécuté aussi bien en local que sur des environnements cloud. Il s’intègre aisément dans des **workflows variés**, que ce soit pour le scripting, l’automatisation, le traitement de données, le développement web, l’intelligence artificielle ou encore le calcul scientifique.

Grâce à une **communauté très active** et un **écosystème riche en bibliothèques open source** (comme NumPy, Pandas, Matplotlib, Scikit-learn, TensorFlow ou Flask), Python s’est imposé comme un **outil incontournable** dans le domaine de la science des données, de l’IA, et de l’ingénierie logicielle en général.

### **2. Pourquoi Python domine la Data Science ?**  

Python s'est imposé comme le langage le plus populaire dans le milieu de la data science grâce aux facteurs suivants :

**a. Bibliothèques spécialisées** :
Python dispose d’un écosystème de bibliothèques puissantes et matures pour l’analyse, le traitement, la visualisation et la modélisation de données :

* **Pandas** : pour la **manipulation et l’analyse de données tabulaires**, avec ses structures `DataFrame` et `Series` idéales pour nettoyer, transformer et agréger les données.
* **NumPy** : pour le **calcul scientifique et les opérations sur tableaux multidimensionnels**, avec des performances proches du C.
* **Matplotlib/Seaborn** : pour la **visualisation de données**. `Matplotlib` offre une grande flexibilité, tandis que `Seaborn` simplifie la création de visualisations statistiques élégantes.
* **Scikit-learn** : pour le **Machine Learning** : classification, régression, clustering, sélection de modèles, etc. avec une API simple et cohérente.

**b. Simplicité d'apprentissage** :
Par rapport à R, SAS ou même Java, Python est **plus lisible, moins verbeux**, et sa syntaxe intuitive en fait un excellent langage pour les **débutants en programmation ou en data science**.

**c. Écosystème riche et moderne** :
Python s’intègre parfaitement à des environnements interactifs très appréciés des analystes et chercheurs :

* **Jupyter Notebook** : pour créer des notebooks interactifs mêlant code, texte et visualisations.
* **Google Colab** : une alternative cloud gratuite à Jupyter, avec accès GPU/TPU.
* **Anaconda** : distribution Python complète pour la data science, avec gestion de packages et environnements virtuels simplifiée.

**d. Communauté gigantesque et active** :
Grâce à sa **communauté mondiale**, Python bénéficie d’une **documentation abondante**, de milliers de **tutoriels** et d’un support communautaire très réactif (forums, Stack Overflow, GitHub…). Cela facilite la **résolution rapide de problèmes** et l’accès à des solutions éprouvées.

En plus de cela, n'importe qui peut développer une bibliothèque Python et la mettre à disposition des utilisateurs.

**E. Python comme couteau suisse d'accès aux données**  
Python permet de **connecter, importer et exporter** des données depuis presque toutes les sources :  
- **Fichiers locaux** : CSV (`pandas.read_csv`), Excel (`openpyxl`), JSON  
- **Bases de données** : SQL (SQLite, PostgreSQL via `sqlalchemy`), NoSQL  
- **APIs et Web Scraping** : `requests`, `BeautifulSoup`, `Scrapy`  
- **Big Data** : Intégration avec PySpark, Dask  

**Exemple** : **Instagram** est codé en Python,  c’est l’un des langages principaux utilisés par les ingénieurs de chez Google, **Netflix** utilise Python pour l’élaboration de ses algorithmes de recommandation ;

---

## **III. Installer Python via Anaconda**

La manière la plus simple et recommandée pour commencer en Data Science avec Python est d’utiliser la **distribution Anaconda**.

**Anaconda** est une plateforme tout-en-un qui installe :

* **Python** (avec gestion d'environnements virtuels)
* Plus de **250 bibliothèques scientifiques** (Pandas, NumPy, SciPy, etc.)
* Des outils puissants comme **Jupyter Notebook** et **Spyder**
* Un gestionnaire graphique : **Anaconda Navigator**


#### **Sur Windows ou macOS** :

Pour installer Anaconda sur une machine **Windows** ou **macOS** :

1. Rendez-vous sur le site officiel : [https://www.anaconda.com/products/distribution](https://www.anaconda.com/products/distribution)
   
3. Téléchargez l’installeur graphique correspondant à votre système (Windows/macOS).

4. Double-cliquez sur le fichier téléchargé pour lancer l’installation.

5. Lors de l’installation, vous pouvez **conserver les options par défaut**, elles conviennent à la plupart des usages.

6. Une fois l’installation terminée, vérifiez que tout fonctionne en lançant l’application **Jupyter Notebook** (disponible via le menu Anaconda Navigator ou depuis un terminal avec la commande `jupyter notebook`).

#### **Sur Linux** :

Vous pouvez installer Anaconda en ligne de commande. Voici les étapes recommandées :

```bash
cd /tmp
curl -O https://repo.anaconda.com/archive/Anaconda3-5.2.0-Linux-x86_64.sh
sha256sum Anaconda3-5.2.0-Linux-x86_64.sh  # (facultatif mais recommandé)
bash Anaconda3-5.2.0-Linux-x86_64.sh       # Lancer l'installation
source ~/.bashrc                           # Activer Anaconda
```

> Vous pouvez remplacer la version `5.2.0` par une version plus récente disponible sur le site officiel si besoin.

Après installation, testez la commande :

```bash
conda --version
```
pour vérifier que Conda (le gestionnaire d’environnement d’Anaconda) est bien installé.

## **IV. Structures de données essentielles**  

Python fournit des structures de données intégrées très puissantes et faciles à utiliser. Voici les principales à connaître pour toute analyse de données :


### **1. Listes (`list`)**

Une **liste** est une collection ordonnée et **modifiable** d’éléments. Elle peut contenir des types de données variés (entiers, chaînes, listes, etc.).

- **Déclaration et accès**

```python
fruits = ['pomme', 'banane', 'orange']
print(fruits[0])        # 'pomme'
print(fruits[-1])       # 'orange' (index négatif : depuis la fin)
```

- **Slicing**

```python
print(fruits[0:2])      # ['pomme', 'banane']
```

- **Méthodes utiles**

```python
fruits.append('mangue')     # Ajout d'un élément
fruits.remove('banane')     # Suppression d'un élément
fruits.sort()               # Tri
print(fruits)
```

### **2. Dictionnaires (`dict`)**

Les **dictionnaires** permettent de stocker des paires **clé-valeur**. C’est la structure la plus utilisée pour représenter des données **structurées**.

- **Déclaration**

```python
etudiant = {
    'nom': 'Jean',
    'age': 22,
    'note': 16.5
}
```

- **Accès et modification**

```python
print(etudiant['nom'])         # 'Jean'
etudiant['age'] = 23           # Mise à jour
etudiant['classe'] = 'Maths'   # Nouvelle entrée
```

- **Parcours**

```python
for cle, valeur in etudiant.items():
    print(cle, ":", valeur)
```

### **3. Tuples (`tuple`)**

Un **tuple** est comme une liste, mais **immuable** : une fois créé, son contenu ne peut pas être modifié. Très utile pour représenter des données **fixes** ou comme **clés de dictionnaires**.

- **Déclaration**

```python
coordonnees = (45.75, -73.58)
print(coordonnees[0])     # 45.75
```
- **Pourquoi utiliser un tuple ?**

* Pour garantir que les données ne changent pas (ex : coordonnées GPS).
* Meilleure performance que les listes.
* Utilisable comme clé dans un dictionnaire :

```python
eleves = {
    ('Jean', 'Dupont'): 14.5,
    ('Marie', 'Durand'): 17.0
}
```

## **V. Projet pratique : Nettoyage de fichiers CSV simples avec Python**  
- Chargement d’un fichier CSV (`pandas.read_csv`)  
- Exploration des données (`head()`, `info()`, `describe()`)  
- Nettoyage (gestion des valeurs manquantes, filtrage)  
- Export des données nettoyées  


Dans ce projet, nous allons appliquer les bases de l'analyse de données avec la bibliothèque **Pandas**, en travaillant sur un **fichier CSV réel**.

#### **1. Chargement d’un fichier CSV**

On commence par importer Pandas et charger un fichier :

```python
import pandas as pd

# Charger un fichier CSV
df = pd.read_csv('penguins_lter.csv')
```

Vous pouvez aussi charger un fichier en ligne :

```python
url = "/penguins_lter.csv"
df = pd.read_csv(url)
```

#### **2. Exploration des données**

Première inspection pour comprendre la structure du jeu de données :

```python
df.head()        # Affiche les 5 premières lignes
df.tail()        # Les 5 dernières
df.shape         # Dimensions (lignes, colonnes)
df.info()        # Types de colonnes, valeurs nulles
df.describe()    # Statistiques descriptives
df.columns       # Liste des noms de colonnes
```

#### **3. Nettoyage des données**

Le nettoyage est essentiel pour fiabiliser l'analyse.

**a. Gestion des valeurs manquantes**

```python
df.isnull().sum()                # Nombre de valeurs manquantes par colonne
df = df.dropna()                 # Supprimer les lignes contenant des valeurs nulles
# OU
df['Culmen Depth (mm)'].fillna(df['Culmen Depth (mm)'].mean(), inplace=True)   # Remplacer les valeurs nulles par la moyenne
```

**b. Suppression ou renommage de colonnes :**

```python
df = df.drop(columns=['Comments'])
df.rename(columns={'Culmen Length (mm)': 'Culmen_Length_mm'}, inplace=True)
```

**c. Filtrage de lignes :**

```python
df = df[df['Culmen_Length_mm'] >= 10]   # Garder uniquement les élèves avec une note ≥ 10
```

**d. Formatage des données :**

```python
df['Stage'] = df['Stage'].str.upper()   # Nom en majuscules
df['Date Egg'] = pd.to_datetime(df['Date Egg'])  # Conversion en datetime
```

#### **4. Export des données nettoyées**

Après nettoyage, on peut sauvegarder le fichier :

```python
df.to_csv('donnees_nettoyees.csv', index=False)
```

