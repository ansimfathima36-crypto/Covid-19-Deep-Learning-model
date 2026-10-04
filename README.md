# 🦠 COVID-19 Image Classification using CNN

A Deep Learning project that uses **Convolutional Neural Networks (CNN)** to classify chest X-ray images into **COVID-19** and **Normal** classes.

## 📌 Project Overview

The goal of this project is to develop a deep learning-based image classification system that can identify COVID-19 cases from chest X-ray images.

The project includes:

* Image data analysis
* Data visualization
* Image preprocessing
* CNN model development
* Model comparison
* Performance evaluation
* COVID-19 recall analysis

> **Note:** This project is an educational machine learning project and should not be considered a medical diagnostic system.

## 🎯 Objective

The main objective is to build a CNN-based model that can classify chest X-ray images as:

* 🦠 **COVID-19**
* 🫁 **Normal**

The project aims to explore how deep learning can be applied to medical image classification.

## 📊 Dataset

The dataset contains **251 chest X-ray images** belonging to two classes:

| Class    | Description                                      |
| -------- | ------------------------------------------------ |
| COVID-19 | Chest X-ray images of COVID-19 affected patients |
| Normal   | Chest X-ray images classified as normal          |

### Image Details

* **Number of Images:** 251
* **Image Size:** 128 × 128 pixels
* **Channels:** 3 (RGB)

### Dataset Files

* `CovidImages.npy` – Image data stored as NumPy arrays
* `CovidLabels.csv` – Corresponding image labels

## 🛠️ Technologies Used

* Python
* NumPy
* Pandas
* Matplotlib
* Seaborn
* OpenCV
* TensorFlow
* Keras
* Scikit-learn
* Google Colab

## 🧠 Deep Learning Approach

The project uses a **Convolutional Neural Network (CNN)** for binary image classification.

### CNN Workflow

```text
Chest X-ray Images
        ↓
Data Loading
        ↓
Data Visualization
        ↓
Image Preprocessing
        ↓
Train / Validation / Test Split
        ↓
CNN Model Training
        ↓
Model Evaluation
        ↓
COVID-19 / Normal Prediction
```

## 🏗️ Models Developed

Two CNN models were developed and compared:

### Model 1 — 3-Layer CNN

The deeper CNN contains:

* 3 Convolutional layers
* 3 MaxPooling layers
* Flatten layer
* Dense hidden layer with ReLU activation
* Sigmoid output layer

The model contains approximately **4.29 million trainable parameters**.

### Model 2 — 2-Layer CNN

A simpler CNN architecture was also developed to compare performance and generalization.

The project selected the **2-layer CNN as the final model** because it provided strong validation performance with a simpler architecture.

## ⚙️ Model Configuration

The CNN uses:

* **Activation:** ReLU for hidden layers
* **Output Activation:** Sigmoid
* **Optimizer:** Adam
* **Loss Function:** Binary Cross-Entropy
* **Evaluation Metric:** Accuracy
* **Classification Threshold:** 0.5

## 📈 Model Evaluation

The models were evaluated using:

* Training Accuracy
* Validation Accuracy
* COVID-19 Recall
* Test Accuracy
* Test Recall

### Model Comparison

| Model       | Train Accuracy | Validation Accuracy | COVID Recall |
| ----------- | -------------: | ------------------: | -----------: |
| 3-Layer CNN |           100% |              97.37% |         100% |
| 2-Layer CNN |         99.43% |                100% |         100% |

Based on the notebook's model-selection discussion, the **2-layer CNN was chosen as the final model** because it offered strong performance with a simpler architecture and better generalization.

## 🏆 Final Model Performance

The final 2-layer CNN was evaluated on the test dataset.

According to the recorded notebook output:

* **Test Accuracy:** 100%
* **Test COVID Recall:** 100%

> Results can vary when the notebook is retrained because of differences in the training environment, data splitting, and model initialization.

## 🔍 Key Learnings

Through this project, I gained practical experience in:

* Working with image datasets
* Loading `.npy` and `.csv` files
* Image preprocessing
* CNN architecture
* Convolution and pooling
* Binary image classification
* Model training and validation
* Model comparison
* Classification evaluation
* COVID-19 recall analysis
* TensorFlow/Keras model development

## 📁 Project Structure

```text
COVID-19-Image-Classification/
│
├── Covid_19_Image_Classification.ipynb
├── CovidImages.npy
├── CovidLabels.csv
└── README.md
```

## 🚀 Future Improvements

* Increase the size and diversity of the dataset
* Apply data augmentation
* Experiment with transfer learning models
* Improve model generalization
* Test the model on a larger independent dataset
* Explore explainable AI techniques for medical images

## ⚠️ Disclaimer

This project is created for **educational and learning purposes only**. The model should not be used as a substitute for professional medical diagnosis or clinical decision-making.

## 👩‍💻 Author

**Ansim Fathima**

B.Sc. Data Science
Interested in **Data Analytics, Data Science, Machine Learning & AI**

---

⭐ If you find this project useful, feel free to explore the notebook and learn from the implementation!
