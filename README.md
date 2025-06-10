Project: MLflow Experiment Tracking Demo
========================================
This project demonstrates how to integrate MLflow into a simple machine learning workflow for experiment tracking, model logging, and evaluation.
It uses a regression task (predicting iris class) as an example, and shows how to:
* Initialize and configure an MLflow tracking URI
* Use mlflow.start_run() for clean experiment tracking
* Log model parameters, metrics, and artifacts
* Save and version models using mlflow.sklearn.log_model
* Retrieve and test saved models using MLflow’s PyFunc interface
</br>

Structure
=========
* It provides two versons of project codes:
1) project_code_short.ipynb: the short version project notebook with model training and MLflow integration. It contains the basic functions for this porject.
2) project_code_long.ipynb: the long version project notebook with model training and MLflow integration. It tries to create a reusable template for mlflow implementation based this porject. The additional functions include confusion matrix, SHAP analysis, and classification report.
* mlruns/: auto-generated directory storing experiment metadata
* mlartifacts/: stores saved model files and other outputs (for MLflow ≥ 2.x)
* requirements.txt: Dependencies that needs to be installed
</br>

Dependencies
============
* Python 3.10+
* MLflow 2.x
* scikit-learn
* pandas
* numpy
* matplotlib