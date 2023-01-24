# DT-RN-chapitre2
Source code for INSEE Working Paper on use cases of neural networks with Official Statistics

## Chapitre 2 : Prédire pour imputer
Ce répertoire contient le code produisant les résultats du chapitre 2. Le programme est en **python**, le réseau de neurone est réalisé avec les librairies **Keras** et **Tensorflow**.

Le code exploite des données disponibles uniquement en interne sur les serveurs de calcul de l'Insee (fichiers de production de l'enquête Emploi). Il s'agit d'un notebook jupyter conçu pour être exploitable directement sur les collections rpython et lab.

Le notebook se divise en 5 parties :
1. Un préambule de chargement des packages et fonctions mobilisées
2. La préparation des données: construction de la variable à imputer et des features, traitement des valeurs manquantes et vectorisation des nomenclatures
3. L'entraînement du RN: split train/test, construction du modèle, entraînement, analyse des résultats sur l'échantillon de validation et enregistrement du modèle
4. Prédiction sur l'échantillon test: différentes mesures de performances sur différents échantillons test, prédictions par tranche, résultats sur la population des non-répondants au salaire en clair qui ont répondu par tranche ("véritable" non-réponse)
5. Comparaison avec des modèles linéaires: sur les mêmes inputs que le RN, ou sur des variables plus classiques de modélisation économétrique

