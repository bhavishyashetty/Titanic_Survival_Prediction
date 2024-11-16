# Titanic Survival Prediction 🚢

## Overview  
This project aims to predict the survival of passengers aboard the Titanic using machine learning techniques. The prediction is based on features such as **passenger class (Pclass)**, **sex**, and other factors, using **Logistic Regression** as the primary machine learning model. 

The project utilizes data preprocessing techniques such as encoding categorical features, feature selection, and visualization using **seaborn** for data analysis.  

---

## Dataset  
The Titanic dataset used in this project contains the following columns:  
1. **PassengerId**: A unique identifier for each passenger.  
2. **Pclass**: Passenger's class (1st, 2nd, or 3rd).  
3. **Name**: Name of the passenger.  
4. **Sex**: Gender of the passenger (Male/Female).  
5. **Age**: Age of the passenger.  
6. **SibSp**: Number of siblings or spouses aboard the Titanic.  
7. **Parch**: Number of parents or children aboard the Titanic.  
8. **Ticket**: Ticket number.  
9. **Fare**: Fare paid for the ticket.  
10. **Cabin**: Cabin number.  
11. **Embarked**: Port of embarkation (C = Cherbourg; Q = Queenstown; S = Southampton).  
12. **Survived**: Whether the passenger survived (1 = Yes, 0 = No) - This is the target variable.  

---

## Objective  
The goal is to predict whether a passenger survived or not based on features such as **Pclass**, **Sex**, and **Age**, using **Logistic Regression**. The model will be trained and evaluated on a split dataset and tested with new input data.  

---

## Workflow  

### 1. **Data Preprocessing**  
- **Data Cleaning**: Only numerical features are considered for correlation analysis.  
- **Encoding Categorical Features**: The **'Sex'** feature is encoded using **LabelEncoder** for model compatibility.  
- **Feature Selection**: Relevant features are selected for training (Pclass and Sex).  

### 2. **Exploratory Data Analysis (EDA)**  
- Visualizing correlations between numerical features using **heatmap**.  
- Analyzing survival distribution using **countplot** based on passenger class and sex.  

### 3. **Modeling**  
- Train a **Logistic Regression** model to predict the target variable `Survived` using the selected features.  
- Split the dataset into training and testing sets using **train_test_split**.  

### 4. **Evaluation**  
- Model performance is evaluated on the testing set to predict whether a passenger survived based on the trained features.  
- Sample predictions for a new passenger are made using the trained model.  

---

## Setup  

### Prerequisites  
Ensure you have Python ≥3.8 installed along with the following libraries:  
```bash  
pip install numpy pandas scikit-learn seaborn matplotlib  
```  

### Steps to Run  
1. Clone the repository:  
   ```bash  
   git clone https://github.com/your-username/Titanic_Survival_Prediction.git  
   cd Titanic_Survival_Prediction  
   ```  
2. Place your dataset in the project directory as `titanic.csv`.  
3. Run the script in your Python environment (e.g., Jupyter Notebook, VS Code).  

---

