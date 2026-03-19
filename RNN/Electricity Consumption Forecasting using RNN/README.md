
# Electricity Consumption Forecasting using RNN

---

## 1. Problem Statement

Electricity consumption changes over time due to factors like daily usage patterns, peak hours, and demand fluctuations.  
Accurate prediction of electricity load is important for efficient power management and grid stability.

The goal of this project is to build a time-series forecasting model that predicts future electricity consumption based on past data using a Recurrent Neural Network (RNN).

---

## 2. Dataset Description

We used the PJM Hourly Energy Consumption Dataset, which contains historical electricity load data.

### Features:
- Datetime → Timestamp of electricity usage
- PJME_MW → Electricity load in Megawatts (MW)

### Characteristics:
- Hourly time-series data
- Real-world electricity consumption
- Suitable for sequence modeling

---

## 3. What is RNN?

A Recurrent Neural Network (RNN) is a type of neural network designed for sequential data.

Unlike traditional models, RNNs maintain a hidden state that allows them to remember information from previous time steps.

### Why RNN?
- Captures time dependencies
- Learns patterns across sequences
- Suitable for time-series forecasting

In this project, the RNN uses past electricity values to predict the next value.

---

## 4. Model Implementation

### Steps:

1. Data Preprocessing:
   
2. Sequence Creation:
   
3. Model Architecture:
  
4. Training:
   
---

## 5. Model Performance

The model was evaluated using Root Mean Squared Error (RMSE).

### Result:
- RMSE ≈ 417 MW

### Interpretation:
- The model captured temporal patterns effectively
- Predictions closely follow actual values
- Error is low compared to the overall data scale

---

## Conclusion

The RNN model successfully learned time-based patterns in electricity consumption and provided accurate short-term predictions.  
This shows the effectiveness of sequence models in real-world forecasting problems.
