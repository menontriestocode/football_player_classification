# Golden Foot: Football Player Classification

This project implements a computer vision and machine learning pipeline for classifying football players based on facial images.  
It applies feature extraction, supervised learning, and API deployment techniques to identify players such as Cristiano Ronaldo, Lionel Messi, Zlatan Ibrahimović, Luka Modrić, and Edinson Cavani.  
Developed by **Vignesh Suresh Menon**, B.Tech Data Science (Final Year), Manipal Institute of Technology.

---

## 1. Project Overview

The objective of this project is to automate the identification of football players from images using classical computer vision and machine learning techniques.  
The workflow follows a structured process: data collection, cleaning, feature engineering, model training, and deployment via a Flask API.

---

## 2. Project Structure

| Section | Description |
|----------|--------------|
| **Part 1 – Introduction** | Overview of the classification problem and its scope. |
| **Part 2 – Data Collection** | Downloading and organizing images of selected football players. |
| **Part 3 – Data Cleaning** | Filtering and preprocessing images using OpenCV and Haar Cascades to retain clear facial images. |
| **Part 4 – Feature Engineering** | Extracting combined features using raw pixel intensities and wavelet transforms for robust representation. |
| **Part 5 – Model Training** | Training and evaluating classifiers such as Support Vector Machine, Random Forest, and Logistic Regression using GridSearchCV. |
| **Part 6 – API Server** | Implementing a Flask server to serve the trained model for real-time predictions. |
| **Part 7 – Deployment** | Packaging the model and deploying the Flask API on Render, Heroku, or AWS EC2. |

---

## 3. Technical Stack

**Programming Language:**  
- Python 3.x  

**Core Libraries:**  
- OpenCV  
- NumPy  
- pandas  
- scikit-learn  
- PyWavelets  
- Flask  
- joblib  

**Development Tools:**  
- Jupyter Notebook  
- Visual Studio Code  
- Git and GitHub  

**Deployment Platforms:**  
- Render  
- Heroku  
- AWS EC2  

---

## 4. Methodology

1. **Data Acquisition**  
   - Images of target football players collected through automated and manual scraping.  

2. **Preprocessing**  
   - OpenCV Haar Cascades used for face and eye detection.  
   - Misclassified, blurred, or low-quality samples removed.  
   - Images standardized to uniform size and format.  

3. **Feature Extraction**  
   - Combined raw pixel intensities with wavelet-based texture features.  
   - Stacked feature vectors for improved class separability.  

4. **Model Development**  
   - Evaluated classifiers: SVM, Random Forest, Logistic Regression.  
   - Hyperparameter tuning performed via GridSearchCV.  
   - Metrics: accuracy, precision, recall, F1-score.  

5. **Model Serving**  
   - Flask API exposes `/predict` endpoint for inference.  
   - Accepts image input and returns predicted player label with confidence score.  

6. **Deployment**  
   - Model serialized with joblib.  
   - Flask app packaged for deployment on Render/Heroku/AWS EC2.  

---

## 5. Results

- Achieved high classification accuracy across five footballers.  
- Demonstrated consistent recognition under varied lighting and poses.  
- Flask API delivers fast and reliable prediction performance.  

---

## 6. Future Enhancements

- Extend dataset to include additional players and diverse image sources.  
- Integrate deep learning architectures (CNNs, transfer learning using VGG16 or ResNet).  
- Implement automated image augmentation for improved model generalization.  
- Deploy at scale with GPU-enabled cloud infrastructure for faster inference.  

---

## 7. Author

**Vignesh Suresh Menon**  
B.Tech Data Science, Final Year  
Manipal Institute of Technology, Manipal  
Email: [menonvigneshbiz@gmail.com](mailto:menonvigneshbiz@gmail.com)  
Phone: +91 8977637177  

---

## 8. License

This project is intended for educational and research purposes.  
All player images remain the property of their respective owners and are used strictly under fair-use academic demonstration.
