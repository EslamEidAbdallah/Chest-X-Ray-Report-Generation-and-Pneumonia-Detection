# Automated Chest X-Ray Report Generation and Pneumonia Detection System

This project is an AI-powered medical imaging system that detects pneumonia from chest X-ray images and automatically generates:

- Medical radiology reports
- Patient advice
- Arabic translation
- Downloadable PDF reports

The system uses Transfer Learning models such as DenseNet121 and MobileNetV2 for pneumonia detection and integrates the Gemini AI model for report generation and patient guidance.

---

# Project Features

- Pneumonia Detection using Deep Learning
- Medical Report Generation using Gemini AI
- Patient Advice Generation
- Arabic Translation of Reports and Advice
- PDF Export for Reports
- Streamlit Web Application
- Kaggle Notebook for Training and Evaluation

---

# Project Title

## Automated Chest X-Ray Report Generation and Pneumonia Detection System

---

# Technologies Used

- Python
- TensorFlow / Keras
- Streamlit
- Gemini AI API
- OpenCV
- PIL
- ReportLab / FPDF
- Transfer Learning

---

# Models Used

| Model | Accuracy | Precision | Recall | AUC |
|------|------|------|------|------|
| CNN Model | 0.9451 | 0.9251 | 0.9922 | 0.9931 |
| DenseNet121 | 0.9677 | 0.9668 | 0.9818 | 0.9949 |
| MobileNetV2 | 0.9822 | 0.9820 | 0.9896 | 0.9951 |

MobileNetV2 achieved the best overall performance and was selected for deployment in the application.

---

# Project Files

- `chest_xray_app.py` → Streamlit application
- `MobileNetV2_Model.keras` → Trained MobileNetV2 model
- `chest-x-ray-pneumonia-detection.ipynb` → Kaggle notebook for training and testing
- `API_key.env` → Gemini API key file
- `requirements.txt` → Required Python libraries

---

# Dataset

The dataset used in this project is available on Kaggle:

[Chest X-Ray Dataset](https://www.kaggle.com/datasets/vivek468/beginner-chest-xray-image-classification/data?utm_source=chatgpt.com)

---

# How to Run the Kaggle Notebook

1. Open Kaggle.
2. Upload or open the notebook file:

```bash
chest-x-ray-pneumonia-detection.ipynb
Add the dataset to the notebook:
Click "Add Input"
Search for the dataset
Add the Chest X-Ray dataset
Run all notebook cells sequentially.

The notebook performs:

Data preprocessing
Model training
Evaluation
Visualization
Saving the trained model
Create a Conda Environment
Create the environment
conda create -n x_ray python=3.11 -y
Activate the environment
conda activate x_ray
Install Required Libraries

All required libraries are included in the requirements.txt file.

Install them using:

pip install -r requirements.txt
Gemini API Key Setup

Create a file named:

API_key.env

Add your Gemini API key inside the file:

GOOGLE_API_KEY=your_api_key_here
How to Run the Application

Run the Streamlit application using:

streamlit run chest_xray_app.py

After running the command, Streamlit will generate a local URL similar to:

http://localhost:8501

Open the link in your browser.

Application Workflow
Upload a Chest X-ray image
The AI model predicts whether Pneumonia is detected
Gemini AI generates:
Radiology Report
Patient Advice
Arabic translation is generated
The report can be exported as a PDF

Future Improvements
Multi-disease chest X-ray classification
Cloud deployment
Real-time hospital integration
Improved report generation
Advanced explainable AI visualization
Author

Eslam Eid Abdullah

Faculty of Computer Science
Arab Open University
