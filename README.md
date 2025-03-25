# Movie Rating Prediction

## Project Overview
This project focuses on predicting movie ratings based on various features using machine learning techniques. The model is trained in **Google Colab**, leveraging datasets and saving trained models for future use.

## 📁 Repository Structure
```
📦 Movie-Rating-Prediction
 ┣ 📂 data            # Contains datasets (CSV files)
 ┣ 📂 models          # Contains trained models (e.g., .pkl files)
 ┣ 📜 README.md       # Project documentation
```

##  How to Run the Project

1. **Clone the Repository:**  
   ```bash
   git clone https://github.com/rithikaedara/Movie-Rating-Prediction.git
   cd Movie-Rating-Prediction
   ```

2. **Prepare the Data:**  
   - The dataset is available in the `data` folder.
   - Ensure you have the necessary dependencies installed (e.g., pandas, scikit-learn, xgboost).

3. **Load and Use the Model:**  
   - The trained model is available in the `models` folder.
   - You can load and use it in a Python script:
     ```python
     import pickle
     with open('models/xgboost_movie_rating_model.pkl', 'rb') as file:
         model = pickle.load(file)

This repository contains all necessary files to understand and use the model. 





