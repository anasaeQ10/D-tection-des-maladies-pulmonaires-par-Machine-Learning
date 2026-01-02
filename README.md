# 🫀 Heart Disease Prediction – Data Mining Project

## 📌 Description du projet
Ce projet de **Data Mining** porte sur la **prédiction des maladies cardiovasculaires** à partir de données cliniques réelles.  
L’objectif est de comparer des modèles de **Machine Learning** afin d’identifier le modèle le plus fiable pour détecter la présence d’une maladie cardiaque, un enjeu critique dans le domaine médical.

Le projet est implémenté en **Python** à l’aide d’un **Notebook Jupyter**.

---

## 🎯 Contexte & Objectif
Les maladies cardiovasculaires sont parmi les principales causes de mortalité dans le monde.

🎯 **Objectif principal** :  
> Prédire la présence d’une maladie cardiaque chez un patient à partir de variables cliniques, tout en minimisant les **faux négatifs**, particulièrement critiques en médecine.

---

## 📊 Dataset
- **Source** : Cleveland Heart Disease Dataset  
- **Nombre de patients** : 303  
- **Nombre de variables** : 14  
- **Variable cible** : `target`  
  - `0` : Absence de maladie cardiaque  
  - `1` : Présence de maladie cardiaque  

### Exemples de variables
- `age` : âge
- `sex` : sexe
- `cp` : type de douleur thoracique
- `trestbps` : pression artérielle au repos
- `chol` : cholestérol
- `thalach` : fréquence cardiaque maximale
- `thal`, `ca` : indicateurs cliniques avancés

---

## 🧹 Préparation des données
- Nettoyage des valeurs manquantes  
- Encodage des variables catégorielles  
- Conversion des types de données  
- Standardisation des variables numériques  

---

## 🤖 Modèles de Machine Learning
- **Régression Logistique** (baseline)
- **Random Forest Classifier**

---

## 📈 Résultats

### 🔹 Régression Logistique
- **Accuracy** : 86.9 %
- **Recall (patients malades)** : 93 %
- **Faux négatifs** : 2

### 🔹 Random Forest
- **Accuracy** : 88.5 %
- **Recall (patients malades)** : 96 %
- **Faux négatifs** : 1

---

## ⚖️ Comparaison des modèles
- Random Forest offre de meilleures performances
- Moins de faux négatifs (critique en médecine)
- Modèle plus robuste

📌 **Modèle retenu** : **Random Forest Classifier**

---

## 🔍 Importance des variables
Les variables les plus importantes sont :
- `thalach`
- `cp`
- `thal`
- `ca`
- `age`

Résultats cohérents avec les connaissances médicales.

---

## 🛠️ Technologies utilisées
- Python 3
- Jupyter Notebook
- pandas
- numpy
- matplotlib
- seaborn
- scikit-learn

---

## ▶️ Exécution du projet
```bash
git clone https://github.com/votre-username/heart-disease-prediction.git
cd heart-disease-prediction
jupyter notebook
