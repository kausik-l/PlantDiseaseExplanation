# 🌱 Trusted AI Project: Plant Disease Classification and Explanation

This project was done for the Trusted AI course at the University of South Carolina.

<img width="373" height="309" alt="Screenshot 2025-07-14 at 4 44 09 PM" src="https://github.com/user-attachments/assets/737d0b63-584b-4618-bed2-460842365f26" />

## 🎯 Project Overview
This project tackles the real-world problem of plant disease identification using deep learning, with more emphasis on explainability and trustworthiness of AI systems. While traditional classifiers like CNN and InceptionV3 achieve good accuracy, they often lack transparency. This project combines model performance analysis with LIME-based explanations to improve trust in AI-driven crop diagnostics.

📄 Full Report: docs/Plant_Disease_Explanation___Trusted_AI_project.pdf

## 🧠 Motivation
Every year, countries like India lose over 35% of crop yield due to plant diseases, many of which go undetected due to poor access to diagnostics. With the rise of mobile AI solutions, it is crucial to build systems that not only detect diseases but justify their predictions to users like farmers, agronomists, or government monitoring agents.

## 📂 Repository Contents
.
├── Code
     └─ Eval-PlantDoc.ipynb
     └─ Eval-PlantVillage.ipynb
├── docs/
│   └── Plant_Disease_Explanation___Trusted_AI_project.pdf
└── README.md

| Dataset        | Description                                     | Classes     | Notes                                           |
|----------------|-------------------------------------------------|-------------|-------------------------------------------------|
| **PlantVillage** | Lab-collected, consistent lighting, clean images | 15 (subset) | High quality, but lacks real-world variability  |
| **PlantDoc**     | Real-world images, varying backgrounds & quality | 17          | Contains watermarks and lighting inconsistencies |



