# Predict-Customer-Churn-with-TensorFlow
Predict Customer Churn with TensorFlow
📌 Description

Ce projet illustre l’utilisation de TensorFlow (tf.keras) pour construire, entraîner et évaluer un modèle de Deep Learning de prédiction du churn client.
L’objectif principal n’est pas d’obtenir la meilleure performance possible, mais de tester et comprendre l’utilisation complète de TensorFlow : préparation des données, définition du modèle, entraînement, suivi avec TensorBoard et sauvegarde pour un éventuel déploiement.

⚙️ Stack technique

Langage : Python

Framework : TensorFlow / Keras

Data processing : pandas, NumPy, scikit-learn

Visualization : Matplotlib, Seaborn, TensorBoard

🧩 Étapes du projet

# 1️⃣ Préparation des données 

Chargement du dataset Churn.csv depuis Google Drive

Encodage des variables catégorielles avec get_dummies()

Normalisation avec StandardScaler()

Division en 80 % train / 20 % test

# 2️⃣ Définition du modèle TensorFlow

Création d’un modèle séquentiel
🧠

ReLU : introduit de la non-linéarité

Dropout : limite le surapprentissage

Sigmoid : produit une probabilité (classification binaire)

# 3️⃣ Compilation

Adam : apprentissage rapide et stable

Binary Crossentropy : adaptée à la classification binaire

Accuracy : mesure globale des bonnes prédictions

# 4️⃣ Entraînement du modèle

Utilisation de callbacks professionnels :

EarlyStopping → arrête automatiquement l’entraînement si la validation n’évolue plus

TensorBoard → permet de suivre les courbes de perte et d’accuracy

# 5️⃣ Évaluation du modèle

Résultats obtenus :

Accuracy : ≈ 76 %

Bon rappel sur la classe “Non churn”, plus faible sur la classe “Churn”.

# 📉 Déséquilibre des classes

Ce déséquilibre explique que le modèle détecte mieux les clients fidèles que les churns.

Pour améliorer le modèle :

Pondérer les classes avec class_weight='balanced'

Rééchantillonner les données (oversampling ou SMOTE)

Ajuster le seuil de décision pour mieux capter la classe minoritaire

👉 Mais ce n’est pas l’objectif ici : le but de ce projet est de tester et documenter l’utilisation de TensorFlow, pas d’optimiser la performance du modèle.

# 📦 Sauvegarde du modèle

☁️ Déploiement possible

TensorFlow offre plusieurs options selon le contexte :

Option	Usage
TensorFlow Serving	API REST / gRPC côté serveur
TensorFlow Lite	Applications mobiles et embarquées
TensorFlow.js	Exécution côté navigateur
Cloud Platforms	Déploiement sur GCP, AWS ou Azure

# 👤 Auteur

Kokouvi KADA-SEDODE
Data Scientist & Machine Learning Engineer
