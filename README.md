# Comment Toxicity Detection System

## AIM
To develop an AI-based system capable of detecting and classifying toxic comments in real-time,  
ensuring safer online interactions.

---

## OBJECTIVES
1. Create a hybrid CNN–RNN (LSTM) model for comment classification.  
2. Classify comments into toxicity levels: **toxic, severe toxic, obscene, threat, insult, identity_hate**.  
3. Deploy the model for real-time use with a user-friendly interface.  
4. Improve detection of disguised toxic content using special characters.  
5. Ensure platform adaptability, scalability, and efficient deployment.  

---

## Dataset Description

The dataset used for this project is a multi-label text classification dataset containing online comments.  
Each comment is labeled across six toxicity categories:

- **toxic**  
- **severe_toxic**  
- **obscene**  
- **threat**  
- **insult**  
- **identity_hate**

### Dataset Characteristics
- Contains thousands of user-generated comments.  
- Each comment may belong to **multiple toxicity categories**.  
- Includes clean (non-toxic) and harmful (toxic) samples.  
- Used for training an NLP model capable of understanding context, offensive patterns, and hidden toxic variations.  

### Data Preprocessing Steps
- Removal of special characters (optional, to detect disguised toxicity).  
- Text normalization (lowercasing, trimming).  
- Tokenization and padding for equal-length sequences.  
- Conversion to embedding vectors for model input.  

---

## Model Architecture

### • Input Layer  
Accepts tokenized and embedded comments, converting raw text into numerical form suitable for neural network processing.

### • CNN Layer  
Extracts local linguistic patterns and phrase-level features indicating toxic behavior.

### • LSTM Layer  
Captures long-term dependencies and contextual relationships across sequences of words.

### • Dense Layer  
Processes extracted features to perform multi-label classification across toxicity categories.

### • Output Layer  
Produces final predictions, mapping each comment to its respective toxicity labels.

---

## Model Training

### Training Process
- The dataset is split into **training and validation sets**.  
- Comments are tokenized and converted into padded sequences.  
- An embedding layer transforms text into vector representations.  
- CNN extracts local features; LSTM captures sequence dependencies.  
- Multi-label classification uses **sigmoid activation** to output probabilities for each toxicity class.  

### Training Visualization
- Training & validation loss curves  
- Accuracy plots  
- Confusion matrix for each label  
These visualizations help monitor performance and avoid overfitting.

---

## System Overview
The **Comment Toxicity Detection System** promotes safer online communication by automatically identifying harmful or offensive comments.  
Using:

- Natural Language Processing (NLP)  
- A hybrid CNN + LSTM deep learning model  
- A Gradio-based real-time user interface  

the system ensures accurate classification, smooth deployment, and instant predictions.

---

## Key Features
- Instantly check comment toxicity through a simple interactive interface.  
- Moderators can take quick action based on prediction results.  
- Admins can update or retrain the model with ease.  
- Real-time interface ensures fast and actionable feedback.  
- Deep learning approach delivers high accuracy and adaptability.  

---

## Result 
<img width="876" height="360" alt="image" src="https://github.com/user-attachments/assets/a27e0636-6c20-44bf-ab90-1bea52ffd96c" />


