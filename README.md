# Heart Disease Prediction

## Project Description
This project leverages machine learning models to predict the likelihood of heart disease based on patient data. It uses models such as Random Forest, XGBoost, and a Stacking model (Random Forest + XGBoost) to build a highly accurate classifier. Feature selection and hyperparameter tuning are also applied for optimization.

## Project Files
- `main_code.ipynb`: Jupyter notebook containing the full workflow:
  - Data loading and preprocessing.
  - Exploratory Data Analysis (EDA).
  - Model training and evaluation.
  - Feature selection and hyperparameter tuning.
  - Prediction generation for the test set.
- `submission_last.csv`: The final submission file containing predictions for the test dataset.
- `requirements.txt`: A list of necessary Python libraries to run this project.

## Setup Instructions

1. **Clone the repository**:
    ```bash
    git clone https://github.com/codingxperience/heart-disease.git
    cd your-repo
    ```

2. **Install dependencies**: Use the `requirements.txt` file to install all necessary Python libraries.
    ```bash
    pip install -r requirements.txt
    ```

3. **Run the Jupyter notebook**: Open the `notebook-heartdisease.ipynb` notebook in Jupyter and run the cells sequentially to generate predictions. You can install Jupyter via:
    ```bash
    pip install notebook
    ```

4. **Then run**:
    ```bash
    jupyter notebook
    ```

## Final Output
After running the notebook, the `submission_last.csv` file will be generated, containing the predictions for the test dataset. This file consists of:
- `id`: Unique identifier for each test sample.
- `target`: Predicted value (0 or 1) for heart disease.

## Model Summary
The following models are trained and evaluated in this project:
- **Random Forest**: A basic model with feature importance ranking.
- **XGBoost**: Gradient boosting method for higher performance.
- **Stacking Model**: A meta-model using XGBoost with Random Forest and XGBoost base learners for improved accuracy.

## Feature Selection & Hyperparameter Tuning
- **Feature Selection**: Recursive Feature Elimination (RFE) is applied to select the top features for Random Forest and XGBoost models.
- **Hyperparameter Tuning**: RandomizedSearchCV is used to efficiently search for the best hyperparameters for both Random Forest and XGBoost.

## Results
The final stacking model (Random Forest + XGBoost) achieved the highest accuracy in validation and test phases. The model's accuracy was confirmed by the leaderboard results of the Data Science Nigeria X Microsoft 2024 AI Bootcamp Qualification Hackathon.

## Dependencies
- **Python**: Version 3.8 or higher.
- See `requirements.txt` for the full list of dependencies.

## How to Contribute
Feel free to open issues or submit pull requests if you'd like to improve the code or provide suggestions for optimization.
