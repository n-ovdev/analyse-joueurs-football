# ⚽ Analyse de Données - Joueurs de Football

## 📋 Description

Projet d'analyse de données sur des joueurs de football professionnels réalisé dans le cadre de mon apprentissage en Data Analysis. Ce projet démontre mes compétences en SQL, Python, Pandas et visualisation de données.

## 🎯 Objectifs

- Analyser les caractéristiques des joueurs professionnels
- Nettoyer et préparer les données
- Créer des analyses statistiques pertinentes
- Produire des visualisations claires
- Calculer un score composite de performance

## 🔧 Technologies utilisées

- **Python 3.x**
- **Pandas** : Manipulation et analyse de données
- **Matplotlib** : Création de graphiques
- **Jupyter Notebook** : Environnement de développement
- **SQL** : Requêtes pour extraction de données (équivalent pandas)

## 📊 Dataset

- **Source** : Données de joueurs professionnels
- **Colonnes principales** :
  - `name` : Nom du joueur
  - `age` : Âge
  - `overall` : Note globale
  - `vitesse` : Vitesse
  - `potentiel` : Potentiel du joueur
  - `club_name` : Club
  - `pays` : Pays
  - `salaire` : Salaire

## 🧹 Processus de nettoyage

1. ✅ Vérification des valeurs manquantes
2. ✅ Vérification des doublons
3. ✅ Correction des types de données
4. ✅ Ajout de la colonne `potentiel` calculée
5. ✅ Standardisation des formats

## 📈 Analyses réalisées

### 1. Analyses descriptives
- Top 3 joueurs les plus rapides
- Moyenne overall par club
- Salaire total par pays
- Joueurs explosifs (vitesse >= 90)

### 2. Score composite
Calcul d'un score de performance basé sur :
- Overall (50%)
- Vitesse (30%)
- Potentiel (20%)

### 3. Visualisations
- Top 5 joueurs par overall (bar chart)
- Salaire total par pays (bar chart)
- Relation vitesse vs overall (scatter plot)
- Score composite par joueur

## 📂 Structure du projet
```
projet-football/
│
├── projet_foot.ipynb          # Notebook principal
├── joueurs.csv                # Dataset
├── joueurs_clean.csv          # Données nettoyées
├── top5_overall.png           # Graphique top 5
├── salaire_par_pays.png       # Graphique salaires
├── scatter_vitesse_overall.png # Scatter plot
├── score_composite.png        # Score composite
└── README.md                  # Documentation
```

## 🚀 Installation et utilisation

### Prérequis
```bash
pip install pandas matplotlib jupyter
```

### Exécution
```bash
jupyter notebook projet_foot.ipynb
```

## 📊 Résultats clés

- **Nombre de joueurs analysés** : 7
- **Joueur avec le meilleur overall** : Mbappe
- **Pays avec la plus grande masse salariale** : Espagne
- **Corrélation vitesse/overall** : Positive

## 🎓 Compétences démontrées

- Manipulation de données avec Pandas
- Analyses statistiques (moyennes, groupby, agrégations)
- Création de métriques personnalisées (score composite)
- Visualisation de données
- Nettoyage et préparation de données
- Documentation technique

## 🔄 Équivalent SQL

Les analyses pandas de ce projet peuvent être réalisées en SQL :
```sql
-- Top 3 joueurs les plus rapides
SELECT name, vitesse 
FROM joueurs 
ORDER BY vitesse DESC 
LIMIT 3;

-- Moyenne overall par club
SELECT club_name, AVG(overall) as overall_moyen
FROM joueurs 
GROUP BY club_name;

-- Salaire total par pays
SELECT pays, SUM(salaire) as salaire_total
FROM joueurs 
GROUP BY pays 
ORDER BY salaire_total DESC;
```

## 📧 Contact

**NOAH TONTOLO**
- LinkedIn : NOAH TONTOLO
- Email : noahtontolo@gmail.com
- Portfolio : ComeUp, Fiverr, Malt

## 📝 Licence

Ce projet est libre de droits et à but éducatif.

---

## 🔗 Autres projets

- [Nettoyage de données E-commerce](lien-vers-ton-autre-repo)
