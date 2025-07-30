
# 🧠 Student Exam Performance Predictor

This project is a complete **machine learning web application** built using Python and Flask. It predicts a student's **math exam score** based on various input features like gender, parental education level, reading and writing scores, etc. It demonstrates a full ML pipeline—from data ingestion and preprocessing to model training and deployment.

---

## 🚀 Project Structure

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
📊 Problem Statement
The goal is to build a regression model that predicts a student's math score based on:

Gender

Race/Ethnicity

Parental level of education

Lunch type

Test preparation course

Reading score

Writing score

⚙️ Tech Stack Used
Languages & Libraries: Python, Pandas, NumPy, Scikit-learn, CatBoost, XGBoost

Modeling: Regression models (Random Forest, Gradient Boosting, CatBoost, etc.)

Web Framework: Flask

Frontend: HTML, Bootstrap

Deployment: Localhost (can be extended to platforms like Heroku, AWS, etc.)

📈 Model Performance
Best Model: CatBoost Regressor

R² Score (Test Set): 0.8516

Evaluation: Compared multiple models and selected based on cross-validation R² score.

🧪 How to Run the Project Locally
1. Clone the Repository
bash
Copy
Edit
git clone https://github.com/viplavs2004/ML_PROJECT.git
cd student-exam-performance-predictor
2. Create a Virtual Environment
bash
Copy
Edit
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
3. Install Dependencies
bash
Copy
Edit
pip install -r requirements.txt
4. Run the Flask App
bash
Copy
Edit
python app.py
Then open your browser and visit: http://localhost:5000

🧠 Prediction Flow
User visits homepage with model details

Clicks "Go to Predictor"

Fills in form on /predictdata

Model predicts math score based on form inputs

Result is displayed in real time



✍️ Author
Viplav Singh
B.Tech ECE, IIIT Manipur
Email: viplavs2004@gmail.com
LinkedIn: www.linkedin.com/in/viplavs2004