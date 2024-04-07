# Analyse de sentiment avec l'apprentissage automatique

Ce projet explore diverses techniques d'apprentissage automatique pour l'analyse de sentiment, visant à prédire le ton émotionnel (positif ou négatif) des données textuelles, en particulier les avis des clients d'Amazon.

## Méthodes et technologies:

- **Naive Bayes:** Un classificateur de texte simple mais efficace, connu pour sa rapidité et servant de solide référence.
- **XGBoost:** Une technique avancée renommée pour ses performances élevées dans le traitement des données textuelles clairsemées, ce qui la rend adaptée à une classification détaillée des sentiments.
- **Transformateurs Hugging Face:** Exploite des modèles d'apprentissage profond de pointe pour comprendre le contexte et les nuances du langage, offrant ainsi une profondeur et une précision dans l'analyse des sentiments.

## Données et prétraitement:

Le projet utilise un ensemble de données d'avis clients d'Amazon, en se concentrant sur le texte de l'avis et les évaluations correspondantes. Le nettoyage des données implique de traiter les valeurs manquantes et de garantir l'intégrité des données. Le prétraitement du texte comprend:
- Mise en minuscules
- Suppression des balises HTML et de la ponctuation
- Élimination des mots vides (mots courants avec peu de sens)
- Lemmatisation (réduction des mots à leur forme de base)

La vectorisation TF-IDF transforme les données textuelles en caractéristiques numériques pour l'entraînement du modèle.

## Modélisation et évaluation:

La fonction de modélisation rationalise le processus d'application de différents algorithmes d'apprentissage automatique et d'évaluation de leurs performances. Les modèles sont entraînés sur un ensemble de données équilibré (en utilisant le suréchantillonnage) et évalués à l'aide de mesures telles que le rapport de classification, le score ROC-AUC et la matrice de confusion.

## Résultats et analyse:

- **Naive Bayes:** Fournit une performance de base avec une précision décente.
- **XGBoost:** Atteint une précision plus élevée et démontre son efficacité dans le traitement des données textuelles.
- **Transformateurs Hugging Face:** Offre la précision la plus élevée et capture efficacement les nuances du langage.

## Visualisation:

- Les nuages de mots visualisent les mots les plus fréquemment utilisés dans les avis positifs et négatifs.
- Les diagrammes en barres et les camemberts représentent la répartition des évaluations et des classes de sentiment.
- Les matrices de confusion illustrent la performance des modèles dans la classification des sentiments positifs et négatifs.

## Conclusion:

Ce projet présente l'application de diverses techniques d'apprentissage automatique pour l'analyse de sentiment, démontrant l'efficacité de XGBoost et des Transformateurs Hugging Face pour atteindre une haute précision et comprendre les motifs de langage complexes.

## Travaux futurs:

- Expérimenter avec d'autres architectures d'apprentissage profond et affiner les modèles pré-entraînés.
- Explorer l'analyse de sentiment basée sur les aspects pour identifier le sentiment à l'égard de caractéristiques ou de sujets spécifiques.
- Implémenter les modèles dans une application web pour une analyse de sentiment en temps réel.
