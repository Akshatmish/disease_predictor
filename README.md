Overview

The application leverages logistic regression models trained on synthetic and real datasets to predict diseases such as Heart Disease, Kidney Disease, Liver Disease, Diabetes, Lung Disease, Thyroid Issues, and Stroke. Key features include:

Disease Prediction: Input health metrics to get a probability score and recommended specialist.

Appointment Booking: Schedule consultations with specialists based on predictions.

User-Friendly Interface: Built with Flask and styled using Bootstrap.

Prerequisites

Before running the application, ensure you have the following installed:

Python 3.8 or higher

pip (Python package manager)

Required Python Packages

Install the dependencies using pip:

pip install flask pandas numpy scikit-learn

Installation

**Download the Dataset: **

Place the kidney_disease.csv file in the project root directory. You can download it from Kaggle.

Set Up the Project Structure: Ensure the following structure:

smart-disease-prediction/ ├── app.py ├── kidney_disease.csv ├── templates/ │ ├── index.html │ ├── input.html │ ├── result.html │ ├── error.html │ ├── appointment.html │
├── static/ (optional) ├── reviews.db (created on run) ├── README.md

Run the Application:

python app.py

The app will start on http://localhost:5000.

Usage

Home Page:

Visit http://localhost:5000 in your browser.

Select a disease from the dropdown and click "Predict" to proceed.

**Input Health Data: ** Enter the required health metrics (e.g., age, cholesterol, blood pressure) and submit.

View the prediction probability and specialist recommendations.

**Book an Appointment: **

After a prediction, use the form to book an appointment with the recommended doctor.

Submit with your name, desired date, and time.

Confirm the booking on the next page.

**Features ** Machine Learning Models: Trained on synthetic data for multiple diseases and real data for kidney disease.

Real-Time Appointment Management: Stores and retrieves appointments from a SQLite database.

Responsive Design: Styled with Bootstrap for a clean, mobile-friendly interface.
