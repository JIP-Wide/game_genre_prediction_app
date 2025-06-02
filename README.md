# Game Genre Prediction Demo
An interactive Streamlit web application for predicting video game genres based on user reviews and metadata using a machine learning model.


## Project Overview

This project demonstrates a full ML pipeline for multi-class classification in the video game domain. It includes:

- Data preprocessing of structured metadata and unstructured user reviews
- Feature engineering (TF-IDF, OneHotEncoding, and scaling)
- Class imbalance handling using SMOTETomek
- Training and optimizing an XGBoost classifier with Optuna
- Interactive deployment via a Streamlit app


## Tech Stack

- **Python 3.10+**
- **scikit-learn**, **XGBoost**, **Optuna**
- **Streamlit** (for UI)
- **pandas**, **NumPy**, **NLTK**
- **imbalanced-learn**, **joblib**


## Installation

1. Clone the repository:

```bash
git clone https://github.com/your-username/gema-genre-prediction-demo.git
cd gema-genre-prediction-demo
```

2. (Optional but recommended) Create a virtual environment:  
```bash
python -m venv .venv

# For macOS / Linux
source .venv/bin/activate

# For Windows
.venv\Scripts\activate
```

3. Install the required packages:  
```bash
pip install -r requirements.txt
```


## Usage
Start the Streamlit application locally:  
```bash
streamlit run app.py
```

The app will open in your browser at http://localhost:8501.
You can manually enter or simulate game data and get real-time genre predictions from the trained model.


## Model Pipeline

| Step                  | Description                                           |
|-----------------------|-------------------------------------------------------|
| Text preprocessing    | TF-IDF vectorization of user reviews                  |
| Categorical features  | OneHot encoding                                       |
| Numerical features    | Scaled via StandardScaler, MinMaxScaler, or RobustScaler (based on distribution) |
| Class balancing       | SMOTETomek for improved class distribution            |
| Classification model  | XGBoost with hyperparameter tuning via Optuna         |


## App Preview

![Demo Screenshot](https://link-to-your-screenshot.com/demo.png)


## Sample Results (Evaluation Metrics)

| Metric      | Score     |
|-------------|-----------|
| Accuracy    | 0.9412    |
| Log Loss    | 0.2023    |



## Credits
![DataScientest Logo](https://datascientest.com/wp-content/uploads/2022/03/logo-2021.png)

This project was carried out as part of a Data Analytics training course at the DataScientest institute  

Project carried out by:  
[Vyacheslav Goncharenko](https://www.linkedin.com/in/vyacheslavgoncharenko/)
<a href="https://www.linkedin.com/in/dein-linkedin-name" target="_blank">
  <img src="https://img.shields.io/badge/-LinkedIn-0A66C2?style=flat&logo=linkedin&logoColor=white" alt="LinkedIn" height="20"/>
</a>  
[GitHub Profile](https://github.com/JIP-Wide)

Project mentor:  
[Yaniv Benichou](https://www.linkedin.com/in/yaniv-benichou/)
<a href="https://www.linkedin.com/in/yaniv-benichou/" target="_blank">
  <img src="https://img.shields.io/badge/-LinkedIn-0A66C2?style=flat&logo=linkedin&logoColor=white" alt="LinkedIn" height="20"/>
</a>  

Data provided by:  
[Aaron Martin, Ph.D.](https://www.linkedin.com/in/aaron-martin-phd/)
<a href="https://www.linkedin.com/in/aaron-martin-phd/" target="_blank">
  <img src="https://img.shields.io/badge/-LinkedIn-0A66C2?style=flat&logo=linkedin&logoColor=white" alt="LinkedIn" height="20"/>
</a>  
(https://www.kaggle.com/datasets/aaronrmartin/video-games-gameplay-reviews-sentiment-scores)
