# Breast Cancer Classification using CNN-LSTM with Grey Wolf Optimization

## 🌟 Introduction

Breast cancer remains one of the most prevalent forms of cancer affecting women worldwide. Early and accurate detection is crucial for successful treatment outcomes. This project leverages cutting-edge deep learning techniques combined with nature-inspired optimization algorithms to create a robust classification system that can assist medical professionals in making more accurate diagnoses.

The innovative combination of CNN-LSTM architecture with Grey Wolf Optimization represents a significant step forward in medical image analysis, offering both high accuracy and computational efficiency.

## 🎯 Project Overview

The project uses a sophisticated approach to classify breast cancer cases into healthy and sick categories using medical data. The architecture combines:
- 1D Convolutional Neural Networks (CNN)
- Long Short-Term Memory Networks (LSTM)
- Grey Wolf Optimizer (GWO) for hyperparameter optimization

## 📊 Dataset

The project uses four datasets stored in .mat files:
- `myenvLH.mat`: Left Healthy data
- `myenvLS.mat`: Left Sick data
- `myenvRH.mat`: Right Healthy data
- `myenvRS.mat`: Right Sick data

## 🏗️ Model Architecture

The model consists of:
1. Input Layer
2. Conv1D layer with optimized filters and kernel size
3. Batch Normalization
4. MaxPooling1D
5. Dropout layer
6. LSTM layer
7. Multiple Dense layers (optimized number)
8. Output layer with sigmoid activation

## 🔧 Hyperparameter Optimization

The Grey Wolf Optimizer (GWO) algorithm optimizes the following hyperparameters:
- Number of Conv1D filters
- Kernel size
- LSTM units
- Dropout rate
- Learning rate
- Batch size
- Number of dense layers
- Dense layer units
- Number of epochs

## 📈 Results

The model's performance is evaluated using:
- Training accuracy
- Validation accuracy
- Test accuracy



## 🛠️ Requirements

This project requires Python 3.x and the following packages:
```
tensorflow>=2.10.0
numpy>=1.21.0
scipy>=1.7.0
scikit-learn>=1.0.0
matplotlib>=3.4.0
pandas>=1.3.0
```

## 🚀 Getting Started

1. **Environment Setup**
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate
   ```

2. **Install Requirements**
   ```bash
   pip install -r requirements.txt
   ```

3. **Prepare Data**
   - Place the following .mat files in your project directory:
     - myenvLH.mat
     - myenvLS.mat
     - myenvRH.mat
     - myenvRS.mat

4. **Run the Model**
   ```bash
   python improved_gwo_cnn_lstm.py
   ```

## 📦 Project Structure

```
.
├── improved_gwo_cnn_lstm.py  # Main implementation file
├── myenvLH.mat              # Left Healthy data
├── myenvLS.mat              # Left Sick data
├── myenvRH.mat              # Right Healthy data
├── myenvRS.mat              # Right Sick data
├── gwo_optimization_progress.png    # Optimization visualization
└── final_model_training.png        # Training results visualization
```

## 📝 License

This project is open source and available under the MIT License.

## 👥 Contributing

Contributions, issues, and feature requests are welcome. Feel free to check issues page if you want to contribute.
