# Fraud-Detection-Predition

**Fraud-Detection-Predition** is a Python-based project for detecting fraudulent financial transactions. It includes data exploration, model training, and an application interface for making real-time predictions.

## 📄 Overview

This project demonstrates:

- Exploratory Data Analysis (EDA) of transaction data.
- Preprocessing and feature engineering to address class imbalance.
- Building and training a machine learning model for binary classification.
- Packaging the trained model and deploying it via a simple interface (`app.py`).

##  Dataset

We use the *Fraud Detection Dataset* from Kaggle, covering various transaction features. Access it here:

[Download the dataset (Kaggle)](https://www.kaggle.com/datasets/amanalisiddiqui/fraud-detection-dataset?resource=download) :contentReference[oaicite:1]{index=1}

###  Preprocessing may include:

- Handling missing values.
- Encoding categorical variables.
- Feature scaling.
- Balancing classes using techniques like SMOTE or undersampling.

##  Directory Structure

```
|-- analysis.ipynb                 # Exploration, visualization, and modeling steps
|-- app.py                         # Application for serving model predictions
|-- fraud_detection_model.pkl      # Serialized trained model
|-- README.md                      # Project overview and instructions
```

##  Installation

1. Clone the repository:
```
   git clone https://github.com/deepshikha04yadav/Fraud-Detection-Predition.git
   cd Fraud-Detection-Predition
```
2. Create and activate a Python virtual environment:
```
python3 -m venv venv
source venv/bin/activate  # or `venv\Scripts\activate` on Windows
```
3. Install required dependencies:
```
pip install -r requirements.txt
```

## Running the Model
### From the Notebook (EDA & Training)

Open the Jupyter notebook to explore data and train the model:
```
jupyter notebook analysis.ipynb
```
### Using the Application (app.py)

Launch the app to interact with the model:
```
python app.py      # or
streamlit run app.py
```

Then access the local URL (e.g., http://127.0.0.1:5000) to submit transaction features and get predictions.

## Model Details

* __Type:__ Binary classifier (fraud vs. non-fraud).

* __Training procedure:__ Cleaned data, feature-engineered, split into train/test, trained on models such as logistic regression, random forest, or other chosen classifier.

* __Evaluation metrics:__ Because fraud is rare, you should focus on metrics like precision, recall, F1-score, and AUC rather than accuracy.

## Contributing

Contributions are welcome! To suggest improvements:

1. Fork the repository.

2. Create a new feature branch: git checkout -b my-feature.

3. Make your changes.

4. Submit a pull request for review.
