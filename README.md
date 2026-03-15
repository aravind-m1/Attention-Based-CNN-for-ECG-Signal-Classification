# Multi-Lead ECG for Early Cardiac Disease Detection

## Attention-Based CNN for ECG Signal Classification

## Project Overview

This project presents a deep learning approach for **early cardiac disease detection using multi-lead ECG signals**. The system reconstructs and analyzes ECG waveforms and classifies them into diagnostic categories using an **Attention-Based Convolutional Neural Network (CNN)**.

Electrocardiogram (ECG) signals contain valuable information about the electrical activity of the heart. Manual interpretation of ECG recordings can be time-consuming and prone to human error. This project uses artificial intelligence to automatically extract patterns from ECG signals and accurately classify cardiac conditions.

The proposed model integrates **Convolutional Neural Networks (CNN)** for feature extraction and **Multi-Head Attention mechanisms** for capturing temporal dependencies within ECG signals.

---

## Model Name

**ECG-AttentionNet**

**Description**

ECG-AttentionNet is a deep learning model designed to classify ECG signals by combining convolutional feature extraction with attention mechanisms. CNN layers capture local waveform patterns, while attention layers focus on important signal segments, improving classification accuracy and robustness.

---

## Features

* Multi-lead ECG signal analysis
* Deep learning based classification
* CNN based feature extraction
* Attention mechanism for temporal pattern recognition
* Visualization of ECG signals
* Hyperparameter tuning using Keras Tuner
* Training experiment tracking
* Exportable experiment logs

---

## Technologies Used

### Programming Language

* Python

### Libraries & Frameworks

* TensorFlow / Keras
* Keras Tuner
* NumPy
* Pandas
* Matplotlib
* Seaborn
* WFDB (Waveform Database)

### Tools

* Jupyter Notebook
* Weights & Biases (for experiment tracking)

---

## Project Workflow

### 1. Dataset Loading

The ECG dataset is loaded using the **WFDB library**, which reads waveform database records and converts them into structured signal arrays.

### 2. Data Preprocessing

The dataset undergoes preprocessing steps including:

* Converting signals into NumPy arrays
* Encoding labels into categorical format
* Preparing data for neural network input

### 3. Label Distribution Analysis

Class distribution is analyzed to understand the balance between different ECG categories in training and testing datasets.

### 4. ECG Signal Visualization

Random ECG signals are visualized to inspect waveform characteristics and ensure correct dataset loading.

### 5. Model Architecture

The model consists of:

* Convolutional layers for extracting ECG features
* Multi-Head Attention layers for capturing long-range dependencies
* Dense layers for classification

### 6. Hyperparameter Tuning

Keras Tuner is used to search for optimal model parameters such as:

* Number of filters
* Kernel size
* Activation functions
* Learning rate

### 7. Model Training

The optimized model is trained using the prepared ECG dataset.

### 8. Experiment Tracking

Training experiments are logged using **Weights & Biases (WandB)** to track metrics such as:

* Accuracy
* Loss
* Validation performance

### 9. Result Export

Training logs and experiment results are compressed and exported for future analysis.

---

## Model Architecture Overview

Input ECG Signal
↓
Convolutional Layers (Feature Extraction)
↓
Multi-Head Attention Layer (Temporal Dependency Learning)
↓
Fully Connected Dense Layers
↓
Softmax Output Layer (Classification)

---

## Dataset

The dataset consists of **multi-lead ECG recordings** where each sample represents electrical activity of the heart over time.

Each ECG signal contains:

* Multiple time steps
* Multiple leads (channels)
* Corresponding diagnostic label

---

## How to Run the Project

### Step 1: Install Required Libraries

```
pip install tensorflow keras keras-tuner wfdb numpy pandas matplotlib seaborn wandb
```

### Step 2: Run the Notebook

Open and execute the notebook:

```
Attention-CNN.ipynb
```

Run all cells sequentially to train and evaluate the model.

---

## Results

The model learns ECG waveform patterns and performs classification based on learned features extracted from the signals.

Performance is evaluated using metrics such as:

* Training Accuracy
* Validation Accuracy
* Loss Curves

---

## Applications

* Early cardiac disease detection
* Automated ECG interpretation
* Clinical decision support systems
* Remote health monitoring

---

## Future Improvements

* Integration with real-time ECG monitoring devices
* Deployment as a web-based diagnostic tool
* Training with larger clinical datasets
* Explainable AI for ECG interpretation

---

## Conclusion

This project demonstrates how deep learning can be used to analyze ECG signals and assist in detecting cardiac abnormalities. By combining CNN feature extraction with attention mechanisms, the model can capture both local and long-range patterns in ECG signals, improving diagnostic accuracy.

---

