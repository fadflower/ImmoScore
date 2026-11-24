# 🏠 ImmoScore MLOps

Projet MLOps collaboratif basé sur le jeu de données [House Prices - Advanced Regression Techniques](https://www.kaggle.com/c/house-prices-advanced-regression-techniques).

## 🎯 Objectif

Passer d'un POC (Proof of Concept) réalisé dans un notebook à un pipeline reproductible, versionné et déployable.

## 📂 Structure du projet

```text
immoscore-mlops/
├── notebooks/          # POC et expérimentations
│   └── house_prices_poc.ipynb
├── data/               # Données brutes (ignorées par Git)
├── models/             # Modèles sérialisés (ignorés par Git)
├── src/                # Code de production (pipeline, utils)
├── README.md
└── .gitignore
```

## 🧪 POC — Étapes pré-MLOps

Le notebook `house_prices_poc.ipynb` réalise :

1. Chargement des bibliothèques
2. Chargement de `train.csv`
3. Filtrage des variables numériques et suppression des lignes incomplètes
4. Séparation X / y (`SalePrice`)
5. Découpe train/test stratifiée par binning de la cible
6. Entraînement d'une régression linéaire
7. Mesure RMSE / R² sur train et test
8. Sauvegarde du modèle dans `model.pkl`
9. Inscription des métriques au tableau de discussion
10. Inscription des versions de `scikit-learn` et `pandas`

## 🛠️ Installation

Cloner le dépôt :

```bash
git clone https://github.com/VOTRE-PSEUDO/immoscore-mlops.git
cd immoscore-mlops
```

Installer les dépendances :

```bash
pip install pandas scikit-learn numpy
```

## 👥 Équipe

| Rôle | Membre GitHub |
|---|---|
| Team Lead | @fadflower |
| Membre | @fadwafa02-a11y |

## 📜 Licence

Projet pédagogique — usage interne.
