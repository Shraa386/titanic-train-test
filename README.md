# 🚢 Titanic Survival Prediction (Train-Test Split)

## 📌 Project Overview

This project is based on the famous Titanic dataset. The goal is to predict whether a passenger survived or not using machine learning techniques.

We use a **train-test split** method to train the model on one part of the data and test it on another to evaluate performance.

---

## 📂 Dataset

The dataset contains information about passengers such as:

* Age
* Gender
* Passenger Class (Pclass)
* Fare
* Number of siblings/spouses (SibSp)
* Number of parents/children (Parch)
* Survival (Target variable)

---

## ⚙️ Technologies Used

* Python 🐍
* Pandas
* NumPy
* Sklearn

---

## 🔀 Train-Test Split

We split the dataset into:

* **Training Data (80%)** → Used to train the model
* **Testing Data (20%)** → Used to evaluate the model

Example code:

```python
from sklearn.model_selection import train_test_split

X = data.drop("Survived", axis=1)
y = data["Survived"]

X_train, X_test, y_train, y_test = train_test_split(X, y, test_size=0.2, random_state=42)
```

---

## 🤖 Model Used

We used **Logistic Regression** for prediction.

```python
from sklearn.linear_model import LogisticRegression

model = LogisticRegression()
model.fit(X_train, y_train)
```

---

## 📊 Evaluation

The model is evaluated using accuracy score.

```python
from sklearn.metrics import accuracy_score

y_pred = model.predict(X_test)
accuracy = accuracy_score(y_test, y_pred)
print("Accuracy:", accuracy)```
---

## 📌 Conclusion

This project demonstrates how to:

* Preprocess data
* Split dataset into train and test sets
* Train a machine learning model
* Evaluate model performance

---

## 📎 Author

Shravani Waikar
