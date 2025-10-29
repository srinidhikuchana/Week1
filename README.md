# Electric Vehicle Type Predictor
Electric Vehicle Type Predictor is a machine learning model that classifies electric vehicles as either Battery Electric Vehicles (BEVs) or Plug-in Hybrid Electric Vehicles (PHEVs) using the Electric Vehicle Population dataset from Kaggle. It analyzes key features to improve EV categorization accuracy.
## Dataset
The dataset provides comprehensive information about electric and plug-in hybrid vehicles, including technical specifications and registration details. It captures multiple features such as vehicle make, model, electric range, and location, enabling classification between Battery Electric Vehicles (BEV) and Plug-in Hybrid Electric Vehicles (PHEV).

Key Features

VIN (1–10): Partial Vehicle Identification Number

County / City / State / Postal Code: Registration location details (State = ‘WA’)

Model Year: Year of vehicle manufacture

Make / Model: Manufacturer and model name (e.g., Tesla, Nissan, Chevrolet)

Electric Vehicle Type: BEV or PHEV (Target Column)

CAFV Eligibility: Eligibility for clean fuel incentives

Electric Range: Distance (in miles) the vehicle can travel on electric power alone

Base MSRP: Manufacturer’s Suggested Retail Price

Legislative District: District where the vehicle is registered

DOL Vehicle ID: Unique ID assigned by the Department of Licensing

Vehicle Location: Geographic coordinates (latitude, longitude)

Electric Utility: Local electricity provider

2020 Census Tract: Census data for demographic analysis

## 🎯 Target Variable

Electric Vehicle Type — Predict whether a vehicle is a Battery Electric Vehicle (BEV) or a Plug-in Hybrid Electric Vehicle (PHEV).

📂 Dataset Source: Download the dataset here [https://www.kaggle.com/datasets/gunapro/electric-vehicle-population-data]

## ⚙️ Project Workflow
1. Data Preprocessing

Feature Selection: Chose relevant features and removed redundant columns.

Handling Missing Values: Imputed missing numerical data using the median and categorical data using the mode.

Encoding: Applied Label Encoding for categorical variables and the target column.

Scaling: Standardized numerical features to improve SVM model performance.

2. Model Development

Algorithm: Used a Linear Support Vector Machine (SVM) classifier to predict vehicle type.

Train-Test Split: Divided the data into 80% training and 20% testing sets.

Evaluation Metrics: Measured performance using accuracy, confusion matrix, and classification report.

3. Visualizations

Confusion Matrix Heatmap: Displays correct vs. incorrect predictions.

Feature Importance Plot: Highlights key features influencing classification outcomes (based on SVM coefficients).

## 🧩 Requirements

Python 3.x

pandas

numpy

scikit-learn

matplotlib

seaborn

google.colab (optional — for running on Google Colab)

Install all dependencies using:

pip install pandas numpy scikit-learn matplotlib seaborn

## 🚀 How to Run the Project

1. Clone the repository
2. Navigate to the project directory
cd electric-vehicle-type-prediction
3. Install the dependencies :
pip install -r requirements.txt


Open and run the Jupyter Notebook:

jupyter-lab


Then open the notebook file and execute all cells.
