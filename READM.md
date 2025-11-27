# Defective Part Detection

Projet de détection d’anomalies industrielles visant à identifier automatiquement les pièces défectueuses à partir d’images.  
L’objectif est de comparer les performances de deux modèles de vision par ordinateur : **Fast R-CNN** et **YOLO**, sur un même jeu de données annoté.

---

## 🎯 Objectif du projet

- Détecter si une pièce est **défectueuse ou non** à partir d’images.
- Comparer les performances de **Fast R-CNN** et **YOLO** sur la même tâche.
- Mettre en place un pipeline complet :
  - préparation et prétraitement des données,
  - entraînement des modèles,
  - évaluation et comparaison des résultats.

---

## 🧩 Description générale

Le projet comprend :

- la **collecte et l’annotation des données** via **Roboflow** (définition des classes, bounding boxes, export du dataset),
- le **prétraitement des images** (redimensionnement, normalisation, split train/val/test),
- l’utilisation de **data loaders** pour charger efficacement les données durant l’entraînement,
- l’entraînement de deux modèles :
  - un modèle basé sur **Fast R-CNN**,
  - un modèle basé sur **YOLO** (par exemple YOLOv5/YOLOv8 selon la config),
- la **comparaison des modèles** à l’aide de métriques :
  - précision, rappel, mAP,
  - qualité de la localisation des défauts,
  - temps d’inférence (réalité industrielle).

---

## 🛠️ Technologies utilisées

- **Langage** : Python  
- **Deep Learning / Vision** :
  - PyTorch ou TensorFlow/Keras (selon l’implémentation)
  - Modèle **Fast R-CNN**
  - Modèle **YOLO**
- **Traitement d’images** :
  - OpenCV
- **Gestion des données** :
  - Roboflow (annotation, augmentation, export)
  - DataLoaders pour la gestion des batches
- **Environnement** :
  - Jupyter Notebook / scripts Python
  - Git / GitHub pour le versionnement

---

## 🔎 Résultats

Le projet inclut une **comparaison des modèles** :

- différence de performance entre Fast R-CNN et YOLO,
- qualité de détection des pièces défectueuses,
- avantages et limites de chaque approche dans un contexte industriel.

---

## 🎯 Intérêt du projet

Ce projet montre :

- la capacité à mettre en place une **pipeline complet de vision par ordinateur**,
- la maîtrise de modèles de détection d’objets (**Fast R-CNN** et **YOLO**),
- l’utilisation d’outils modernes comme **Roboflow** pour la gestion du dataset,
- une démarche d’**évaluation et de comparaison** de modèles dans un cas concret d’**inspection visuelle industrielle**.
