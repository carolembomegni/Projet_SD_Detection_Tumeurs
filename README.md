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

#  Projet de detection des tumeurs cerebrales

##  Description du projet

Ce projet vise à développer un modèle de **classification d’images IRM du cerveau** afin de détecter la présence de tumeurs.

L’objectif principal est de :

* Classifier les images en **Tumor / No Tumor** (classification binaire)
* Améliorer la qualité des images avec des techniques de prétraitement
* Entraîner des modèles de Deep Learning performants
* Deployer la solution

---

##  Objectifs

* Prétraiter les images (nettoyage, redimensionnement)
* Appliquer des techniques d'amélioration d'image (CLAHE)
* Équilibrer les classes (data augmentation / GAN)
* Entraîner plusieurs modèles :

  * CNN simple
  * DenseNet
  * Resnet50
  * EfficientNet
  * VGG16
* Évaluer les performances (accuracy, confusion matrix, etc.)
* Deployer le modele

---

## Structure du projet

```
## Structure du projet

```text
projet-tumeur/
│
├── notebooks/
│   ├── 00_importation_dataset.ipynb
│   ├── 01_preprocessing.ipynb
│   ├── 02_creation_binaire.ipynb
│   ├── 03_normalisation.ipynb
│
│   ├── 04_CNN_simple_sans_CLAHE.ipynb
│   ├── 05_DenseNet_sans_CLAHE.ipynb
│   ├── 06_ResNet50_sans_CLAHE.ipynb
│   ├── 07_EfficientNet_sans_CLAHE.ipynb
│   ├── 08_VGG16_sans_CLAHE.ipynb
│
│   ├── 09_application_CLAHE.ipynb   
│
│   ├── 10_CNN_simple_avec_CLAHE.ipynb
│   ├── 11_DenseNet_avec_CLAHE.ipynb
│   ├── 12_ResNet50_avec_CLAHE.ipynb
│   ├── 13_EfficientNet_avec_CLAHE.ipynb
│   ├── 14_VGG16_avec_CLAHE.ipynb
│
│   ├── 15_evaluation_comparaison.ipynb
│   └── 16_deploiement.ipynb
│
├── data_info/
│   └── dataset_description.md
│
├── results/
│   ├── figures/
│   ├── metrics/
│   └── models/
│
├── docs/
│   └── rapport.md
│
└── README.md
```

## ⚙️ Installation

### 1. Cloner le projet

```bash
git clone https://github.com/carolembomegni/Projet_SD_Detection_Tumeurs.git
cd Projet_SD_Detection_Tumeurs
```

### 2. Installer les dépendances

```bash
pip install tensorflow keras numpy pandas matplotlib opencv-python scikit-learn
```

---

## ▶️ Utilisation

Le projet est principalement développé avec **Google Colab**.

### Étapes d’exécution

1. Ouvrir les notebooks dans Google Colab
2. Télécharger et charger le dataset (via Kaggle)
3. Exécuter les notebooks dans l’ordre suivant :

#### 🔹 Étape 1 : Préparation des données

* Importation du dataset
* Préprocessing (nettoyage, redimensionnement)
* Création de la classification binaire (Tumor / No Tumor)
* Normalisation

#### 🔹 Étape 2 : Entraînement des modèles sans CLAHE

* CNN simple
* DenseNet
* ResNet50
* EfficientNet
* VGG16

#### 🔹 Étape 3 : Application de CLAHE

* Amélioration du contraste des images

#### 🔹 Étape 4 : Entraînement des modèles avec CLAHE

* CNN simple
* DenseNet
* ResNet50
* EfficientNet
* VGG16

#### 🔹 Étape 5 : Évaluation et comparaison

* Accuracy
* Precision / Recall / F1-score
* Matrice de confusion
* Comparaison des performances (avec vs sans CLAHE)

#### 🔹 Étape 6 : Déploiement

* Sauvegarde du meilleur modèle
* Préparation pour une utilisation en application ou API

---

### ⚠️ Remarques importantes

* Toujours exécuter les notebooks dans l’ordre pour garantir la cohérence des données
* Utiliser un GPU sur Google Colab pour accélérer l’entraînement
* Chaque membre travaille sur sa branche GitHub
* Éviter de modifier le même notebook à plusieurs

---

### 💡 Optionnel

* Un notebook supplémentaire peut être utilisé pour tester des techniques avancées comme le **GAN** pour l’augmentation des données

# 🧪 Méthodologie

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

---

## 📊 Résultats attendus

* Amélioration des performances avec CLAHE
* Comparaison entre modèles

---

## 👥 Équipe

Projet réalisé en groupe (6 personnes) :

* Membre 1 : Préprocessing
* Membre 2 : CLAHE
* Membre 3 : RestNet50
* Membre 4 : Modèle EfficientNet
* Membre 5 : Modèle DenseNet
* Membre 6 : Évaluation & rapport

---

## ⚠️ Remarques importantes

* Les images ne sont pas incluses dans le repo (dataset volumineux)
* Utiliser Google Colab avec GPU recommandé
* Attention aux conflits Git sur les fichiers `.ipynb`

---

## 📚 Technologies utilisées

* Python
* TensorFlow / Keras
* OpenCV
* Scikit-learn
* Google Colab

---

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
