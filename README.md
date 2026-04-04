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
- Optimized model performance using Firefly Optimization Algorithm
- Image preprocessing including resizing, normalization, and segmentation
- Real-time prediction using a Django web interface


## 📁 Project Structure

```
Blood/               # Django project settings

BloodApp/            # Main application
├── templates/       # HTML files
├── static/          # CSS and images
├── views.py
├── models.py
├── urls.py
├── admin.py
├── apps.py

model/               # Trained model files (e.g., .h5, .npy)
testimages/          # Sample test images

manage.py
requirements.txt
README.md
```


## ⚙️ Prerequisites

Make sure the following are installed on your system:

- Python 3.x
- pip (Python package manager)
- Virtual environment (optional but recommended)

Required python libraries:
- TensorFlow
- Keras
- OpenCV
- NumPy
- Matplotlib
- Django
- Scikit-learn
---

## 🛠️ Setup Instructions

### 🔧 Backend (Django Setup)

1. Clone the repository:
  ``` 
git clone
https://github.com/PollreddySreeja/Blood-Group-Detection-DeepLearning.git
cd Blood-Group-Detection-DeepLearning
```
2. Create and activate virtual environment:
``` 
python -m venv venv
venv\Scripts\activate   # Windows
# OR
source venv/bin/activate   # Mac/Linux
``` 
3. Install dependencies:
```
pip install -r requirements.txt
```
---

## 🗄️ Database Setup

If using XAMPP for MySQL:

1. Open XAMPP Control Panel  
2. Start MySQL service (Apache is optional unless specifically configured) 
3. Ensure MySQL is running  
4. Update database settings in settings.py if required  

Note: If using SQLite, this step can be skipped.

## ▶️ Running the Application

1. Start the Django server:
   ```
   python manage.py runserver
   ```
3. Open in browser:
    ```
   http://127.0.0.1:8000/
   ```
5. Upload an image and get the predicted blood group.

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
- Input size: 32×32 pixels
- Classes: A, B, AB, O
- Optimization: Firefly Optimization Algorithm
- Framework: TensorFlow (Keras API)

## 📊 Dataset

- Contains agglutination images of blood samples
- Approximately 200+ labeled images
- Four classes: A, B, AB, O
- Only a subset of sample images are included in this repository
  
## 🛠️ Troubleshooting

- Ensure all required dependencies are installed correctly
- Verify that the correct Python version is being used
- Verify that model files are present in the 'model/' directory
- Make sure the Django server is running before accessing the application

## Future Scope

- Extend classification to include Rh factor (positive/negative)
- Enable real-time blood group detection using a camera
- Deploy the system as a Mobile application 
- Utilize a larger dataset to further improved model accuracy
  This system reduces dependency on manual laboratory interpretation and demonstrates the potential of AI in medical image analysis.

## 📄 License

This project is licensed under the MIT License.
