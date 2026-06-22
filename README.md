# ml-model-deployment-week4-task2
Deployment of a Machine Learning model using Flask and Docker. The project includes model training, API creation, and containerization for deployment.
# ML Model Deployment - Week 4 Task 2

## 📌 Project Overview
This project demonstrates how to deploy a trained Machine Learning model using Flask and Docker. The model is trained on a dataset and exposed as an API endpoint for predictions.

---

##  Project Structure
- `app.py` → Flask API for serving the ML model  
- `model.pkl` → Trained machine learning model  
- `requirements.txt` → Required Python dependencies  
- `Dockerfile` → Docker configuration for containerization  

---

##  How It Works
1. The trained ML model is saved using `pickle` as `model.pkl`.
2. Flask application loads the model.
3. API receives input features via POST request.
4. Model returns prediction as output.

---

##  API Endpoints

### Home Route
**GET /**
- Response:
- ML Model API Running


---

### Prediction Route
**POST /predict**

#### Input Format:
```json
{
  "features": [0, 1, 0, 1, 0, 1, 0, 1]
}
Output Format:
{
  "prediction": 1
}
Run Docker Container
docker run -p 5000:5000 ml-model-api
Technologies Used
Python
Flask
Scikit-learn
Pandas
NumPy
Docker
