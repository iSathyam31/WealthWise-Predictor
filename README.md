# Income Prediction Project

This project aims to predict whether a person's income exceeds $50K per year based on census data. The best performing model in this project is a **CatBoost Classifier**. Additionally, a **Streamlit** application has been created to allow users to input data and receive income predictions.

## Project Structure

The project is organized as follows:
```
Income_Prediction_Project/
│
├── data/
│ └── data.csv
│
├── model/
│ └── best_model.pkl
│ └── app.py
│
├── Adult_Census.ipynb
├── README.md
└── LICENSE
|__ requirements.txt
```


- **data/data.csv**: The dataset used for training and evaluating the models.
- **model/best_model.pkl**: The saved CatBoost Classifier model.
- **model/app.py**: The Streamlit application script.
- **Adult_Census.ipynb**: Jupyter notebook containing the data preprocessing, model training, and evaluation.

## Installation

To run this project, you need to have Python installed on your machine. You can install the required packages using the following command:

```bash
pip install -r requirements.txt
```
The required packages are listed in the `requirements.txt` file:
```
streamlit
pandas
numpy
scikit-learn
catboost
```

## Streamlit Application
To run the Streamlit application, execute the following command in your terminal:
```
streamlit run model/app.py
```
## Model Deployment
The trained CatBoost Classifier model (`best_model.pkl`) can be deployed in production to make real-time predictions.