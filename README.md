

---

# Water Potability Predictor

A machine learning project that predicts water potability to ensure safe drinking water in light of increasing pollution. This project leverages algorithms like Support Vector Machine, Decision Tree, and K-Nearest Neighbor to classify water samples as potable or non-potable based on water quality indicators.

## Introduction
Access to safe drinking water is vital, but pollution remains a persistent threat to water quality worldwide. This project provides a machine learning solution for predicting water potability, potentially aiding efforts to ensure safer drinking water.

## Dataset
The dataset includes several key indicators of water quality:
- **pH**
- **Hardness**
- **Solids**
- **Chloramines**
- **Sulfate**
- **Conductivity**
- **Organic Carbon**
- **Trihalomethanes**
- **Turbidity**

The dataset was imbalanced, so **SMOTE (Synthetic Minority Oversampling Technique)** was applied to improve model performance.

## Features
The model uses these features to determine water potability, assessing qualities that impact water safety and quality.

## Methodology

### 1. Data Preprocessing
   - **Data Imbalance**: Addressed with **SMOTE** to balance the classes.
   - **Data Split**: Divided into **training (70%)** and **testing (30%)** sets.

### 2. Algorithms Used
   - **Support Vector Machine (SVM)**
   - **Decision Tree (DT)**
   - **K-Nearest Neighbor (KNN)**

### 3. Hyperparameter Tuning
   - Used **Stratified Cross-Validation (k=10)** and **GridSearch** for finding optimal parameters.

### 4. Feature Selection
   - **Sequential Feature Selection** to identify the most relevant features.

### 5. Ensemble Learning
   - Combined models to enhance generalization and overall accuracy.

## Results
The **Decision Tree** model achieved the highest accuracy at **73.75%**, followed by SVM and KNN. This result shows the potential for using machine learning in early water quality assessments.

## How to Run the Project

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/Danahalgarni/WaterPotabilityPredictor.git
   cd WaterPotabilityPredictor
   ```

2. **Install Dependencies**:
   ```bash
   pip install -r requirements.txt
   ```

3. **Run the Project**:
   ```bash
   python main.py
   ```

## Conclusion
This project demonstrates the power of machine learning in addressing environmental issues. By accurately predicting water potability, it contributes to safer water quality assessment, aiding public health and environmental safety efforts.

---
