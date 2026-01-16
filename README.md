
---

## 🔹 Part 1: Model Training

- Loaded and explored the **Churn Modelling dataset**
- Removed irrelevant columns (`RowNumber`, `CustomerId`, `Surname`)
- Dropped the `Exited` column to avoid data leakage
- Applied:
  - `StandardScaler` for numerical features
  - `OrdinalEncoder` for categorical features
- Built an **Artificial Neural Network (ANN)** using TensorFlow/Keras
- Used:
  - ReLU activation for hidden layers
  - Linear activation for the output layer (regression)
- Trained the model using **Mean Squared Error (MSE)** loss
- Saved:
  - Trained model as `model.h5`
  - Preprocessing pipeline as `preprocessor.pkl`

---

## 🔹 Part 2: Model Prediction

- Loaded the saved ANN model (`model.h5`)
- Loaded the saved preprocessing pipeline
- Applied **the same preprocessing** to new input data
- Generated predictions for **Estimated Salary**
- Ensured no retraining or data leakage during prediction

---

## 🔹 Part 3: Streamlit Application & Deployment

- Built an interactive **Streamlit web application**
- Users can input customer details through a UI
- The app:
  - Applies the trained preprocessing pipeline
  - Uses the trained ANN model
  - Predicts and displays the **Estimated Salary**
- Designed for easy deployment on platforms like:
  - Streamlit Community Cloud
  - Render
  - Localhost

---

## 🛠️ Tech Stack

### 🔹 Programming & Libraries
- **Python**
- **NumPy**
- **Pandas**
- **Matplotlib / Seaborn** (EDA & visualization)

### 🔹 Machine Learning
- **Scikit-learn**
  - ColumnTransformer
  - StandardScaler
  - OrdinalEncoder
- **TensorFlow / Keras**
  - Artificial Neural Networks (ANN)

### 🔹 Model Deployment
- **Streamlit**
- **Pickle** (for saving preprocessing pipeline)

---

## ⚠️ Important Note

The `EstimatedSalary` feature in the Churn Modelling dataset is **synthetically generated** and does not have strong correlation with other features.  
Therefore, this project primarily demonstrates:
- Correct ML pipeline design
- Proper preprocessing handling
- Model training and reuse
- Deployment workflow  

rather than high predictive accuracy.

---

## 👩‍💻 Author

**Prerna Prashar**  
- AIML Student  
- Interested in Machine Learning, Deep Learning, and Model Deployment  
- Passionate about building end-to-end ML projects  

---

## 📜 License

This project is for **educational and learning purposes**.
