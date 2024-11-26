# MediInsight

## Overview
This is a web-based medical diagnosis prediction application built using Flask and machine learning. The application allows users to input their symptoms and receive a potential disease diagnosis along with detailed information about the predicted condition.

## Features
- Symptom-based disease prediction using machine learning
- Comprehensive disease information including:
  - Disease description
  - Precautions
  - Recommended medications
  - Diet recommendations
  - Workout suggestions
- Spelling correction for symptom inputs
- User-friendly web interface
- Multiple web pages (Home, About, Contact, Developer, Blog)

## Technologies Used
- Python
- Flask
- Scikit-learn
- Pandas
- NumPy
- TextBlob (for spelling correction)
- HTML/CSS (Frontend)

## Prerequisites
- Python 3.7+
- pip (Python package manager)

## Installation

### 1. Clone the Repository
```bash
git clone https://github.com/yourusername/medical-diagnosis-app.git
cd medical-diagnosis-app
```

### 2. Create Virtual Environment (Optional but Recommended)
```bash
python -m venv venv
source venv/bin/activate  # On Windows, use `venv\Scripts\activate`
```

### 3. Install Dependencies
```bash
pip install -r requirements.txt
```

### 4. Prepare Datasets and Model
- Ensure the following files are in their respective directories:
  - `dataset/symtoms_df.csv`
  - `dataset/precautions_df.csv`
  - `dataset/workout_df.csv`
  - `dataset/description.csv`
  - `dataset/medications.csv`
  - `dataset/diets.csv`
  - `model/svc.pkl`

## Running the Application
```bash
python app.py
```
Navigate to `http://localhost:5000` in your web browser.

## How It Works
1. User enters symptoms separated by commas
2. Application processes and standardizes symptoms
3. Machine learning model predicts potential disease
4. Detailed disease information is displayed, including:
   - Description
   - Precautions
   - Medications
   - Diet recommendations
   - Workout suggestions

## Supported Symptoms
The application supports a wide range of symptoms with spelling correction and synonym matching. Symptoms can be entered in various formats and the application will attempt to match them to its internal dictionary.

## Pages
- **Home**: Symptom input and diagnosis
- **About**: Information about the project
- **Contact**: Contact information
- **Developer**: Details about the development team
- **Blog**: Related medical information

## Limitations
- This is a predictive tool and should not replace professional medical advice
- Accuracy depends on the training data and model
- Limited to the diseases in the training dataset





