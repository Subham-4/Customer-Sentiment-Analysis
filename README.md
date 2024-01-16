# Customer Sentiment Analysis

This project focuses on customer sentiment analysis using machine learning algorithms. The dataset used in this project is loaded from the 'Data Vortex_Round 2.csv' file. The goal is to predict customer responses based on various features like age, education, marital status, spending behavior, and others.

## Data Preprocessing

The dataset undergoes several preprocessing steps:

1. **Age Calculation:** Age is calculated from the 'DtCustomer' column and added as a new feature.

2. **Categorical Data Transformation:**
   - 'Marital' values are transformed into binary categories ('Alone' or 'Not Alone').
   - 'Education' values are transformed into binary categories ('Degree' or 'No Degree').

3. **Feature Engineering:**
   - 'Child' is created as the sum of 'Kidhome' and 'Teenhome'.
   - 'Spending' is calculated as the sum of spending on various product categories.
   - 'Purchases' is calculated as the sum of different types of purchases.
   - 'NumCmpResponce' is calculated as the sum of responses to various campaigns.

4. **Feature Selection:**
   - Only relevant features are kept for analysis.

5. **Null Values Handling:**
   - Any null values in the dataset are addressed.

## Model Training

Three different machine learning models are trained on the preprocessed data:

1. **XGBoost Classifier:** Achieves an accuracy of approximately 88% on the test set.

2. **Neural Network:** A simple neural network with dropout layers. Achieves an accuracy of around 86% on the test set.

3. **Logistic Regression:** Achieves an accuracy of approximately 86% on the test set.

4. **K-Nearest Neighbors (KNN):** Achieves accuracy scores around 84%.

## Evaluation and Visualization

Various metrics such as accuracy, F1 score, and confusion matrices are used to evaluate model performance. Confusion matrices are displayed using matplotlib to visualize the true positive, true negative, false positive, and false negative values.

## Usage

1. Clone the repository:

   ```bash
   git clone https://github.com/your-username/customer-sentiment-analysis.git
   ```

2. Install the required dependencies:

   ```bash
   pip install numpy pandas xgboost scikit-learn matplotlib tensorflow
   ```

3. Run the Jupyter Notebook or Python script to train and evaluate the models.


## Acknowledgments

- The project uses various machine learning models and libraries. Credits to the authors and contributors of XGBoost, scikit-learn, TensorFlow, and others.
