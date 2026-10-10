
# 🎓 Student Exam Performance Prediction

An end-to-end Machine Learning project that predicts student exam performance using Python, Scikit-learn, and Flask. The project includes data preprocessing, model training, a reusable prediction pipeline, and a web application deployed on Render.

## 🚀 Live Demo

**Live Application:** https://ml-project-7t21.onrender.com

**GitHub Repository:** https://github.com/rahuldungdung809-alt/ML_project_

## 📌 Overview

Student Exam Performance Prediction demonstrates how machine learning can be integrated into a web application. The project follows a modular architecture that separates model training, prediction, utility functions, and application logic.

Users can access the deployed application and submit input through the web interface to obtain predictions.

## ✨ Features

- Data preprocessing and feature transformation
- Machine learning model training and evaluation
- Reusable prediction pipeline
- Flask-based web application
- Model and preprocessing artifact management
- Custom logging and exception handling
- Modular Python project structure
- Docker support for containerization
- Deployment on Render

## 🛠️ Tech Stack

| Technology | Purpose |
|---|---|
| Python | Core programming language |
| Pandas | Data manipulation and analysis |
| NumPy | Numerical computations |
| Scikit-learn | Machine learning and preprocessing |
| CatBoost | Gradient boosting, if enabled |
| Flask | Web application |
| Dill / Pickle | Model serialization, depending on implementation |
| Docker | Containerization |
| Git & GitHub | Version control |
| Render | Application deployment |

## 📂 Project Structure

```text
ML_project_/
├── artifacts/
├── catboost_info/
├── logs/
├── notebook/
├── src/
│   ├── components/
│   ├── pipeline/
│   │   ├── predict_pipeline.py
│   │   └── train_pipeline.py
│   ├── __init__.py
│   ├── exception.py
│   ├── logger.py
│   └── utils.py
├── static/
├── templates/
├── app.py
├── Dockerfile
├── requirements.txt
├── setup.py
├── .dockerignore
├── .gitignore
└── README.md
```

## ⚙️ Installation and Setup

### 1. Clone the repository

```bash
git clone https://github.com/rahuldungdung809-alt/ML_project_.git
cd ML_project_
```

### 2. Create a virtual environment

**Windows**

```bash
python -m venv venv
venv\Scripts\activate
```

**Linux / macOS**

```bash
python3 -m venv venv
source venv/bin/activate
```

### 3. Install dependencies

```bash
python -m pip install --upgrade pip
pip install -r requirements.txt
```

### 4. Run the application

```bash
python app.py
```

Open the local application in your browser:

http://127.0.0.1:5000

Ensure that the required model and preprocessing artifacts are available before generating predictions.

## 🐳 Run with Docker

Build the Docker image:

```bash
docker build -t student-exam-performance .
```

Run the container:

```bash
docker run --rm -p 5000:5000 student-exam-performance
```

Open the application:

http://localhost:5000

Ensure that the Dockerfile uses the correct application entry point and that Flask binds to `0.0.0.0` inside the container.

## 🧠 Machine Learning Workflow

1. Load and explore the dataset.
2. Clean and preprocess the data.
3. Transform numerical and categorical features.
4. Train the configured machine learning models.
5. Evaluate model performance using appropriate metrics.
6. Save the trained model and preprocessing objects.
7. Load the saved artifacts through the prediction pipeline.
8. Generate predictions through the Flask web interface.

## 📊 Model Evaluation

Model performance should be reported using actual training results.

For regression tasks, common evaluation metrics include:

- **R² Score:** Measures how well the model explains variation in the target.
- **Mean Absolute Error (MAE):** Measures the average absolute prediction error.
- **Root Mean Squared Error (RMSE):** Penalizes larger prediction errors more heavily.

Add the final model name and measured scores after verifying your training results.

## ☁️ Deployment

The application is deployed on Render.

**Live URL:** https://ml-project-7t21.onrender.com

Deployment checklist:

- Install dependencies from `requirements.txt`.
- Configure the correct application start command.
- Ensure the application uses the hosting platform's expected port.
- Make required model artifacts available at runtime.
- Configure any required environment variables.
- Test the deployed application after deployment.

## 🔮 Future Improvements

- Compare multiple machine learning models.
- Add model evaluation visualizations.
- Improve input validation and error handling.
- Add automated tests for the prediction pipeline.
- Add screenshots of the application interface.
- Implement continuous integration and deployment.

## 👨‍💻 Author

**Rahul Dung Dung**

Computer Engineering Student  
Interested in Machine Learning, Data Science, and Software Development.

**GitHub:** https://github.com/rahuldungdung809-alt

## 📄 License

This project is created for educational and learning purposes.