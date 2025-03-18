# GrowthLink-Task_DS
# 🚢 Titanic Survival Prediction  

## 📌 Project Overview  
This project aims to develop a **Machine Learning model** to predict whether a passenger survived the **Titanic disaster**. Using historical passenger data, the model classifies individuals based on features like age, gender, ticket class, fare, and cabin information.  

## 📂 Project Structure  
📁 Titanic-Survival-Prediction  
│-- 📄 README.md  # Project Documentation  
│-- 📄 titanic_survival.ipynb  # Jupyter Notebook with full code  
│-- 📄 requirements.txt  # List of required Python libraries  
│-- 📄 titanic_model.pkl  # Saved trained model  
│-- 📁 data  
│   │-- train.csv  # Training dataset  
│   │-- test.csv  # Testing dataset  
│-- 📁 images  
│   │-- confusion_matrix.png  # Confusion Matrix visualization  
│   │-- survival_rate.png  # Survival Rate plot  

## 📊 Dataset Details  
- **Source:** [Kaggle Titanic Dataset](https://www.kaggle.com/datasets/brendan45774/test-file)  
- **Target Variable:** `Survived` (1 = Survived, 0 = Did not survive)  
- **Features Used:**  
  - **Numerical:** `Age`, `Fare`, `Pclass`  
  - **Categorical:** `Sex`, `Embarked`, `Cabin`, `Ticket`  

## ⚙️ Data Preprocessing Steps  
✔ **Handled Missing Values** (Age, Fare, Embarked filled with median/mode)  
✔ **Dropped Unnecessary Columns** (`Name`, `Ticket`, `Cabin`)  
✔ **Encoded Categorical Variables** (`Sex`, `Embarked`)  
✔ **Normalized Numerical Data** (`Age`, `Fare`)  

## 📈 Model Training & Evaluation  
✔ **Model Used:** `RandomForestClassifier (n_estimators=100)`  
✔ **Training & Testing Split:** 80% Train, 20% Test  
✔ **Evaluation Metrics:**  
- Accuracy  
- Precision, Recall, F1-score  
- Confusion Matrix  

### 📊 Model Performance  
| Metric         | Score |  
|---------------|-------|  
| **Accuracy**  | 85%  |  
| **Precision** | 83%  |  
| **Recall**    | 78%  |  
| **F1-Score**  | 80%  |  

## 🚀 How to Run the Project?  
### 1️⃣ Install Dependencies  
Run the following command:  
```bash
pip install -r requirements.txt
