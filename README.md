# Student Career & Job Predictor (SVM)

This project is a Streamlit-based web application that uses a Support Vector Machine (SVM) classifier to predict whether a student has a part-time job based on their academic performance and study habits.

## Features

* **Interactive Data Exploration**: View a preview of the first 10 rows of the student dataset directly in the app.
* **Dynamic Model Tuning**:
* Adjust the test data size using a slider (10% to 50%).
* Select different SVM kernels (linear, poly, rbf, or sigmoid) to see how they impact prediction accuracy.


* **Real-time Performance Metrics**: Displays the model's accuracy score based on the selected parameters.
* **Single Student Prediction**: A manual tool where you can input specific student metrics to get an instant job status prediction.

## Input Parameters

The model utilizes the following nine features for its predictions:

* Absence Days
* Weekly Self-Study Hours
* Math Score
* History Score
* Physics Score
* Chemistry Score
* Biology Score
* English Score
* Geography Score

## Technologies Used

* **Frontend**: Streamlit
* **Data Handling**: Pandas
* **Machine Learning**: Scikit-learn (SVM, StandardScaler, LabelEncoder)

## Setup and Installation

1. **Prerequisites**: Ensure you have Python installed along with the required libraries:
```bash
pip install streamlit pandas scikit-learn

```


2. **Dataset**: The application expects a CSV file named `student-scores.csv` located at `c:\Users\Aanjney\Downloads\`. *(Note: You may need to update the file path in `app.py` to match your local environment)*.
3. **Run the App**:
```bash
streamlit run app.py

```



## Usage

1. Open the application in your browser.
2. Use the **Sidebar** to configure the test data split and the SVM kernel.
3. Review the **Model Performance** metric to see the accuracy of your configuration.
4. Scroll to the **"Check Single Student Prediction"** section, enter the student's data, and click **"Predict Job Status"** to see the result.
