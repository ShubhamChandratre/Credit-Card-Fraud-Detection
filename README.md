
# Credit Card Fraud Detection

This project aims to build a machine learning model to detect fraudulent credit card transactions. The dataset used for training and testing contains anonymized transaction features and labels indicating whether a transaction is fraudulent or not.

## Project Overview

Credit card fraud is a significant problem in financial systems. Detecting fraudulent transactions in real time is critical to preventing monetary losses. In this project, we use machine learning techniques to identify fraudulent transactions based on historical data.

## Dataset

The dataset used for this project is highly imbalanced, as fraudulent transactions represent a very small fraction of the total. The features in the dataset are anonymized for confidentiality purposes.

- **Total transactions**: `284,807`
- **Fraudulent transactions**: `492`
- **Non-fraudulent transactions**: `284,315`

## Key Features of the Notebook

1. **Data Preprocessing**: 
   - Standardization of features.
   - Handling class imbalance using undersampling techniques.
   
2. **Exploratory Data Analysis**:
   - Visualization of fraud vs. non-fraud transaction distributions.
   - Correlation matrix and heatmap for feature relationships.
   
3. **Model Training**:
   - The model used is **Logistic Regression**.
   - Training on an undersampled dataset to balance the fraud/non-fraud class distribution.

4. **Model Evaluation**:
   - Confusion matrix (for both training and test data).
   - Receiver Operating Characteristic (ROC) curve and Area Under Curve (AUC) score.
   - Precision, recall, F1-score.

## Installation

### Prerequisites

Ensure you have the following dependencies installed:

- Python 3.x
- Jupyter Notebook
- Pandas
- Numpy
- Scikit-learn
- Seaborn
- Matplotlib

You can install these dependencies via pip:

```bash
pip install pandas numpy scikit-learn seaborn matplotlib
```

### Running the Notebook

1. Clone the repository:

```bash
git clone https://github.com/yourusername/Credit-Card-Fraud-Detection.git
```

2. Navigate to the project directory:

```bash
cd Credit-Card-Fraud-Detection
```

3. Launch Jupyter Notebook:

```bash
jupyter notebook
```

4. Open the `Credit-Card-Fraud-Detection.ipynb` notebook and run all cells to reproduce the analysis.

## Evaluation Metrics

- **Confusion Matrix**: Helps understand the performance of the model by comparing true vs predicted values.
- **ROC-AUC Curve**: The ROC curve visualizes the trade-off between true positive rate (recall) and false positive rate, while AUC quantifies the overall performance of the classifier.

## Results

- The logistic regression model performed well on the undersampled dataset with an AUC score of approximately 0.90.
- The confusion matrix on test data shows good performance in identifying fraudulent transactions with low false positives.

## Visualizations

- **Correlation Heatmap**: Visualizes correlations between features.
- **ROC Curve**: Shows the true positive rate vs false positive rate of the model.
- **Confusion Matrices**: Display both training and test data performance.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
