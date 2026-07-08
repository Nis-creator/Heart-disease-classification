# Heart Disease Prediction

This project uses machine learning to predict the likelihood of a patient developing coronary heart disease within ten years.

## Project Overview

- Dataset: `heart-disease-prediction_ca9d91fb-0255-41f2-9e92-d5cd33edca38.csv`
- Approach: Logistic Regression classification
- Feature selection: top 10 features using `SelectKBest` with `f_classif`
- Evaluation metrics: accuracy, confusion matrix, classification report
- Visualization: confusion matrix heatmap

## Files

- `Heart_disease2.ipynb` - Jupyter notebook containing the complete data loading, preprocessing, feature selection, model training, evaluation, and visualization pipeline.
- `heart-disease-prediction_ca9d91fb-0255-41f2-9e92-d5cd33edca38.csv` - dataset used to train and evaluate the model.
- `.gitignore` - ignores common Python, notebook, and environment files.
- `.gitattributes` - ensures `.ipynb` files are treated as binary to avoid line ending conversion issues.

## Requirements

- Python 3.x
- pandas
- numpy
- scikit-learn
- seaborn
- matplotlib

## How to Run

1. Activate the project virtual environment:

```powershell
& .\venv\Scripts\Activate.ps1
```

2. Open `Heart_disease2.ipynb` in Jupyter Notebook or JupyterLab.
3. Run the notebook cells to load the data, train the model, and view the evaluation output.

## Notes

- The notebook checks for missing values and drops any rows containing them.
- The model training step is skipped if the training set contains only a single class.
- The confusion matrix plot is displayed only when the model is successfully trained.
