# Prédiction des délais de livraison Olist

Projet d’apprentissage automatique réalisé par Pacôme et Nicolas en FIL A3 à IMT Atlantique, année 2026–2027.

## Objectif

À partir des informations disponibles au moment de l’achat, nous voulons :

- **Estimer le délai réel de livraison** en jours (régression).
- **Prédire le risque de dépasser la date de livraison promise** (classification binaire).

## Données

Olist a publié sur Kaggle environ 100 000 commandes réelles anonymisées, passées au Brésil entre 2016 et 2018. Nous partirons des fichiers sur les commandes, les articles et les clients pour construire une table avec une ligne par commande. Les premières variables incluront le délai promis, le nombre d’articles, le montant des articles, les frais de port et l’État de livraison.

Les deux cibles seront calculées à partir de la date de livraison réelle. L’analyse supervisée portera sur les commandes livrées dont cette date est renseignée.

[Jeu de données original publié par Olist sur Kaggle](https://www.kaggle.com/datasets/olistbr/brazilian-ecommerce)

## Démarche

1. Vérifier les jointures, étudier les valeurs manquantes et explorer les profils de commandes avec du clustering.
2. Comparer des modèles de référence et des modèles d’ensemble pour les deux tâches.
3. Optimiser les hyperparamètres par validation croisée imbriquée et évaluer les modèles sur un jeu de test réservé.

Ce dépôt accueillera le notebook Google Colab et le code de préparation des données.

## Travaux connexes

- [Camille Le Roy, prédiction des retards de livraison avec XGBoost](https://camille-le-roy.github.io/projects/ecommerce_predicting_delivery_delay/)
- [Delivery Delay Prediction, comparaison de modèles de classification sur Olist](https://github.com/fang2544/delivery-delay-prediction)
