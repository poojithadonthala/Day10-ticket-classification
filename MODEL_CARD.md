
# MODEL CARD: Support Ticket Priority Classification

## 1. Model Name
TF-IDF + Logistic Regression

## 2. Model Purpose
Classifies support tickets into four priority categories:
Critical, High, Medium, and Low.

## 3. Dataset Information
Dataset: tickets_labelled.xlsx
Total Records: 800
Training Records: 640
Testing Records: 160

Input Features:
- Ticket Title
- Ticket Description
- Channel

Target:
- Priority

## 4. Model Architecture
- TF-IDF Vectorizer
- Logistic Regression
- Class Weight: Balanced
- Random State: 42

## 5. Evaluation Metrics
Accuracy: 0.8938
Macro Precision: 0.8961
Macro Recall: 0.8819
Macro F1-Score: 0.8883

## 6. Error Analysis
Misclassified Tickets: 17
Total Test Tickets: 160

## 7. Limitations
- Performance depends on the quality of labelled tickets.
- Critical tickets have fewer training examples.
- Ambiguous descriptions may cause incorrect predictions.
- The model may not understand complex context or sarcasm.
- Predictions should be reviewed by a human before making important decisions.

## 8. Intended Use
This model is a classic machine learning baseline
for support ticket priority classification.

It can be compared with future LLM-based
classification approaches.
