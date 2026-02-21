# AI-Based Skin Disease Prediction Chatbot

## Overview
This project is an **AI-powered chatbot** designed to predict skin diseases by combining **image classification, decision tree analysis, and NLP-based conversational capabilities**. Users can upload an image of a skin condition and answer a short questionnaire, after which the chatbot predicts the most probable skin disease.  

The system leverages:  
- **Customized Convolutional Neural Network (CNN)** for image-based skin disease classification.  
- **Dynamic ID3 Decision Tree** to refine predictions based on user symptoms.  
- **Natural Language Processing (NLP)** for handling user queries and providing general information about skin diseases.  

The goal is to provide an **accessible, accurate, and user-friendly tool** for skin disease detection, especially for individuals who may not have immediate access to dermatologists.

---

## Features
- Image-based skin disease classification into six categories:  
  - Actinic Keratosis  
  - Basal Cell Carcinoma  
  - Melanoma  
  - Nevus  
  - Seborrheic Keratosis  
  - Squamous Cell Carcinoma  
- Dynamic questionnaire for improved prediction accuracy using Decision Tree.  
- NLP-enabled chatbot to answer general queries about skin diseases.  
- User-friendly interface that guides users through image upload and symptom input.

---

## Tech Stack
- **Programming Languages:** Python  
- **Deep Learning:** TensorFlow, Keras, CNN  
- **Machine Learning:** ID3 Decision Tree, Data Augmentation (Augmentor)  
- **NLP:** NLTK for preprocessing and query handling  
- **Data Visualization:** Matplotlib, Seaborn  
- **Datasets:** ISIC2019 Skin Disease Image Dataset, custom symptom dataset for decision tree  
- **Others:** Pandas, NumPy, PIL

---

## Project Modules

### Module 1: CNN Model for Skin Disease Classification
- Trains a **custom CNN** on the ISIC2019 dataset.  
- Handles **class imbalance** using data augmentation.  
- Model achieves:  
  - **Training Accuracy:** 89.25%  
  - **Validation Accuracy:** 87.33%  
- Saves the trained CNN model for inference.

### Module 2: Disease Shortlisting
- Loads the trained CNN model to shortlist probable diseases for a given image.  
- Diseases above a defined threshold (0.5) are selected for further analysis.

### Module 3: Dynamic Decision Tree
- Uses a **Dynamic ID3 Decision Tree** to ask symptom-based questions.  
- Refines predictions using answers from the user.  
- Improves diagnostic accuracy to **~91.56%**.

### Module 4: NLP Chatbot
- Handles general questions about skin diseases using a preprocessed Q&A corpus.  
- Provides interactive, conversational support for users.

## Results

- Accurate skin disease predictions based on uploaded images and symptom analysis.  
- **CNN model validation accuracy:** 87.33%  
- **Decision Tree integrated predictions:** 91.56% accuracy  
- Real-time chatbot interaction with symptom-based guidance and general skin disease knowledge.
---
