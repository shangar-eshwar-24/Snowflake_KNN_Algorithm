# Gender Classification using Snowflake & KNN

This project demonstrates an **end-to-end machine learning pipeline** that connects **Snowflake** with **Python**, fetches data, trains a **K-Nearest Neighbors (KNN)** model for gender classification, evaluates performance, and saves the trained model for reuse.

---

## 🚀 Project Overview
- Connects to a **Snowflake database** using `snowflake-connector-python`
- Fetches gender-related data into a Pandas DataFrame
- Preprocesses and encodes labels
- Trains a **KNN classifier** using Scikit-learn
- Evaluates model accuracy and classification metrics
- Saves and loads the trained model using **Pickle** and **Joblib**

---

## 🛠️ Tech Stack
- **Python**
- **Snowflake**
- **Pandas**
- **Scikit-learn**
- **Pickle & Joblib**

---

## 📂 Project Structure
```
project-root/
├── model.pkl            # Trained ML model
├── main.py / notebook.ipynb
├── README.md
└── requirements.txt
```

---

## ⚙️ Installation

```bash
# Install required libraries
pip install snowflake-connector-python pandas scikit-learn joblib
```

---

## 🔗 Snowflake Connection
The project connects to Snowflake using the following parameters:
- User
- Password
- Account Identifier
- Database & Schema
- Warehouse

> ⚠️ **Security Note:** Do not expose Snowflake credentials in public repositories. Use environment variables or `.env` files instead.

---

## ▶️ Workflow
1. Connect Python to Snowflake
2. Fetch data using SQL query
3. Encode gender labels (`Male → 0`, `Female → 1`)
4. Split dataset into training and testing sets
5. Train KNN model (`k = 3`)
6. Evaluate accuracy and classification report
7. Save and reload the trained model

---

## 📊 Model Evaluation
- **Algorithm:** K-Nearest Neighbors (KNN)
- **Evaluation Metrics:**
  - Accuracy Score
  - Precision, Recall, F1-Score

---

## 💾 Model Persistence
The trained model is saved using:
- `pickle`
- `joblib`

This allows the model to be reused without retraining.

---

## 📈 Results
- Achieved reliable accuracy on the test dataset
- Model successfully predicts gender classes

---

## 🧠 Future Enhancements
- Use advanced models (Logistic Regression, SVM, Random Forest)
- Hyperparameter tuning for optimal `k`
- Add data visualization
- Deploy model using Flask or FastAPI

---

## 🤝 Contributing
Contributions are welcome. Fork the repository and submit a pull request.

---

## 📄 License
This project is licensed under the MIT License.

---

## 👤 Author
**Shangaranarayanan M**  
GitHub: https://github.com/shangar-eshwar-24/Snowflake_KNN_Algorithm

