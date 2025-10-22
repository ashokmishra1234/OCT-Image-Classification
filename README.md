🩺 OCT Retinal Disease Classification
📘 Project Overview

This project focuses on automated classification of Optical Coherence Tomography (OCT) retinal images into four diagnostic categories using a fine-tuned MobileNetV3 model. It enables clinicians and researchers to perform real-time retinal disease detection through an interactive Streamlit web application.

🚀 Key Highlights

Model Architecture: Fine-tuned MobileNetV3 pre-trained on ImageNet for OCT image classification.

Performance: Achieved 95.03% validation accuracy and macro F1-score = 0.91.

Deployment: Built an interactive Streamlit interface for real-time inference and visualization.

Data Efficiency: Enhanced model generalization using data augmentation, transfer learning, and optimized training protocols.

🧠 Model Capabilities

The model classifies retinal OCT images into four disease categories:

Class	Description
CNV (Choroidal Neovascularization)	Neovascular membrane with subretinal fluid
DME (Diabetic Macular Edema)	Retinal thickening and intraretinal fluid
Drusen (Early AMD)	Multiple drusen deposits beneath the retina
Normal	Preserved foveal contour with no retinal abnormalities
🧩 Tech Stack

Programming Language: Python

Deep Learning Framework: TensorFlow / Keras

Model: MobileNetV3 (Fine-tuned)

Web App Framework: Streamlit

Libraries: NumPy, Pandas, Matplotlib

Deployment Tools: Streamlit, TensorFlow SavedModel

📂 Project Structure
OCT-Medical-Image-Classification/
│
├── Trained_Model.h5                # Fine-tuned MobileNetV3 model
├── app.py                          # Streamlit application code
├── recommendation.py               # Disease description and recommendations
├── requirements.txt                # Dependencies
├── README.md                       # Project documentation
└── sample_images/                  # Sample OCT test images

⚙️ How It Works

Upload an OCT image through the web interface.

The model preprocesses the image (resize → normalize → batch).

The fine-tuned MobileNetV3 model predicts the disease category.

The app displays the predicted diagnosis and medical insights for that category.

💻 Installation & Usage

Clone the Repository

git clone https://github.com/<your-username>/OCT-Medical-Image-Classification.git
cd OCT-Medical-Image-Classification


Install Dependencies

pip install -r requirements.txt


Run the App

streamlit run app.py


Access the Dashboard
Open your browser at 👉 http://localhost:8501

📊 Dataset Description

Source: Retinal OCT dataset by Kermany et al., 2018 (UCSD, Kaggle).

Size: 84,495 high-resolution images.

Categories: CNV, DME, Drusen, Normal.

Splits: Train / Validation / Test.

Preprocessing: Resizing (224×224), normalization, data augmentation.

🧪 Results Summary
Metric	Value
Validation Accuracy	95.03%
Macro F1-Score	0.91
Model Input Size	224×224×3
Training Epochs	25 (with early stopping)
🖼️ Streamlit Demo Features

Upload and classify OCT images in real-time.

View disease-specific details and recommendations.

Interactive and clean UI with categorized explanations.
