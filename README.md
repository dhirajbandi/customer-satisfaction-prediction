# **Predicting Customer Satisfaction Before Purchase**  
🚀 **End-to-End Machine Learning Pipeline for Customer Review Prediction**  

![Python](https://img.shields.io/badge/Python-3.8%2B-blue.svg)  
![MLflow](https://img.shields.io/badge/MLflow-Enabled-brightgreen)  
![ZenML](https://img.shields.io/badge/ZenML-Pipeline-orange)  
![Streamlit](https://img.shields.io/badge/Streamlit-Dashboard-red)  

## **📌 Project Overview**  
This project builds a **machine learning pipeline** that predicts **customer satisfaction scores (review ratings) before purchase** based on historical e-commerce data.  

Using the **Brazilian E-Commerce Public Dataset (Olist)**, we train models to predict how likely a customer is to leave a **positive or negative review** based on order details, shipping, and product attributes.  

This pipeline is **fully automated**, meaning it:
- **Trains, evaluates, and updates the model automatically** when new data arrives.  
- **Deploys the model in real-time** for businesses to use predictions before order placement.  
- **Provides an interactive Streamlit dashboard** for live review score predictions.  

## **🎯 Key Features**  
✔ **End-to-end ML Pipeline** using **ZenML** for training, evaluation, and deployment.  
✔ **Model tracking & versioning** using **MLflow** to compare performance over time.  
✔ **Automated retraining & deployment** when new data is available.  
✔ **Feature engineering** for insights into customer behavior & product impact.  
✔ **Live interactive dashboard** (built with **Streamlit**) for real-time predictions.  

---

## **📊 Dataset Used**  
📂 **Brazilian E-Commerce Public Dataset (Olist)** – [Available on Kaggle](https://www.kaggle.com/datasets/olistbr/brazilian-ecommerce)  
- **100,000+ orders** from **2016–2018** across multiple marketplaces in Brazil.  
- Includes order status, payment details, shipping times, and **customer reviews**.  

### **🔹 Target Variable:**  
**Customer review score** (1 to 5 stars)  

### **🔹 Features Used:**  
✅ **Order status** (delivered, canceled, etc.)  
✅ **Product price, freight cost, total payment**  
✅ **Customer’s past order history & satisfaction scores**  
✅ **Shipping time & delays**  
✅ **Product category & attributes**  

---

## **🛠 Technologies Used**  
| Technology  | Purpose  |
|-------------|--------------------------------------------------------------|
| **Python**  | Data Processing & Machine Learning  |
| **Pandas, NumPy**  | Data Cleaning & Feature Engineering  |
| **Scikit-learn, XGBoost**  | ML Models for Review Score Prediction  |
| **ZenML**  | ML Pipeline Automation  |
| **MLflow**  | Model Tracking, Experiment Logging, & Deployment  |
| **Streamlit**  | Interactive Dashboard for Predictions  |

---

## **🚀 Project Workflow**  
### **1️⃣ Data Ingestion & Cleaning**  
- Load raw customer order data.  
- Remove missing/irrelevant columns, clean categorical data.  

### **2️⃣ Feature Engineering**  
- Extract insights like **average past review score per customer**, **order delays**, etc.  
- Standardize features for better model accuracy.  

### **3️⃣ Model Training & Evaluation**  
- Train **XGBoost, Random Forest, and Gradient Boosting models**.  
- Use **MLflow tracking** to log experiments & compare performance.  
- Evaluate using **Mean Squared Error (MSE)**.  

### **4️⃣ Model Deployment & Continuous Learning**  
- Automatically **retrain and deploy** when new data arrives.  
- Use **ZenML & MLflow** to track versions and serve predictions in real-time.  
- Deploy a **Streamlit dashboard** for businesses to test live predictions.  

---

## **📦 Installation & Setup**  
Clone the repository and install dependencies:  
```bash
git clone https://github.com/dhirajbandi/customer-satisfaction-prediction.git
cd customer-satisfaction-prediction
pip install -r requirements.txt
```

### **🔹 Set Up ZenML & MLflow**
Ensure you have **ZenML** and **MLflow** installed:  
```bash
pip install zenml["server"] mlflow
zenml up  # Launch ZenML Server & Dashboard
```

### **🔹 Run the Training Pipeline**
```bash
python run_pipeline.py
```

### **🔹 Deploy the Continuous Training Pipeline**
```bash
python run_deployment.py
```

### **🔹 Start the Streamlit Dashboard**
```bash
streamlit run streamlit_app.py
```
Once running, open your browser at **`http://localhost:8501`** to interact with the live dashboard.  

---

## **📌 Future Improvements**
✅ Incorporate **sentiment analysis** on customer reviews for better insights.  
✅ Improve prediction accuracy with **deep learning models**.  
✅ Deploy on cloud services (AWS, GCP) for **scalability**.  
✅ Add a **recommendation system** to suggest better products to at-risk customers.  

---

## **📬 Contact & Support**
📧 **Dhiraj Bandi** – [Email Me](mailto:dhirajbandiwork@gmail.com)  
🔗 **LinkedIn:** [linkedin.com/in/dhiraj-bandi](https://www.linkedin.com/in/dhiraj-bandi/)  
📂 **GitHub:** [github.com/dhirajbandi](https://github.com/dhirajbandi)  

---

## **🌟 Acknowledgements**
Special thanks to **ZenML** and **MLflow** for their open-source tools that made this project possible! 🙌  
