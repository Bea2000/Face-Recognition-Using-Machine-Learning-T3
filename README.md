# Face Recognition Using Machine Learning

This project was completed as part of an Artificial Intelligence course during the first semester of 2023 at the Pontificia Universidad Católica de Chile. The goal was to build a face recognition system that could distinguish between Avengers and Chitauri characters using machine learning techniques.

## Context

As part of a mission with S.H.I.E.L.D. in Manhattan, you need to identify your allies, the Avengers, and differentiate them from your enemies, the Chitauri. To achieve this, a set of drones capable of facial recognition is available, but they need to be trained with updated data. Your task is to use machine learning to train these drones to recognize the Avengers accurately.

## Objectives

1. **Data Analysis and Exploration**: Load the Avengers dataset, which contains facial images of several Avengers. Analyze the dataset and visualize the distribution of images across classes (Avengers characters).
2. **Data Preprocessing**: Extract facial landmarks from the images using the `face_recognition` library. Clean the dataset, handling cases where landmarks cannot be detected, and update the class distribution.
3. **Feature Engineering**: Generate meaningful features from the extracted landmarks to improve the classification performance.
4. **Model Training and Evaluation**: Train machine learning models (SVM, Naive Bayes, and Decision Trees) to classify the images into different Avengers based on their facial features.
5. **Classification and Prediction**: Use the trained models to classify new images and evaluate their performance in recognizing Avengers.

## Dataset

The dataset contains images of Avengers divided into subfolders based on the character:

- Black Widow
- Captain America
- Hawkeye
- Hulk
- Iron Man
- Nick Fury
- Thor

Each folder contains images of the respective Avenger's face, and the class labels are inferred from the folder names.

## Requirements

The project requires the following libraries:
    - `pandas`
    - `scikit-learn`
    - `face_recognition`
    - `gdown` (to download the dataset)

## How to Run the Project

1. **Clone the Repository**:

    ```bash
    git clone https://github.com/yourusername/your-repo-name.git
    cd your-repo-name
    ```

2. **Run the Code**:
    You can run the code directly on your local machine or use Google Colab with GPU support for better performance.

## Feature Engineering

Using facial landmarks, we created custom features such as distance between the eyes, the width of the nose, and more, which helped in distinguishing between different Avengers.

