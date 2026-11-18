# Facial Emotion Recognition (FER)

\<p align="center">
&#x20; \<img src="[https://img.shields.io/badge/Python-8B6F47?style=for-the-badge&logo=python&logoColor=white](https://img.shields.io/badge/Python-8B6F47?style=for-the-badge\&logo=python\&logoColor=white)" />
&#x20; \<img src="[https://img.shields.io/badge/TensorFlow-8B6F47?style=for-the-badge&logo=tensorflow&logoColor=white](https://img.shields.io/badge/TensorFlow-8B6F47?style=for-the-badge\&logo=tensorflow\&logoColor=white)" />
&#x20; \<img src="[https://img.shields.io/badge/Keras-8B6F47?style=for-the-badge&logo=keras&logoColor=white](https://img.shields.io/badge/Keras-8B6F47?style=for-the-badge\&logo=keras\&logoColor=white)" />
&#x20; \<img src="[https://img.shields.io/badge/Computer%20Vision-8B6F47?style=for-the-badge](https://img.shields.io/badge/Computer%20Vision-8B6F47?style=for-the-badge)" />
&#x20; \<img src="[https://img.shields.io/badge/Deep%20Learning-8B6F47?style=for-the-badge](https://img.shields.io/badge/Deep%20Learning-8B6F47?style=for-the-badge)" />
\</p>

## 📌 Overview

Facial Emotion Recognition (FER) is a deep learning project designed to identify human emotions from facial expressions using computer vision techniques.

The project explores and compares two deep learning architectures, **VGG16** and **ResNet50**, to classify facial expressions into seven emotional categories.

It combines image preprocessing, transfer learning, model fine-tuning, and performance evaluation, with a Streamlit application for interactive emotion prediction.

## 🎯 Objectives

- Develop deep learning models for facial emotion classification.
- Explore CNN architectures and transfer learning.
- Compare VGG16 and ResNet50 performance.
- Evaluate model generalization on unseen data.
- Build an interactive application for real-time image-based predictions.

## 🧠 Emotion Categories

The models classify facial expressions into seven categories:

|  Emotion | Emotion |  Emotion |
| :------: | :-----: | :------: |
|   Angry  | Disgust |   Fear   |
|   Happy  | Sadness | Surprise |
| Contempt |         |          |

## 📂 Datasets

The project explores two facial expression datasets:

**1. CK+48 Dataset**

- Used for VGG16 experimentation.
- Contains facial expression images organized into emotion categories.
- Images were processed at 48 × 48 resolution.

**2. FER2013 Dataset**

- Used for ResNet50 experimentation.
- Contains facial images labeled with seven emotion classes.
- Images were resized to 224 × 224 pixels to match the pretrained ResNet50 architecture.

## ⚙️ Methodology

### 1. Data Preprocessing

- Image resizing and normalization.
- Dataset organization and label preparation.
- Training and validation data preparation.

### 2. Model Architectures

**VGG16**

A convolutional neural network architecture used to extract facial features and learn emotion-related patterns.

**ResNet50**

A deeper residual network leveraging skip connections to facilitate training and feature extraction.

### 3. Transfer Learning & Fine-Tuning

The ResNet50 model uses ImageNet-pretrained weights.

The training process includes:

- Transfer learning with pretrained feature extraction.
- Fine-tuning selected layers.
- Model optimization and evaluation.

### 4. Model Evaluation

The models are evaluated using classification accuracy on their respective datasets, with particular attention to performance on unseen test data.

## 📊 Experimental Results

| Model    | Dataset | Metric              | Result |
| -------- | ------- | ------------------- | -----: |
| VGG16    | CK+48   | Validation Accuracy |    65% |
| ResNet50 | FER2013 | Training Accuracy   | 78.30% |
| ResNet50 | FER2013 | Test Accuracy       | 64.56% |

**Key observations:**

- ResNet50 achieved 78.30% training accuracy.
- The test accuracy of 64.56% highlights the challenge of generalizing facial emotion recognition to unseen images.
- Further improvements could explore data augmentation, regularization, and hyperparameter optimization.

*Note: These results come from different datasets and experimental setups, so they should not be interpreted as a direct architecture comparison.*

## 🖥️ Interactive Application

A Streamlit application was developed to demonstrate the trained model's predictions through an interactive interface.

Users can upload a facial image and obtain an emotion classification.

**Run the application:**

```bash
streamlit run app.py
```

## 🛠️ Technologies & Tools

| Category        | Technologies         |
| --------------- | -------------------- |
| Programming     | Python               |
| Deep Learning   | TensorFlow, Keras    |
| Architectures   | VGG16, ResNet50, CNN |
| Computer Vision | OpenCV               |
| Data Processing | NumPy, Pandas        |
| Visualization   | Matplotlib           |
| Deployment      | Streamlit            |
| Development     | VS Code, Git, GitHub |

## 🚀 Getting Started

**1. Clone the repository**

```bash
git clone https://github.com/YOUR_USERNAME/YOUR_REPOSITORY.git
```

**2. Navigate to the project directory**

```bash
cd YOUR_REPOSITORY
```

**3. Install dependencies**

```bash
pip install -r requirements.txt
```

**4. Launch the application**

```bash
streamlit run app.py
```

Make sure the required trained model files and datasets are available in their expected locations before running the application.

## 🔮 Future Improvements

- Improve classification accuracy and generalization.
- Experiment with additional CNN architectures.
- Apply advanced data augmentation techniques.
- Explore real-time facial emotion recognition using a webcam.
- Investigate lightweight models for efficient deployment.

## 👩‍💻 Author

**Malek Yaferni**

Industrial Computer Engineering Student | AI & Machine Learning Enthusiast

- [GitHub](https://github.com/YOUR_USERNAME)
- [LinkedIn](YOUR_LINKEDIN_URL)

---

\<p align="center">   \<i>Exploring the intersection of Deep Learning and Computer Vision.\</i> \</p>
