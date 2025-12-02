# 🌾 Crop Recommendation System

A machine learning–powered system that recommends the most suitable crop based on soil nutrients and environmental conditions. Built with **Scikit-Learn** and deployed using **Flask**, this project provides a simple web interface and API for real-time crop prediction.

---

## 🚀 Features
- RandomForest-based ML model for accurate crop recommendation  
- Complete ML pipeline: preprocessing → training → evaluation  
- Flask API for real-time predictions  
- User-friendly web interface (HTML/CSS/JS)  
- Jupyter Notebook for data exploration and experimentation  

---

## 📁 Project Structure
- app.py
- train_model.py
- Crop_Recommendation_System.ipynb
- Crop_recommendation.csv
- static/
- templates/

yaml
Copy code

---

## ⚙️ Installation
```bash
pip install flask pandas numpy scikit-learn joblib
🧪 Train the Model
bash
Copy code
python train_model.py
This generates best_model.pkl used for prediction.

🌐 Run the Web App
bash
Copy code
python app.py
Then open in your browser:
http://127.0.0.1:5000

🔗 API Endpoint
POST /predict

Example JSON request:

json
Copy code
{
  "N": 50,
  "P": 30,
  "K": 40,
  "temperature": 25,
  "humidity": 80,
  "ph": 6.5,
  "rainfall": 200
}
📌 Notes
Ensure dataset and model paths are correctly set in train_model.py and app.py

Add a requirements.txt and .gitignore for easier setup and cleaner repository

You may customize the UI inside templates/index.html and static/
