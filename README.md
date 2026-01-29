# Plant Disease Detection using CNN

Ce dépôt contient le projet de détection de maladies des plantes utilisant un modèle CNN (Convolutional Neural Network) entraîné sur le dataset "New Plant Diseases Dataset (Augmented)".

## Description

Le projet consiste à entraîner un modèle de classification d'images pour détecter et identifier des maladies sur différentes cultures (pommes, tomates, pommes de terre, raisin, etc.). Les notebooks fournis montrent le prétraitement des images, la définition du modèle, l'entraînement et l'évaluation.

## Structure du dépôt

- `plant_disease_cnn.ipynb` - Notebook principal montrant le pipeline complet (préprocessing, modèle, entraînement et test).
- `plant-disease-detection-using-cnn-model.ipynb` - Notebook alternatif/détaillé avec variations d'architecture et d'hyperparamètres.
- `requirements.txt` - Dépendances Python nécessaires.
- `New Plant Diseases Dataset(Augmented)/` - Dossier du dataset divisé en `train/` et `valid/` (classes par sous-dossier).

## Prérequis

- Python 3.8+ recommandé
- GPU pour accélérer l'entraînement (optionnel mais recommandé)
- Bibliothèques (voir `requirements.txt`)

Installer les dépendances :

```bash
pip install -r requirements.txt
```

## Utilisation

1. Vérifier que le dataset est placé dans `New Plant Diseases Dataset(Augmented)/` avec `train/` et `valid/`.
2. Ouvrir l'un des notebooks (`plant_disease_cnn.ipynb`) dans Jupyter / JupyterLab.
3. Exécuter les cellules de haut en bas :
   - Chargement et augmentation des données
   - Définition du modèle CNN
   - Entraînement
   - Évaluation et visualisation des résultats

## Entraînement (exemple rapide)

- Ajuster les hyperparamètres dans le notebook (batch size, epochs, learning rate).
- Lancer l'entraînement ; sauvegarder le meilleur modèle (checkpoint) sur base de la métrique de validation.

## Évaluation

- Les notebooks incluent des courbes d'entraînement (loss/accuracy) et des matrices de confusion.
- Pour une évaluation hors-notebook, charger le modèle sauvegardé et exécuter l'inférence sur un dossier d'images de test.

## Fichiers importants

- `plant_disease_cnn.ipynb` - pipeline de référence
- `requirements.txt` - dépendances
- `New Plant Diseases Dataset(Augmented)/` - données d'entraînement et validation

## Résultats attendus

- Modèle capable de classifier plusieurs maladies courantes des plantes avec une précision variable selon la classe et les données d'entrainement.
- Visualisations des pertes, de l'accuracy et de la matrice de confusion.

