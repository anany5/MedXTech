# MedXTech: Developing a Patient Condition Prediction System

## Team Members:
1. Ansh Agrawal (2100290100031)
2. Anany Raj Singh (2100290100027)
3. Adish Sharma (2100290100011)

## Steps for Execution:
### Step 0: Data Collection & Preparation
- Health metrics were collected, including:
  - Heart Rate  
  - Respiratory Rate  
  - Body Temperature  
  - Oxygen Saturation  
  - Age  
  - Gender  
  - Derived metrics: HRV, Pulse Pressure, BMI, MAP  
- Data preprocessing involved cleaning, normalization, and feature engineering using Python (Pandas, NumPy).
- Data was sourced from open datasets.

### Step 1: Train the Machine Learning Model
- Open the provided Colab notebook [`Health_Prediction_Model_Training.ipynb`](https://colab.research.google.com/drive/1fhlwe3DACcz1pcVkSVcSFyg0GUO1utLj?usp=sharing)
- Run all cells to train the ML model.
- Download the generated files: `scaler.joblib` and `model.joblib`.
- Place these files inside the backend folder `backend/models/`.

### Step 2: Setup and Run the Flask Backend
- In `backend/`, create a `.env` file containing your MongoDB credentials:
  ```bash
  MONGO_USER=your_mongodb_username
  MONGO_PASS=your_mongodb_password
- Install dependencies:
  ```bash
  pip install -r requirements.txt
- Run it locally or deploy to Render using the Dockerfile provided. Set      MONGO_USER and MONGO_PASS as environment variables in Render.

### Step 3: Run the Frontend
- Navigate to the frontend/ directory.

- No build step is needed; it is a static website.

- You can test it locally by opening index.html in a browser.

- Or deploy it to Render using the provided Dockerfile or a static site hosting method.

### Step 4: Use the Application
- Visit the deployed frontend site.

- Navigate to Check Health.

- Fill in the form with health parameters like: Heart Rate, Respiratory Rate, Body Temperature, Oxygen Saturation, etc.

- Submit the form to receive a prediction: Sick or Not Sick.


## Links
### Website link
- [Frontend](https://ui-updated.onrender.com/)
- [Backend](https://flaskbackendgithub-updated-correct.onrender.com) only available for POST requests
### Docker Image link
- Here is the Docker container for the Flask backend: [Docker flaskbackend](https://hub.docker.com/r/someone101/flaskbackend)
- Here is the Docker container for the Flask Frontend: [Docker uifrontend](https://hub.docker.com/r/someone101/uifrontend)


## Checklist:
1. Final Project Report
2. Certificate VII Semester (Dated: December 2024).
3. Certificate VIII Semester (Dated: May 2025).
4. Synopsis
5. Final Presentation
6. Source Code
7. Database dump (.sql file)
8. If a web project, then a Docker file for deployment
9. README (This file)