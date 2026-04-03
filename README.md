# Blood-Group-Detection-DeepLearning
Deep learning-based blood group classification from agglutination images using CNN and Firefly Optimization with Django deployment

This project is a deep learning-based system that classifies human blood groups (A, B, AB, O) from agglutination images.  
It uses a Convolutional Neural Network (CNN) along with Firefly Optimization for improved performance.  
The system also includes a Django-based web interface for real-time prediction.

## Features

- Blood group classification from images
- CNN-based deep learning model
- Image preprocessing (resizing, normalization, denoising, segmentation)
- Hyperparameter tuning using Firefly Optimization
- Django web interface for prediction
- Upload image and get instant result
- Sample test images included


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

---

## Prerequisites

- Python 3.x
- pip
- Virtual environment (optional but recommended)

---

## Setup Instructions

### Backend (Django)

1. Clone the repository:


2. Navigate to project folder:
cd Blood-Group-Detection-DeepLearning


3. Install dependencies:
pip install -r requirements.txt


---

## Running the Application

1. Start the Django server:
   python manage.py runserver
2. Open browser:
   (http://127.0.0.1:8000/)
3. Upload an image and get prediction.

## Model Details

- Model: Convolutional Neural Network (CNN)
- Optimization: Firefly Optimization Algorithm
- Input size: 32x32 images
- Classes: A, B, AB, O
- Framework: TensorFlow / Keras

---

## Future Scope

- Include Rh factor classification (positive/negative)
- Real-time detection using camera
- Mobile application deployment
- Larger dataset for improved accuracy

  ## License

This project is for educational purposes.
