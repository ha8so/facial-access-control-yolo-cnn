# Facial Access Control using YOLO and CNN

## 📌 Contexte du projet
La reconnaissance faciale est aujourd’hui un élément central des systèmes de sécurité modernes. Elle permet un **contrôle d’accès automatisé, rapide et sans contact**, contrairement aux badges, codes ou cartes, qui sont facilement partageables ou volés.

Cependant, la reconnaissance faciale en conditions réelles reste un défi à cause de :
- variations de luminosité
- angles de caméra
- expressions faciales
- accessoires (masques, lunettes, ombres)

Notre objectif est de concevoir un **pipeline de reconnaissance faciale en deux étapes**, combinant la rapidité de **YOLO** pour détecter les visages et la capacité discriminante d’un **CNN** pour décider si la personne est autorisée ou non.

---

## 🎯 Objectifs du projet
- Détecter les visages en temps réel avec YOLO (v5 ou v8)
- Classifier les visages détectés via un CNN (binaire : *autorisé / non autorisé*)
- Optimiser l’inférence (ONNX, quantization FP16/INT8)
- Évaluer la performance avec : *accuracy, F1-score, rappel, AUC-ROC*
- Étudier l’impact de :
  - la taille d’image
  - le seuil de détection
  - l’augmentation de données
  - la profondeur du CNN

---

## 📌 Dataset utilisé
Nous utiliserons des bases publiques d’images faciales, telles que :

- **LFW — Labeled Faces in the Wild**
- **CelebA**
- (optionnel) Dataset interne pour “autorisé / non autorisé”

Chaque image est associée à une étiquette :

| Valeur | Signification |
|---------|--------------|
| `1`     | Visage autorisé |
| `0`     | Visage non autorisé |

---

## 🛠️ Méthodologie prévue (Pipeline)
1. **Détection du visage (YOLO)**
2. **Extraction de la zone faciale**
3. **Classification CNN (ou ResNet/VGG fine-tunée)**
4. **Étude d’ablation**
5. **Optimisation d’inférence (ONNX, quantization)**
6. **Évaluation et visualisation Grad-CAM**

---

## 🚀 Étapes à venir (Roadmap)
| Étape | Statut |
|---------|---------|
| Création du repo GitHub | ✅ |
| Notebook YOLO – détection | ⏳ |
| CNN – classification | ⏳ |
| Étude d’ablation | ⏳ |
| Déploiement / Démo | ⏳ |
| Rapport final + soutenance | ⏳ |

---

## 🤝 Collaboration Git
Chaque membre travaille sur **sa branche** :

