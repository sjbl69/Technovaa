# Analyse du turnover – TechNova Partners

Projet réalisé dans le cadre de la formation OpenClassrooms.

## Objectif
Analyser les causes du turnover au sein de l’entreprise TechNova Partners
et construire un modèle de classification permettant d’identifier les employés à risque de départ.

## Données
Trois sources RH :
- sirh.csv
- performance.csv
- survey.csv

Les données sont fusionnées pour constituer un jeu de données central.

## Notebooks
- 01_EDA_and_Cleaning.ipynb : analyse exploratoire et préparation des données
- 02_Modeling_and_SHAP.ipynb : modélisation, évaluation et interprétabilité

## Méthodologie
- Nettoyage et EDA
- Feature engineering
- Modélisation (Dummy, Logistic Regression, RandomForest)
- Gestion du déséquilibre
- SHAP pour l’interprétation

## Environnement
Dépendances gérées avec **uv** (voir `pyproject.toml`).

## Auteur
Selma – Projet OpenClassrooms

