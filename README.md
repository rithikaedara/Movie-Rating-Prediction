# Movie Rating Prediction

## 📌 Project Overview
This project aims to predict IMDb movie ratings using machine learning techniques. The dataset includes movie details such as genre, duration, director, and actors. We preprocess the data, train an XGBoost model, and evaluate its performance.

## 📂 Repository Structure
```
Movie-Rating-Prediction/
│── data/
│   ├── IMDb Movies India.csv
│   ├── cleaned_IMDb_Movies_India.csv (processed data)
│── models/
│   ├── xgboost_movie_rating_model.pkl (saved model)
│── notebooks/
│   ├── movie_rating_prediction.ipynb (main notebook)
│── README.md (project documentation)
```

## 🔧 Installation & Setup
1. Clone the repository:
   ```bash
   git clone https://github.com/rithikaedara/Movie-Rating-Prediction.git
   cd Movie-Rating-Prediction
   ```
2. Install required dependencies:
   ```bash
   pip install -r requirements.txt
   ```
3. Run the Jupyter Notebook in Google Colab or locally.

## 🚀 How to Run the Model
1. **Preprocess the Data**: The notebook contains steps for handling missing values and feature engineering.
2. **Train the Model**: We train an XGBoost model to predict IMDb ratings.
3. **Make Predictions**: The model can be used to predict ratings for new movies.

## 📊 Example Usage
```python
import pickle
import pandas as pd

# Load the model
with open('models/xgboost_movie_rating_model.pkl', 'rb') as f:
    model = pickle.load(f)

# Create a sample input
sample_data = pd.DataFrame({
    'Year': [2022],
    'Duration': [120],
    'Genre': ['Drama'],
    'Votes': [5000],
    'Director': ['Christopher Nolan'],
    'Actor 1': ['Leonardo DiCaprio'],
    'Actor 2': ['Tom Hardy'],
    'Actor 3': ['Joseph Gordon-Levitt']
})

# Predict rating
predicted_rating = model.predict(sample_data)
print("Predicted IMDb Rating:", predicted_rating)
```

## 📜 License
This project is for educational purposes only.

---
### ✅ Final Steps
📌 **Commit and push the README.md to GitHub**:
```bash
git add README.md
git commit -m "Added README file"
git push origin main
```
Then, proceed with the submission!

