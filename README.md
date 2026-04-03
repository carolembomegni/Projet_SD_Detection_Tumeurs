# Projet_SD_Detection_Tumeurs
# Projet Détection de Tumeurs Cérébrales

##  Description du projet

Ce projet vise à développer un modèle de **classification d’images IRM du cerveau** afin de détecter la présence de tumeurs.

L’objectif principal est de :

* Classifier les images en **Tumor / No Tumor** (classification binaire)
* Améliorer la qualité des images avec des techniques de prétraitement
* Entraîner des modèles de Deep Learning performants

##  Objectifs

* Prétraiter les images (nettoyage, redimensionnement)
* Appliquer des techniques d'amélioration d'image (CLAHE)
* Équilibrer les classes (data augmentation)
* Entraîner plusieurs modèles :

  * CNN simple
  * EfficientNet
  * DenseNet121
  * ResNet50
* Évaluer les performances (accuracy, confusion matrix, etc.)

##  Structure du projet

```
projet-tumeur/
│
├── notebooks/
│   ├── 01_preprocessing.ipynb
│   ├── 02_clahe.ipynb
│   ├── 
│   ├── 04_model_training.ipynb
│   └── 05_evaluation.ipynb
│
├── data_info/
│   └── dataset_description.md
│
├── results/
│   └── figures/
│
├── docs/
│   └── rapport.md
│
└── README.md
```

##  Installation

### 1. Cloner le projet

```bash
git clone https://github.com/carolembomegni/Projet_SD_Detection_Tumeurs.git
cd Projet_SD_Detection_Tumeurs
```
### 2. Installer les dépendances

```bash
pip install tensorflow keras numpy pandas matplotlib opencv-python scikit-learn
```

##  Utilisation

Le projet est principalement développé avec **Google Colab**.

Étapes :

1. Ouvrir les notebooks dans Colab
2. Charger le dataset
3. Exécuter les étapes dans l’ordre :

* Préprocessing
* CLAHE
* (Optionnel) GAN
* Entraînement des modèles
* Évaluation

##  Méthodologie

### 🔹 Prétraitement

* Nettoyage des images
* Redimensionnement (224x224)
* Normalisation

### 🔹 Amélioration des images

* Application de **CLAHE** pour améliorer le contraste

### 🔹 Équilibrage des données

* Data augmentation

### 🔹 Modélisation

* CNN de base
* Transfer Learning :

  * EfficientNetB0
  * DenseNet
  * ResNet50

### 🔹 Évaluation

* Accuracy
* Precision / Recall / F1-score
* Matrice de confusion

##  Résultats attendus

* Amélioration des performances avec CLAHE
* Comparaison entre modèles

##  Équipe

Projet réalisé en groupe (6 personnes) :

* Membre 1 : Préprocessing
* Membre 2 : CLAHE
* Membre 3 : RestNet50
* Membre 4 : Modèle EfficientNet
* Membre 5 : Modèle DenseNet
* Membre 6 : Évaluation & rapport

##  Remarques importantes

* Les images ne sont pas incluses dans le repo (dataset volumineux)
* Utiliser Google Colab avec GPU recommandé
* Attention aux conflits Git sur les fichiers `.ipynb`

##  Technologies utilisées

* Python
* TensorFlow / Keras
* OpenCV
* Scikit-learn
* Google Colab

##  Auteur

Projet réalisé dans le cadre d’un cours en Data Science.
-FRANÇOIS XAVIER GOMSI TESSA
-WILLY STANLIN TAGUEDONG
-CAROLE MBOMEGNI NANA
-LOIC MAMBOU NGANKEU
-THIERRY PASCAL ZOKOU TCHOKONTHE
-ANGELE BLANDINE FEUSSI NGUEMKAM

##  Améliorations possibles

* Optimisation des hyperparamètres
* Utilisation de modèles plus avancés
* Déploiement du modèle (API ou application web)
