# 🌦️ KNN Weather Classifier

An interactive machine learning web application built with **Streamlit**. This project demonstrates the **K-Nearest Neighbors (KNN)** algorithm by classifying weather conditions based on real-time user inputs for temperature and humidity.

---

## 🚀 Overview
The **KNN Weather Classifier** uses a supervised learning approach to predict whether a day is **Sunny** or **Rainy**. It maps historical data points onto a 2D plane and uses proximity (distance) to determine the classification of a new data point.

## 🛠️ Tech Stack
* **Python**: Core logic and data processing.
* **Streamlit**: Web interface and interactivity.
* **Scikit-Learn**: Machine learning model (`KNeighborsClassifier`).
* **Matplotlib & NumPy**: Data visualization and array handling.

## 📊 Features
* **Interactive Sidebar**: Adjust temperature and humidity sliders to see immediate model updates.
* **Visual Classification**: A live-updating scatter plot that marks the "New Day" with a star icon.
* **ML in Action**: Uses $k=3$ neighbors to demonstrate how proximity-based algorithms work.

## 📝 How It Works
The model predicts the weather based on the following logic:
1.  **Input**: The user provides a Temperature and Humidity value.
2.  **Distance**: The algorithm calculates the Euclidean distance between the user input and the known dataset:
    $$d = \sqrt{(x_2 - x_1)^2 + (y_2 - y_1)^2}$$
3.  **Voting**: The model looks at the 3 closest neighbors. The majority class (Sunny or Rainy) among those neighbors becomes the final prediction.

## ⚙️ Installation & Usage

1. **Clone the repository or save the script** as `app.py`.
2. **Install the required packages**:
   ```bash
   pip install streamlit numpy matplotlib scikit-learn

Run the Streamlit app:

Bash
`streamlit run app.py`
## 📂 Project Structure
app.py: Contains the model initialization, the Streamlit UI, and the Matplotlib plotting logic.

Training Data: Hardcoded values for quick demonstration (Temperature vs. Humidity).   
