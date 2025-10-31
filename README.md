# Health_analysis


# Body Fat Percentage Prediction using Machine Learning & Gradio

## 🚀 Project Overview  
This project uses a machine-learning model (linear regression) to **predict body-fat percentage** from measurable features such as weight, BMI, calories intake, lean-mass estimation, and calorie-balance. A web interface built with Gradio allows users to input their data (weight, height, calories intake) and get an instant prediction.  
It’s designed to demonstrate:  
- Data preprocessing & feature engineering (BMI, lean mass, calorie balance)  
- Building & evaluating a regression model with scikit‑learn  
- Deploying a user-friendly interface in Google Colab (and for later production use)  

## 📋 Table of Contents  
- [Features](#features)  
- [Dataset & Features](#dataset-features)  
- [Getting Started](#getting-started)  
  - [Prerequisites](#prerequisites)  
  - [Installation](#installation)  
  - [Usage](#usage)  
- [Model Evaluation](#model-evaluation)  
- [Deployment](#deployment)  
- [Future Improvements](#future-improvements)  
- [Project Structure](#project-structure)  
- [Technologies Used](#technologies-used)  
- [License](#license)  
- [Acknowledgements](#acknowledgements)  

## ✨ Features  
- Calculates derived features: BMI, calorie balance, lean mass  
- Trains a linear regression model on these features to predict fat percentage  
- Provides a Gradio web interface to input values and view predictions  
- Easy to extend for more advanced modelling (e.g., tree-based, deep learning) or deployment  

## 📊 Dataset & Features  
- **Target**: Body fat percentage (`Fat_Percentage`)  
- **Input Features** (used in model):  
  - `Weight (kg)`  
  - `BMI`  
  - `Calories` (daily intake in kcal)  
  - `BMI_calc` (BMI computed from weight & height)  
  - `cal_balance` (calorie intake minus estimated calories burned)  
  - `lean_mass_kg` (estimated lean body mass in kg)  
- Note: For new users (via interface), BMI, calorie balance and lean mass are computed automatically (based on weight, height, calories intake) so the user only needs to enter measurable inputs.

## 🧰 Getting Started  
### Prerequisites  
- Python 3.10+  
- Basic libraries: pandas, numpy, scikit-learn, gradio  
### Installation  
```bash
# Clone the repo
git clone https://github.com/yourusername/body-fat-prediction.git
cd body-fat-prediction

# (Optional) create and activate virtual env
python -m venv venv
source venv/bin/activate  # (or venv\Scripts\activate on Windows)

# Install dependencies
pip install -r requirements.txt
