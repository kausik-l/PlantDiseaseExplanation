# 🌱 Trusted AI Project: Plant Disease Classification and Explanation

This project was done for the Trusted AI course at the University of South Carolina.

<div align="center">
  <img width="373" height="309" alt="Screenshot 2025-07-14 at 4 44 09 PM" src="https://github.com/user-attachments/assets/737d0b63-584b-4618-bed2-460842365f26" />
</div>

## 🎯 Project Overview
This project tackles the real-world problem of plant disease identification using deep learning, with more emphasis on explainability and trustworthiness of AI systems. While traditional classifiers like CNN and InceptionV3 achieve good accuracy, they often lack transparency. This project combines model performance analysis with LIME-based explanations to improve trust in AI-driven crop diagnostics.

📄 Full Report: docs/Plant_Disease_Explanation___Trusted_AI_project.pdf

## 🧠 Motivation
Every year, countries like India lose over 35% of crop yield due to plant diseases, many of which go undetected due to poor access to diagnostics. With the rise of mobile AI solutions, it is crucial to build systems that not only detect diseases but also justify their predictions to users like farmers, agronomists, or government monitoring agents.

## 📂 Repository Contents

- `code/` — Eval-PlantDoc.ipynb and Eval-PlantVillage.ipynb.
- `models/` — Saved models and logs.
- `docs/` — My project report.
- `README.md` — This file.

## 🧰 Models Trained
1. Custom CNN: 5 Conv-BN-ReLU-MaxPool-Dropout blocks; Dense output with softmax classifier.
2. InceptionV3: Pre-trained on ImageNet, fine-tuned with a custom dense head; Transfer learning for improved generalization.

## Datasets
1. PlantVillage: Clean, lab-collected dataset with 15 disease classes. Pictures taken in a more controlled lab settings.
2. PlantDoc: Real-world dataset with diverse backgrounds. Contains 17 disease classes. Lower quality (watermarks, lighting issues), yet more realistic.

## 💡 Explainability: LIME
To build trustworthy AI, I used LIME (Local Interpretable Model-Agnostic Explanations) to highlight regions of the leaf that influenced model predictions.
Key Observations:
1. LIME explanations revealed that PlantVillage-trained models generalized better.
2. Only the PlantVillage-InceptionV3 model correctly predicted both plant and disease name on a held-out tomato leaf.

<div align="center">
     <img width="254" height="256" alt="Screenshot 2025-07-14 at 4 37 39 PM" src="https://github.com/user-attachments/assets/e8eb0538-e55b-45c6-a8bd-99f1d229de9b" />
</div>
