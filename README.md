# Iris Species Classification using Logistic Regression

![Python](https://img.shields.io/badge/Python-3.10%2B-blue.svg)
![Libraries](https://img.shields.io/badge/Libraries-Pandas%20%7C%20Scikit--learn%20%7C%20Seaborn-orange.svg)
![License](https://img.shields.io/badge/License-MIT-green.svg)



### ## 📝 Overview

This project demonstrates a complete machine learning workflow for building a binary classification model. The goal is to predict whether an iris flower is of the **Iris virginica** species based on its sepal and petal measurements.

The project covers all key stages from data exploration and visualization to model training and performance evaluation.

---

### ## 🌸 Dataset

The project uses the classic **Iris dataset**, a well-known dataset in pattern recognition and machine learning.

* **Source:** Scikit-learn's built-in datasets (originally from the UCI Machine Learning Repository).
* **Features:**
    1.  Sepal Length (cm)
    2.  Sepal Width (cm)
    3.  Petal Length (cm)
    4.  Petal Width (cm)
* **Target:** Three species of Iris flowers (Setosa, Versicolor, Virginica).
* **Samples:** 150 total (50 for each species).

---

### ## ⚙️ Project Workflow

The analysis is structured in a Jupyter Notebook (`iris_classification.ipynb`) and follows these steps:

1.  **Exploratory Data Analysis (EDA):**
    * Loaded the dataset into a Pandas DataFrame.
    * Checked for missing values, data types, and statistical properties.
    * Analyzed the class distribution to confirm the dataset is balanced.

2.  **Data Visualization:**
    * Created a **pair plot** to visualize relationships between all features, colored by species.
    * Generated a **correlation heatmap** to identify multicollinearity between features.
    * Used **box plots** to compare the feature distributions for each species.

3.  **Data Preprocessing:**
    * Converted the multi-class problem into a binary one (Virginica vs. Not Virginica).
    * Split the data into 80% for training and 20% for testing.
    * Scaled the features using `StandardScaler` to normalize their range.

4.  **Model Training & Evaluation:**
    * Trained a **Logistic Regression** model on the preprocessed training data.
    * Evaluated the model's performance on the unseen test set using accuracy, a classification report, and a confusion matrix.

---

### ## 🛠️ Technologies Used

* **Python 3.10+**
* **Pandas:** For data manipulation and analysis.
* **Scikit-learn:** For data preprocessing, model training, and evaluation.
* **Matplotlib & Seaborn:** For data visualization.
* **Jupyter Notebook / Google Colab:** As the development environment.

---

### ## 🚀 How to Run

To run this project on your local machine or in Google Colab:

1.  **Clone the repository:**
    ```bash
    git clone [https://github.com/your-username/your-repo-name.git](https://github.com/your-username/your-repo-name.git)
    ```
2.  **Navigate to the project directory:**
    ```bash
    cd your-repo-name
    ```
3.  **Install dependencies (if running locally):**
    ```bash
    pip install pandas scikit-learn matplotlib seaborn jupyterlab
    ```
4.  **Launch and run the notebook:**
    * **Locally:** Open the `iris_classification.ipynb` file in Jupyter Lab/Notebook.
    * **Google Colab:** Upload the `iris_classification.ipynb` file and run the cells.

---

### ## 📊 Model Performance

The trained Logistic Regression model demonstrated excellent performance on the held-out test set.

* **Accuracy:** **100%**

* **Confusion Matrix:** The matrix confirms that there were zero misclassifications.
    * **True Negatives (Not Virginica):** 20
    * **True Positives (Virginica):** 10
    * **False Positives / Negatives:** 0

    

* **Classification Report:**
    | Class         | Precision | Recall | F1-Score |
    | :------------ | :-------- | :----- | :------- |
    | Not Virginica | 1.00      | 1.00   | 1.00     |
    | Virginica     | 1.00      | 1.00   | 1.00     |

---

### ## 📄 License

This project is licensed under the MIT License. See the `LICENSE` file for details.
