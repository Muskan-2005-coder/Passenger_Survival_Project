# 🚢 Passenger Survival Prediction using Machine Learning

This project implements a machine learning pipeline to predict survival on the Titanic. The solution is based on detailed feature engineering and exploratory data analysis using the classic Titanic dataset from Kaggle.

---

## 📁 Project Structure

- `S_Prediction.ipynb`: Python script containing data preprocessing, model training, evaluation, and prediction on test data.
- `train.csv`: Training dataset with features and survival labels.
- `test.csv`: Test dataset used for generating final predictions.
- `resultfile.csv`: Output file containing predicted survival values for the test data.
---

## ✅ Requirements

- Python 3.x
- pandas
- numpy
- matplotlib
- seaborn
- scikit-learn

---

## ⚙️ Setup

1. Clone the repository:

    ```bash
    git clone https://github.com/Muskan_2005-coder/Passenger_Survival.git
    cd Passenger_Survival
    ```

2. Install the required packages:

    ```bash
    pip install pandas numpy matplotlib seaborn scikit-learn
    ```

---

## 🚀 Usage

1. **Training the Model**:
    - The model is trained on `train.csv` using:
        - **Random Forest Classifier**
        - Train/Test split (80/20)
        - Accuracy evaluation

2. **Feature Engineering Includes**:
    - Filling missing values
    - Creating new features like `AgeGroup` and `Title`
    - Dropping irrelevant columns like `Cabin`, `Ticket`, and `Name`
    - Encoding categorical features like `Sex`, `Embarked`, `Title`


3. **Prediction Output**:
    - The model predicts survival for passengers in `test.csv`
    - Outputs a `resultfile.csv` in the required Kaggle format:
      ```
      PassengerId,Survived
      892,0
      893,1
      ...
      ```

---

## 📊 Example Output

```text
Model Accuracy (Validation): 83.8%
