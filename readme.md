# Week 2 - Halfday 2

## Missions & Activities:

### Activity 1 – ~30 minutes
- **Peer Review and Validation of Data Analysis (Halfday 1)**: Work in pairs to review and compare your code and results. Exchange the outcome of the previous acitivity. Write together 1-2 slides with a list of the key-differences concerning:
    - The result you had
    - The method you used to get to that results
- **Consolidation by the Professor**: After peer review, the professor will provide further clarification and consolidation of the concepts.

### Activity 2
- **Problem**: Data preparation. Now that you have a general understanding of our data, let’s prepare it for classification!
- **Hints**: Preparing the data involves addressing potential issues such as non-standardized data, missing values, and outliers, as well as splitting the data appropriately for evaluation (training set, validation set, and test set).
- **Tools**: scikit-learn
- **New/Consolidation of ML Glossary**: Standardization/Normalization/Rescaling, Cross-validation, One-hot encoding

## Expected Outcomes:
A continuation of your previous Jupyter notebook to prepare the data for classification. Your notebook should perform the tasks listed below. In your notebook, systematically use markdown cells to:
- Explain the goal of your code
- Comment on the results
- Provide direct answers to **all** the questions listed below (Section [Questions](#questions))

## Tasks – Preprocessing
0.  Copy & Paste your notebook (the .ipynb file) from the previous part in this folder.
    In the terminal, `cd` to the project folder and run the following instructions:

     ```bash
        pip install poetry
        poetry install
    ```
    
    *poetry* is as package manager ([and much more](https://python-poetry.org/)). Following the previous instructions and thanks to the .toml file provided in this folder, you will have all the libraries needed (pandas, numpy, scikit-lean, etc.).
1. Separate the features (X) from the label (y)
2. Split the data into training and test sets
3. Impute missing values
4. Rescale/standardize the features:
    - Explore the differences between Min-Max Scaler, Standard Scaler, and Robust Scaler
5. Encode the categorical features:
    - Compare One-Hot Encoding and Label Encoding in scikit-learn
6. Don't forget to *commit&push* your submission

## Questions:
At the end of the activity, you should be able to answer these questions and *justify* your answers:
- Why and when is it important to rescale/standardize the features?
- What is the difference between Min-Max Scaler, Standard Scaler, and Robust Scaler? **Hints**:
    - Understand the formulas used for the Min-Max Scaler, Standard Scaler.
    - Explain the possible impact of outliers on rescaling.
- Should I "fit" my scaler:
    - On the training set only?
    - On the test set only?
    - On both datasets (conjointly or separately)?
- Feature Encoding:
    - What does the `OneHotEncoder` do?
    - How does it differ from the `LabelEncoder`? When should you use one instead of the other?