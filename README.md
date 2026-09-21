# 🌱 Plant Seedlings Classification using CNN

A computer vision project that classifies plant seedling images into 12 different plant species using Convolutional Neural Networks (CNNs), image preprocessing, and data augmentation.

The project demonstrates an end-to-end deep learning workflow, including exploratory data analysis, image preprocessing, model development, model improvement, and performance evaluation.

## 📌 Project Overview

Identifying plant species at the seedling stage can be challenging because many plants have very similar visual characteristics.

The objective of this project is to develop a deep learning image classification model capable of automatically identifying the species of a plant seedling from an image.

Such computer vision systems could potentially support agricultural applications such as:

* Automated plant identification
* Weed detection
* Crop monitoring
* Precision agriculture
* Reduction of manual plant inspection

## 🎯 Objective

Build and evaluate a multi-class image classification model that predicts the species of a plant seedling from an input image.

The project focuses on:

* Image preprocessing
* Exploratory analysis of image data
* Convolutional Neural Networks
* Data augmentation
* Handling class imbalance considerations
* Multi-class model evaluation
* Analysis of model generalization

## 📊 Dataset

The dataset contains **4,750 images** of plant seedlings belonging to **12 species**, including:

* Black-grass
* Charlock
* Cleavers
* Common Chickweed
* Common Wheat
* Fat Hen
* Loose Silky-bent
* Maize
* Scentless Mayweed
* Shepherds Purse
* Small-flowered Cranesbill
* Sugar Beet

The dataset has moderate class imbalance, with some species having significantly more samples than others.

## 🔧 Project Workflow

1. **Exploratory Data Analysis**

   * Visualized plant species
   * Analyzed class distribution
   * Identified class imbalance

2. **Image Preprocessing**

   * Converted images from BGR to RGB
   * Resized images to **64 × 64**
   * Normalized pixel values
   * Encoded target labels
   * Split data into training, validation, and test sets

3. **CNN Model Development**

   * Built a custom CNN using TensorFlow/Keras
   * Used convolution, max-pooling, dense, and dropout layers
   * Used Softmax for multi-class classification

4. **Model Improvement**

   * Applied data augmentation including rotation, shifting, zooming, and horizontal flipping
   * Compared the augmented CNN with the baseline model

## 📈 Results

| Model                   | Validation Accuracy | Weighted F1 |
| ----------------------- | ------------------: | ----------: |
| Baseline CNN            |               72.6% |       69.9% |
| CNN + Data Augmentation |           **75.6%** |   **73.2%** |

### Final Test Performance

* **Accuracy:** 75.2%
* **Weighted Precision:** 73.4%
* **Weighted Recall:** 75.2%
* **Weighted F1 Score:** 72.0%

The CNN with data augmentation showed better generalization and reduced overfitting compared with the baseline model.

## 💡 Key Insights

* Data augmentation improved model performance and generalization.
* Class imbalance affected performance across individual plant species.
* Visually similar plant species were more challenging for the model to distinguish.
* Per-class precision and recall are important in addition to overall accuracy.

## 🛠️ Technologies Used

**Python | TensorFlow | Keras | OpenCV | NumPy | Pandas | Scikit-learn | Matplotlib | Seaborn | Google Colab**

## 🚀 Future Improvements

* Experiment with transfer learning models such as **VGG16, ResNet, or EfficientNet**
* Apply additional techniques for handling class imbalance
* Perform hyperparameter tuning
* Deploy the model as a simple web application for plant identification

## 👩‍💻 Author

**Nikhila Vecham**

AI/ML enthusiast building hands-on machine learning and deep learning projects.
