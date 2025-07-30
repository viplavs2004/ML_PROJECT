# Student Exam Performance Prediction

This project is a complete machine learning web application that predicts a student's **math exam score** based on various academic and demographic features. It demonstrates an end-to-end ML workflow: from data ingestion and transformation to model training and deployment using Flask.

## Project Overview

This regression model was trained using various algorithms and evaluated to find the best-performing one. The deployed web app allows users to input student details and receive a predicted math score.

### Features
- Data ingestion and cleaning pipeline
- Automated data transformation (encoding, scaling)
- Multiple regression models trained and evaluated
- Model selection based on performance (R² score)
- Flask-based frontend for user interaction
- HTML form to collect prediction input
- Displays predicted score in real-time

## Problem Statement

Given the following input features:

- Gender
- Race/Ethnicity
- Parental level of education
- Lunch type
- Test preparation course
- Reading score
- Writing score

The goal is to predict a student's **math score** using a regression model.


##  Project Structure

```bash
StudentExamPerformance/
├── app.py                        # Flask app main file
├── templates/
│   ├── index.html                # Project intro/homepage
│   └── home.html                 # Prediction input form
├── src/
│   ├── components/               # Data ingestion, transformation, model training
│   ├── pipeline/                 # Prediction pipeline
│   ├── utils.py                  # Utility functions (model saving, evaluation)
│   ├── logger.py                 # Logging
│   └── exception.py              # Custom error handling
├── artifacts/                   # Stores model.pkl, transformed data
├── notebook/
│   └── data/stud.csv            # Raw dataset
├── requirements.txt             # Python dependencies
└── README.md                    # This file


## Model Performance
Best model selected: CatBoost Regressor

R² Score on test data: 0.8516

How to Run the Project
Step 1: Clone the Repository
First, clone the project from GitHub and navigate to the project directory:

Open your terminal or command prompt and run:


git clone https://github.com/viplavs2004/ML_PROJECT.git
cd ML_PROJECT
Step 2: Set Up the Environment
You can set up your Python environment using either venv or conda.

Option A: Using venv (Standard Python)
Create a virtual environment:


python -m venv venv
Activate the environment:

On Windows: venv\Scripts\activate

On macOS/Linux: source venv/bin/activate

Option B: Using Conda
Create a new conda environment with Python 3.11:


conda create --name ml_project_env python=3.11
Activate the conda environment:


conda activate ml_project_env
Step 3: Install Required Packages
Once your environment is activated, install all the necessary dependencies using:


pip install -r requirements.txt
Step 4: Run the Flask Application
Start the Flask web application by running:


python app.py
The application will be hosted locally at: http://127.0.0.1:5000/

Open this URL in your web browser to interact with the application.

App Pages
Home Page (/)
This is the landing page of the web application. It provides an overview of the project, including:

The objective of the model

The performance metric (R² Score)

A brief explanation of how the model works

A call-to-action button to navigate to the prediction form

You can include a screenshot here showing how the home page looks.

Prediction Page (/predictdata)
Once the user clicks on the prediction button from the home page, they are taken to this form-based page.

This page contains a form where the user can input:

Gender

Ethnicity

Parental level of education

Lunch type

Test preparation course

Reading score

Writing score

After submitting the form, the model processes the input and displays the predicted math score immediately.

You can include a screenshot here showing the prediction form and how the result is displayed.

Author
Viplav Singh
B.Tech ECE, IIIT Manipur
Email: viplavs2004@gmail.com
LinkedIn: www.linkedin.com/in/viplavs2004



Displays the predicted Math Score upon submission.

Author
Viplav Singh
B.Tech ECE, IIIT Manipur
Email: viplavs2004@gmail.com
LinkedIn: www.linkedin.com/in/viplavs2004
