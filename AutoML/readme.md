# UCI Adult Income Classification

## Overview
The repository contains Python code for UCI Adult Income dataset in the Jupyter notebook, and raw data files from the source.

The project aims to create predictive model to classify participants income into two groups (<=50K and >50K). In this project, we utilized AutoML framework from TPOT for model selection and hyperparameter tunning. Then we followed-up with performing comparative study with traditional ML pipeline and manual hyperparameter tuning. In comparison, the manual process resulted in a higher accuracy score in less time.


## Instructions

### Libraries
- tpot
- scikit-learn
- NumPy
- pandas
- matplotlib.pyplot
- seaborn

### Files:
- Train data: data/adult.data
- Test data: data/adult.test

### Execution
- file: adult_income.ipynb
- The jupyter notebook is equipped with necessary libraries need for smooth run.
- Run all cells in the notebook to process the following in sequential order:
    - Data loading
    - Data preprocessing that includes imputing missing values with KNN model, scaling numerical features using scikit-learn StandardScaler, and one-hot-encode categorical features.
    - Used TPOT AutoML package to automatically perform model selection and hyperparameter tuning. The framework identified Gradient Descent algorithm and achieved accuracy 87.06%. Note that the package creates tpot_pipeline.py to help with running the model manually after making necessary changes.
    - Used the same Gradient Descent algorithm and iteratively tuned hyperparameters and achieved accuracy of 87.52%.
    - Detailed comparative study was performed and concluded that both the approaches assisted in the process. However, it is best to use AutoML in model selection and random grid search in hyperparameter tuning.

## Contributing

Feel free to contribute to the project by opening issues or submitting pull requests. Please follow coding standards and provide clear documentation for any changes.

## License

This project is licensed under the [MIT License] (LICENSE).
