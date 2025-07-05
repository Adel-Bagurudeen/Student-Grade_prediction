
# Student Grade Prediction using Logistic Regression
This project uses **Logistic Regression** to classify whether a student is likely to **pass (1)** or **fail (0)**, based on two measurable parameters:

- Study Hours
- Attendance Rate

The model is built using **Python** and run in **Google Colab**.

---

## Dataset Overview

This project uses a **synthetic dataset**, created manually within the code. The dataset includes the following attributes:

| Feature      | Description                                |
|--------------|--------------------------------------------|
| `StudyHours` | Number of hours the student studies daily  |
| `Attendance` | Student's attendance percentage (0-100%)   |
| `Result`     | Target variable: 0 = Fail, 1 = Pass        |

**Sample Data:**

| StudyHours | Attendance | Result |
|------------|------------|--------|
| 2          | 65         | 0      |
| 5          | 80         | 1      |
| 7          | 95         | 1      |


---

## Tools and Libraries Used

The implementation was done in **Google Colab** using the following Python libraries:

| Library        | Usage                                      |
|----------------|--------------------------------------------|
| `pandas`       | Data structure and manipulation             |
| `matplotlib`   | Data visualization                          |
| `scikit-learn` | Machine learning modeling and evaluation    |

### Key Modules from `scikit-learn`:
- `train_test_split`: Splits the dataset into training and test sets
- `LogisticRegression`: Builds and trains the classification model
- `accuracy_score`, `confusion_matrix`, `classification_report`: Evaluates model performance

---

## Project Workflow

### 1. Data Preparation
- The dataset is initialized as a Python dictionary and converted into a DataFrame.
- Input features: `StudyHours` and `Attendance`
- Output label: `Result`

### 2. Data Visualization
- A scatter plot is generated to explore the relationship between inputs and output.
- Data points are color-coded by `Result` using a colormap (`bwr`).

### 3. Model Training
- The dataset is split into 80% training and 20% testing data.
- A Logistic Regression model is trained using the training portion.

### 4. Predictions
- The model is evaluated on the test set.
- You can manually input new values to test real-time predictions.

### 5. Model Evaluation
- **Accuracy Score**: Measures the correctness of predictions
- **Confusion Matrix**: Compares predicted and actual outcomes
- **Classification Report**: Displays precision, recall, and F1-score

---

## Example Output
Accuracy Score       : 0.10
Prediction Example:
```plaintext
![Student Chart](https://github.com/user-attachments/assets/45cf8e8d-abb1-4bc7-8378-ab4d2b445e2a.png)

