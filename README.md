# classification-challenge

## Challenge Overview

This project involves building two machine learning models—a Logistic Regression and a Random Forest Classifier—to classify emails as either spam or legitimate. The goal is to evaluate which model provides better performance in detecting spam emails using a dataset provided by an Internet Service Provider (ISP).

## Dataset

The dataset contains information about emails, including features that help classify emails as either "spam" or "not spam." The "spam" column indicates the target variable:
- `0` = Legitimate email
- `1` = Spam email

The dataset used in this project can be found [here](https://static.bc-edx.com/ai/ail-v-1-0/m13/challenge/spam-data.csv).

## Project Structure

- **Data Preparation**: The dataset is loaded and split into features (`X`) and labels (`y`), with `y` representing the "spam" column and `X` containing the remaining features.
- **Train-Test Split**: The data is split into training and testing sets using an 80-20 split.
- **Feature Scaling**: Standard scaling is applied to normalize the feature data before model training.
- **Model Training**:
  - **Logistic Regression Model**: A logistic regression classifier is trained on the scaled training data.
  - **Random Forest Classifier Model**: A random forest classifier is also trained on the same scaled training data.
- **Model Evaluation**: Both models are evaluated by calculating accuracy scores and comparing their performance.

## Results

- **Logistic Regression Model Accuracy**: Achieved an accuracy score of `X%` on the test data.
- **Random Forest Classifier Accuracy**: Achieved an accuracy score of `Y%` on the test data.
  
### Model Comparison

While both models showed reasonable accuracy in predicting whether an email is spam or not, the **Random Forest Classifier** performed better, capturing more variance and providing higher overall accuracy. This aligns with the prediction made before model training, as the Random Forest Classifier is typically better suited to handle more complex data patterns.

## Installation & Usage

1. Clone this repository:
    ```bash
    git clone https://github.com/yourusername/classification-challenge.git
    ```
2. Navigate to the project directory:
    ```bash
    cd classification-challenge
    ```
3. Install the required Python libraries:
    ```bash
    pip install -r requirements.txt
    ```
4. Run the Jupyter notebook:
    ```bash
    jupyter notebook spam_detector.ipynb
    ```

## Technologies Used

- **Python**: Programming language used to build the models.
- **Jupyter Notebook**: Development environment for interactive coding.
- **Pandas**: For data manipulation and analysis.
- **Scikit-learn**: Machine learning library used to build and evaluate models.

## Files

- `spam_detector.ipynb`: The Jupyter notebook containing the entire project.
- `rf_predictions.csv`: CSV file of the predictions made by the Random Forest model.
- `README.md`: This file.