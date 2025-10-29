# Electric Vehicle Type Predictor
Electric Vehicle Type Predictor is a machine learning model that classifies electric vehicles as either Battery Electric Vehicles (BEVs) or Plug-in Hybrid Electric Vehicles (PHEVs) using the Electric Vehicle Population dataset from Kaggle. It analyzes key features to improve EV categorization accuracy.

## 🧩 Problem Statement

With the rapid adoption of electric mobility, accurately classifying electric vehicles is essential for understanding market trends, policy-making, and infrastructure planning. However, due to the increasing diversity of electric vehicles — including Battery Electric Vehicles (BEVs) and Plug-in Hybrid Electric Vehicles (PHEVs) — manual categorization based on specifications and registration data becomes challenging and inefficient.

This project aims to develop a machine learning model that automatically classifies electric vehicles as BEVs or PHEVs using key attributes such as electric range, model, make, price, and location. By leveraging the Electric Vehicle Population dataset, the model seeks to enhance the accuracy and reliability of EV classification, supporting data-driven insights into the electric vehicle ecosystem.

## Dataset
The dataset provides comprehensive information about electric and plug-in hybrid vehicles, including technical specifications and registration details. It captures multiple features such as vehicle make, model, electric range, and location, enabling classification between Battery Electric Vehicles (BEV) and Plug-in Hybrid Electric Vehicles (PHEV).

## Key Features

•	VIN (1–10): Partial Vehicle Identification Number

•	County / City / State / Postal Code: Registration location details (State = ‘WA’)

•	Model Year: Year of vehicle manufacture

•	Make / Model: Manufacturer and model name (e.g., Tesla, Nissan, Chevrolet)

•	Electric Vehicle Type: BEV or PHEV (Target Column)

•	CAFV Eligibility: Eligibility for clean fuel incentives

•	Electric Range: Distance (in miles) the vehicle can travel on electric power alone

•	Base MSRP: Manufacturer’s Suggested Retail Price

•	Legislative District: District where the vehicle is registered

•	DOL Vehicle ID: Unique ID assigned by the Department of Licensing

•	Vehicle Location: Geographic coordinates (latitude, longitude)

•	Electric Utility: Local electricity provider

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

1. Install Python
Make sure you have Python 3.x installed on your system.
You can verify using:

python --version


2. Clone the Repository
Clone this repository to your local machine using:

git clone https://github.com/srinidhikuchana/Week1.git


3. Navigate to the Project Directory

cd Week1


4. Install the Required Libraries
5. Install all dependencies using pip:

pip install pandas numpy scikit-learn matplotlib seaborn


6. Open the Jupyter Notebook
Launch Jupyter Lab or Notebook
7. Load the Dataset
Make sure the dataset (Electric_Vehicle_Population_Data.csv) is placed in the same directory as your notebook.
(If not, update the dataset path in the code.)

8. Run All Cells
Open the notebook file EV_type_predictor.ipynb and run all cells sequentially (Kernel → Restart & Run All).

9. View Results

10. (Optional) Run on Google Colab

•	Upload the .ipynb file and dataset to Google Colab.
•	Install required libraries with:
!pip install pandas numpy scikit-learn matplotlib seaborn
•	Run all cells to view results online.
