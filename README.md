# Automated Chest X-Ray Report Generation and Pneumonia Detection System

An AI-powered medical imaging system for detecting pneumonia from chest X-ray images and automatically generating medical radiology reports, patient advice, Arabic translations, and downloadable PDF reports.

---

# Project Overview

This project combines Deep Learning and Generative AI technologies to create an intelligent medical assistant capable of:

- Detecting pneumonia from chest X-ray images
- Generating detailed radiology reports
- Providing patient advice
- Translating reports and advice into Arabic
- Exporting reports as downloadable PDFs

The system uses Transfer Learning models such as DenseNet121 and MobileNetV2 for image classification and integrates the Gemini AI model for medical report generation.

---

# Features

- Pneumonia Detection from Chest X-rays
- Medical Report Generation using Gemini AI
- Patient Advice Generation
- Arabic Translation of Reports and Advice
- PDF Report Export
- Streamlit-based User Interface
- Transfer Learning Models
- Kaggle Notebook for Training and Evaluation

---

# Models Used

| Model | Accuracy | Precision | Recall | AUC |
|------|------|------|------|------|
| CNN Model | 0.9451 | 0.9251 | 0.9922 | 0.9931 |
| DenseNet121 | 0.9677 | 0.9668 | 0.9818 | 0.9949 |
| MobileNetV2 | 0.9822 | 0.9820 | 0.9896 | 0.9951 |

MobileNetV2 achieved the best overall performance and was selected for deployment in the final application.

---

# Technologies Used

- Python
- TensorFlow / Keras
- Streamlit
- Gemini AI API
- OpenCV
- PIL
- Transfer Learning
- ReportLab / FPDF

---

# Project Files

| File Name | Description |
|------|------|
| `chest_xray_app.py` | Streamlit application |
| `MobileNetV2_Model.keras` | Trained MobileNetV2 model |
| `chest-x-ray-pneumonia-detection.ipynb` | Kaggle notebook for training and testing |
| `API_key.env` | Gemini API key |
| `requirements.txt` | Required Python libraries |

---

# Dataset

The dataset used in this project is available on Kaggle:

[Chest X-Ray Dataset](https://www.kaggle.com/datasets/vivek468/beginner-chest-xray-image-classification/data?utm_source=chatgpt.com)

---

# How to Run the Kaggle Notebook

## Step 1: Open Kaggle

Go to:

[Kaggle](https://www.kaggle.com?utm_source=chatgpt.com)

---

## Step 2: Upload the Notebook

Upload the following notebook file:

```bash
chest-x-ray-pneumonia-detection.ipynb
```

---

## Step 3: Add the Dataset

1. Click **Add Input**
2. Search for the dataset
3. Add the Chest X-Ray dataset to the notebook

Dataset link:

[Chest X-Ray Dataset](https://www.kaggle.com/datasets/vivek468/beginner-chest-xray-image-classification/data?utm_source=chatgpt.com)

---

## Step 4: Run All Cells

Run all notebook cells sequentially.

The notebook performs:
- Data preprocessing
- Model training
- Model evaluation
- Performance visualization
- Saving trained models

---

# Create a Conda Environment

## Create Environment

```bash
conda create -n x_ray python=3.11 -y
```

---

## Activate Environment

```bash
conda activate x_ray
```

---

# Install Required Libraries

Install all required libraries using:

```bash
pip install -r requirements.txt
```

---

# Gemini API Key Setup

Create a file named:

```bash
API_key.env
```

Add your Gemini API key inside the file:

```env
GOOGLE_API_KEY=your_api_key_here
```

---

# How to Run the Application

Run the Streamlit application using:

```bash
streamlit run chest_xray_app.py
```

After running the command, Streamlit will generate a local URL similar to:

```bash
http://localhost:8501
```

Open the link in your browser.

---

# Application Workflow

1. Upload a Chest X-ray image
2. The AI model predicts the diagnosis
3. Gemini AI generates:
   - Radiology report
   - Patient advice
4. Arabic translation is generated
5. PDF report becomes available for download

---

# Future Improvements

- Multi-disease chest X-ray classification
- Cloud deployment
- Real-time hospital integration
- Explainable AI visualization
- Enhanced report generation

---

# Author

## Eslam Eid Abdullah

Faculty of Computer Science  
Arab Open University
