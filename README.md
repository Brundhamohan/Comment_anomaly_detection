## Overview

This project focuses on detecting anomalies using an Autoencoder deep learning model.  
The model learns the normal pattern of data and identifies abnormal inputs using reconstruction error.  
A Gradio user interface is included for interactive anomaly testing.

## Objective

The objective of this project is to build a machine learning model capable of identifying anomalies by analyzing deviations from normal data patterns.

## Dataset Details

The dataset contains numerical values representing normal and abnormal behavior.  
The Autoencoder is trained mainly on normal data so that it can:

- Learn the distribution of normal values  
- Reconstruct normal data accurately  
- Give high reconstruction error for anomalies  

## Dataset Features

- Numerical data points  
- Abnormal samples for testing  
- Preprocessed and scaled values  

## Methodology

### **Autoencoder Model**
- Encoder compresses input  
- Decoder reconstructs it  
- High reconstruction error = anomaly  

### **Data Preprocessing**
- Data cleaning  
- Scaling  
- Structured using NumPy & Pandas  

## Model Training

- Training on normal samples  
- Loss = Mean Squared Error (MSE)  
- Loss curve visualized using Matplotlib  

## Gradio Interface

A Gradio-based UI is provided to input custom values and check whether they are anomalies.

<img width="1376" height="564" alt="image" src="https://github.com/user-attachments/assets/04b88abc-9602-470e-9920-86f6157df0f0" />


## Result

The trained Autoencoder differentiates normal and abnormal inputs based on reconstruction error:  
- Low error → Normal  
- High error → Anomaly  

The model shows stable training and clear anomaly separation.

## Conclusion

This anomaly detection system is effective for identifying unusual patterns in data.  
It can be used for:

- Quality inspection  
- Monitoring systems  
- Error detection  
- Real-time anomaly alerts  
