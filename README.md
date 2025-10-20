# Pneumonia Detection from Chest X-ray using Deep Learning

##  Contexte du projet
La pneumonie est une infection pulmonaire potentiellement grave qui nécessite un diagnostic rapide. L’analyse manuelle des radiographies thoraciques (Chest X-ray) par un spécialiste reste la méthode courante, mais elle est sujette à la variabilité humaine et peut prendre du temps.  
L’objectif de ce projet est d’automatiser la détection de la pneumonie à partir d’images médicales en utilisant des techniques de **Computer Vision** et des modèles **Deep Learning pré-entraînés**.

Ce travail s’inscrit dans le cadre d’un projet académique dont le but est d’apprendre à mener un projet machine learning de bout en bout, tout en adoptant une approche reproductible, rigoureuse et collaborative.

---

##  Objectif
Développer un modèle capable de classifier automatiquement des radiographies pulmonaires en deux classes :

- **Pneumonia**
- **Normal**

Les objectifs techniques incluent :

- Construire un **pipeline reproductible**
- Exploiter le **Transfer Learning**
- Comparer deux approches :
  1. **Embeddings + modèles légers** (SVM / Régression Logistique)
  2. **Fine-tuning de CNN pré-entraînés** (ResNet, EfficientNet, DenseNet)
- Réaliser une **étude d’ablation**
- Optimiser l’inférence (**quantization FP16 / INT8**)
- Évaluer le modèle à l’aide de métriques pertinentes (AUC, F1-score, précision, rappel)
- Produire des **visualisations explicatives (Grad-CAM)**

---

##  Dataset utilisé
Nous utiliserons le dataset public :

- **Chest X-ray Pneumonia Dataset (Kaggle)**
  https://www.kaggle.com/paultimothymooney/chest-xray-pneumonia

Il s’agit d’images radiographiques organisées en deux classes : `NORMAL` et `PNEUMONIA`.  
Un split **train / validation / test** sera appliqué afin d’assurer une évaluation juste et objective.

---

##  Méthodologie prévue

La démarche suivra les étapes suivantes :

1. **Exploration des données (EDA)**  
2. **Prétraitement & Data Augmentation**
3. **Approche Baseline** (embeddings + modèle léger)
4. **Approche Transfer Learning** (fine-tuning CNN)
5. **Ablation Study**
6. **Évaluation des performances** (AUC, F1, etc.)
7. **Explicabilité (Grad-CAM)**
8. **Optimisation de l’inférence (quantization)**

---

##  Étapes à venir (Roadmap)

| Étape | Statut |
|---------|---------|
| Mise en place du repository GitHub | ✅ |
| Ajout du rapport préliminaire (docs/) | ✅ |
| EDA + Notebook baseline | ⏳ |
| Transfer Learning & Ablation | ⏳ |
| Évaluation & Visualisations | ⏳ |
| Optimisation & Documentation finale | ⏳ |
| Presentation final + Soutenance | ⏳ |

---

##  Contribution des membres
Le développement se fera en équipe, en utilisant des **branches séparées** et des **pull requests** afin d'assurer une collaboration propre et transparente.

---

##  Références
- Kaggle Dataset — Chest X-ray Pneumonia
- ResNet, EfficientNet, DenseNet — Papers & documentation
- Grad-CAM — Selvaraju et al. (2017)
- ONNX / TensorRT — optimisation inference

---



