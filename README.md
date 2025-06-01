# RelSTM: Relative Long Short-Term Memory for Improved Sequential Prediction

This repository contains the implementation and results of **RelSTM**, a modified LSTM architecture that introduces a **Relative Block** and **Feature Block** to enhance sequence prediction performance, particularly for time series tasks such as asset price forecasting.

## 📌 Abstract

Traditional Long Short-Term Memory (LSTM) networks are widely used for sequential modeling but often struggle with vanishing gradients and loss function inefficiencies. RelSTM improves upon the standard LSTM by introducing additional architectural components that preserve signals and enhance directional sensitivity.

Our experiments demonstrate that RelSTM generalizes better than standard LSTM models on validation datasets.

---

## 🖼️ Figure 1: Predictions at Epoch 40

![Prediction Plot](https://github.com/mahan100/ReLSTM/blob/main/predictions_plot_epoch%3D40.png)

---

## 📊 Results

| Model   | Parameters | MSE           | MAE        | RMSE       |
|---------|------------|---------------|------------|------------|
| RelSTM  | 6,861 (26.80 KB) | 7,603,377.42 | 2,099.91   | 2,757.42   |
| LSTM    | 21,025 (82.13 KB) | 9,242,699.18 | 2,278.84   | 3,040.18   |

## 🧠 Features

- ✅ Relative Block for contextual awareness  
- ✅ Feature Block for signal enhancement  
- ✅ Better generalization on time series data  
- ✅ Reduced parameter count compared to standard LSTM  

## 📁 Structure

```bash
.
├── model/                # Implementation of RelSTM and LSTM
├── data/                 # Dataset used for training and evaluation
├── results/              # Output metrics and plots
├── paper/                # LaTeX source of the academic paper
├── README.md
└── requirements.txt      # Required Python packages
