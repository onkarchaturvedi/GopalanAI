An automated cattle body condition scoring system using ArUco Markers for detection and ResNet50 for classification. This project also secured selection in Smart India Hackathon 2025, a national-level government innovation challenge.

# 🐄 [Gopalan AI](https://www.gopalanai.xo.je)

Gopalan AI is an AI-powered cattle analysis system that combines **Deep Learning**, **Computer Vision**, and **Geometric Measurement Techniques** to analyze cattle from images.

The system can:

* ✅ Identify cattle breed
* ✅ Estimate Body Condition Score (BCS)
* ✅ Estimate live body weight
* ✅ Analyze physical measurements using real-world scaling
* ✅ Provide detailed explainable outputs

The project is deployed using **Gradio** and can run as an interactive web application.

---

# 🚀 Features

## 1️⃣ Breed Classification

The first stage of the pipeline identifies the cattle breed using a **ResNet50-based deep learning model** trained on multiple Indian cattle and buffalo breeds.

### Supported Breeds

* Ayrshire
* Banni
* Bhadawari
* Brown Swiss
* Gir
* Guernsey
* Holstein Friesian
* Jaffrabadi
* Kankrej
* Mehsana
* Murrah
* Nagpuri
* Nili Ravi
* Ongole
* Tharparkar

The model also provides:

* Cattle category (Cow/Buffalo)
* Average breed height
* Chest width
* Milk production statistics

---

## 2️⃣ Body Condition Scoring (BCS)

The second stage estimates the **Body Condition Score** of the animal using physical body measurements extracted from images.

### Required Views

The system uses:

* Side View
* Top View
* Back View

### User Interaction

Users manually select anatomical key points such as:

* Nose
* Tail
* Back
* Belly
* Knee
* Hoof
* Rib area
* Hip points
* Rump points

---

## 3️⃣ Real-World Measurement Scaling

The system uses **ArUCo markers** for converting image pixel distances into real-world centimeter measurements.

This allows accurate estimation of:

* Body Length
* Body Depth
* Leg Length
* Hip Width
* Rump Width

---

## 4️⃣ Rib Visibility Analysis

Computer vision techniques such as:

* Edge Detection
* Canny Filtering

are used to estimate rib visibility, which contributes to body condition analysis.

---

## 5️⃣ Weight Estimation

The project estimates approximate live body weight using:

* Body dimensions
* Elliptical body approximation
* Heart girth estimation
* Empirical livestock formulas

The system uses:

* Body depth
* Body length
* Hip width
* Rump width
* Rib visibility

to estimate live cattle weight.

---

# 🧠 Technologies Used

## Deep Learning

* PyTorch
* TIMM
* ResNet50

## Computer Vision

* OpenCV
* ArUCo Marker Detection
* Edge Detection

## Frontend / Deployment

* Gradio
* Hugging Face Spaces

---

# 📊 Pipeline Overview

```text
Input Animal Image
        │
        ▼
Breed Classification (ResNet50)
        │
        ▼
Multi-View Image Upload
(Side / Top / Back)
        │
        ▼
Key Point Selection
        │
        ▼
Real-World Measurement Extraction
        │
        ▼
Rib Visibility Analysis
        │
        ▼
BCS + Weight Estimation
        │
        ▼
Final Explainable Report
```

---

### Visit the AI App now -> [Gopalan AI](https://www.gopalanai.xo.je)

# 👨‍💻 Author

Developed by Onkar Chaturvedi.

