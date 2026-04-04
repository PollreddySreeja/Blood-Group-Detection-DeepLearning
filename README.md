# Blood-Group-Detection-DeepLearning
This project presents an end-to-end deep learning system for automated blood group classification from agglutination images using CNN and Firefly Optimization, integrated with a Django-based web interface for real-time prediction.

## 📑 Table of Contents

- [Features](#features)
- [Project Structure](#project-structure)
- [Prerequisites](#prerequisites)
- [Setup Instructions](#setup-instructions)
  - [Backend](#backend)
- [Running the Application](#running-the-application) 
- [Performance Metrics](#performance-metrics)
- [Model Details](#model-details)
- [Dataset](#dataset)
- [Troubleshooting](#troubleshooting)
- [Future Scope](#future-scope)
- [License](#license)

  
## 🚀 Features

- Automated blood group classification from agglutination images
- Deep CNN architecture for feature extraction
- Optimized model performance using Firefly Optimization
- Robust preprocessing pipeline for noise reduction and segmentation
- Real-time prediction using Django web interface


## 📁 Project Structure

```
├── Blood/ # Django project settings

├── BloodApp/ # Main application
│ ├── templates/ # HTML files
│ ├── static/ # CSS and images
│ ├── views.py
│ ├── models.py
│ ├── urls.py
│
├── model/ # Trained model and data files
├── testImages/ # Sample test images
├── manage.py
├── requirements.txt
└── README.md
```


## ⚙️ Prerequisites

Ensure the following are installed on your system:

- Python 3.x
- pip (Python package manager)
- Core libraries: TensorFlow, Keras, OpenCV, NumPy, Matplotlib, Django, Scikit-learn
- Virtual environment (optional but recommended)
---

## 🛠️ Setup Instructions
### Backend (Django)

1. Open a terminal and navigate to the project directory:
$
git clone
https://github.com/PollreddySreeja/Blood-Group-Detection-DeepLearning.git
cd Blood-Group-Detection-DeepLearning
$

2. Install dependencies:
```
pip install -r requirements.txt
```

---

## 🗄️ Database Setup

If using XAMPP for MySQL:

1. Open XAMPP Control Panel  
2. Start Apache and MySQL services  
3. Ensure MySQL is running  
4. Update database credentials in Django settings if required  

Note: If using SQLite, this step can be skipped.

## ▶️ Running the Application

1. Start the Django server:
   ```
   python manage.py runserver
   ```
3. Open browser:
    ```
   http://127.0.0.1:8000/
   ```
5. Upload an image and get prediction.

## 📈 Performance Metrics
 ```
- Accuracy: 98%
- Precision: 98.68%
- Recall: 98.07%
- F1-score: 98.32%
  ```

---
## 🧠 Model Details

- Model: Convolutional Neural Network
- Input size: 32×32 images
- Classes: A, B, AB, O
- Optimization: Firefly Optimization Algorithm
- Framework: TensorFlow / Keras

## 📊 Dataset

- Contains agglutination images of blood samples
- Approximately 200+ images
- Four classes: A, B, AB, O
- Only sample images are included in this repository
  
## 🛠️ Troubleshooting

- Ensure all dependencies are installed correctly
- Check if the correct Python version is used
- Verify model files are present in the model folder
- Make sure the Django server is running before accessing the application

## Future Scope

- Include Rh factor classification (positive/negative)
- Real-time detection using camera
- Mobile application deployment
- Larger dataset for improved accuracy

  This system reduces dependency on manual laboratory interpretation and demonstrates the potential of AI in medical image analysis.

## 📄 License

This project is for educational purposes.
