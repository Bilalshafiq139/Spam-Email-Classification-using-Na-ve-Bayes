# Spam-Email-Classification-using-Na-ve-Bayes
This repository contains a Python script that implements Spam Email Classification using Naïve Bayes classifiers.




# Spam Email Classification using Naïve Bayes

## Overview
This repository contains a Python script that implements **Spam Email Classification** using **Naïve Bayes classifiers**. The model predicts whether an email is **spam** or **ham (not spam)** based on its textual content.

---

## **Problem Statement**
Email spam is a major issue, and filtering spam messages effectively is crucial for security and productivity. This project builds a **Naïve Bayes-based classifier** to automatically categorize emails as spam or ham based on text-based features.

### **Dataset Description**
The dataset used in this project is from [**Kaggle: SMS Spam Collection Dataset**](https://www.kaggle.com/datasets/uciml/sms-spam-collection-dataset). The dataset includes:
- **Text**: The email content.
- **Target (Label)**:
  - `0`: Ham (not spam).
  - `1`: Spam.

---

## **How the Script Works**
1. **Data Preprocessing**:
   - Loads the dataset and removes unnecessary columns.
   - Converts categorical labels (`spam`, `ham`) into numerical values (`0`, `1`).
   - Removes duplicate entries and missing values.
2. **Exploratory Data Analysis (EDA)**:
   - Analyzes the dataset distribution.
   - Visualizes spam vs. ham message length, word count, and sentence count.
3. **Text Processing**:
   - Converts text to lowercase.
   - Removes special characters, punctuation, and stopwords.
   - Applies **stemming** using the **Porter Stemmer**.
4. **Feature Extraction**:
   - Uses **CountVectorizer** to convert text into numerical vectors.
5. **Model Training**:
   - Splits the dataset into **training (80%)** and **testing (20%)** sets.
   - Trains **Naïve Bayes classifiers**:
     - **Gaussian Naïve Bayes**
     - **Multinomial Naïve Bayes**
     - **Bernoulli Naïve Bayes**
6. **Model Evaluation**:
   - Computes **Accuracy**, **Precision**, and **Confusion Matrix** for all models.
   - Identifies the best-performing classifier.
7. **Visualization**:
   - Displays word cloud of most common spam/ham words.
   - Plots histogram and heatmap of spam/ham word distribution.

---

## **Dependencies**
Ensure you have the following Python libraries installed:
```sh
pip install numpy pandas nltk seaborn matplotlib scikit-learn wordcloud
```

---

## **How to Run the Script**
1. Clone the repository:
   ```sh
   git clone <repository_url>
   ```
2. Navigate to the project folder:
   ```sh
   cd <project_folder>
   ```
3. Run the Python script:
   ```sh
   python spam_email_classification.py
   ```
4. Follow the output to view model performance and classification results.

---

## **Contributing**
Contributions are welcome! Feel free to fork this repository and submit a pull request with improvements or additional features.

