# Real-Time Network Traffic Prediction

This project leverages **deep learning techniques**, specifically **Long Short-Term Memory (LSTM)** and **Gated Recurrent Units (GRU)**, to predict real-time network traffic. By analyzing real-world traffic data, we aim to provide insights into traffic patterns and improve the accuracy of network traffic forecasting.

## 📜 Introduction

The project applies advanced time-series models to forecast network traffic. Using a dataset from the **University of Leipzig**, we compare the effectiveness of LSTM and GRU models for future traffic predictions. The evaluation metrics include:

- **Root Mean Square Error (RMSE)**
- **Mean Absolute Percentage Error (MAPE)**

The results show that **LSTM outperforms GRU**, offering better generalization and accuracy.

---

## 📊 Dataset Overview

- **Source:** University of Leipzig's network traffic data
- **Duration:** Monitored over 4 days and 18 hours
- **Entries:** 6,491
- **Columns:** 26
- **Traffic Types:** TCP, UDP, ICMP
- **Key Features:**
  - `Algorithm`: Model type (e.g., GRU, LSTM)
  - `Look_Back`: Number of previous time steps used for input sequences
  - `Look_Ahead`: Prediction horizon (number of future time steps)
  - `Neuron1`, `Neuron2`, `Neuron3`: Neuron counts in network layers
  - `MAPE (1 Step to 20 Steps)`: MAPE values for multi-step predictions

---

## 🚀 Project Objectives

1. **Data Preprocessing:** Clean and normalize the dataset to prepare it for model training.
2. **Model Implementation:** Build and train LSTM and GRU models for time-series forecasting.
3. **Performance Evaluation:** Compare LSTM and GRU models using RMSE and MAPE.
4. **Model Optimization:** Tune hyperparameters using grid search for optimal performance.
5. **Validation:** Test the models on unseen data to ensure practical applicability.

---

## 📅 Timeline

### Week 1-2
- Data collection and preprocessing: Filtering, anonymization, and time-series conversion.

### Week 3-4
- Implementation of LSTM and GRU models (encoder-decoder architecture).

### Week 5-6
- Initial model training and evaluation using MSE.

### Week 7-8
- Model performance evaluation.

### Week 9-10
- Hyperparameter tuning using grid search.

### Week 11-12
- Final testing and validation.

---

## 🛠 Preprocessing Details

1. **Handling Missing Values:**
   - Address missing entries in `Neuron1`, `Neuron2`, and `Neuron3`.
2. **Normalization:**
   - Apply Gaussian transformation to standardize input features.

---

## 📈 Results

- **LSTM** demonstrates superior performance, achieving lower RMSE and MAPE values compared to GRU.
- LSTM consistently performs better for longer-term predictions, making it the more reliable choice for real-time network traffic forecasting.

### Key Metrics
| Metric       | LSTM         | GRU          |
|--------------|--------------|--------------|
| RMSE (Test)  | Lower        | Higher       |
| MAPE (1-20)  | Lower Errors | Higher Errors|

---

## 💡 Conclusion

This project highlights the capability of recurrent neural networks in predicting complex, non-linear time-series data. LSTM networks, known for their ability to capture long-term dependencies, outperform GRUs for this specific task, making them a valuable tool for network traffic prediction.

---


