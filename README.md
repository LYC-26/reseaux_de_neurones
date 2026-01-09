# Traduction automatique du Chinois classique vers l’Anglais: Comparaison Pivot vs Direct

Ce projet explore la **traduction automatique neuronale** du chinois
classique vers l'anglais.

## Collaborateurs :

- LIU Yongcan : https://github.com/LYC-26
- ZHUGE Mélanie : https://github.com/XXicheese

## Objectif

Évaluer si la **stratégie par pivot** (via le chinois moderne) surpasse la 
**traduction directe** dans un contexte de forte complexité syntaxique.

## Méthodologie
- Architecture : Transformer.
- Modèles : 
    * `W2M` (chinois classique → chinois moderne)
    * `M2E` (chinois moderne → anglais)
    * `W2E` (chinois classique → anglais)
- Évaluation : Quantitative (BLEU) et Qualitative (Evaluation humaine).

## Fichiers
- `best_w2m.keras` : Modèle chinois classique vers chinois moderne
- `best_m2e.keras` : Modèle chinois moderne vers l’anglais
- `best_w2e.keras` : Modèle chinois classique vers l’anglais
- `pivot_translation.ipynb` : Processus complet d'entraînement des modèles
- `evaluation_humaines.csv` : Résultats de l'évaluation humaine pour 
comparer deux systèmes de traduction
    * `Modèle Pivot` : chinois classique → chinois moderne → anglais
    * `Modèle Direct` : chinois classique → anglais
    > *Note : Deux évaluateurs ont examiné chacun un échantillon aléatoire 
de 10 phrases distinctes (soit 20 phrases au total) avec un score de 1 à 5 
pour calculer la moyenne.*
