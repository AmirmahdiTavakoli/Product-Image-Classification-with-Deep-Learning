# Product-Image-Classification-with-Deep-Learning
# 🛍️ Product Image Classification using Deep Learning

## 📖 Overview
This project implements a deep learning model for classifying e-commerce products from images. The goal is to accurately assign product categories using CNN architectures and improve the efficiency of inventory management and customer experience.

## 🛠️ Tech Stack
- Python
- TensorFlow / Keras / PyTorch
- NumPy, Pandas, Matplotlib
- OpenCV
- Scikit-learn

## 📊 Dataset
- **Training Set:** 10 categories, ~1000 images per category  
- **Test Set:** 4000 unlabeled images  
- Images were provided in category-labeled folders.

## 🚀 Models Used
- Pre-trained CNN models (Transfer Learning):
  - ResNet
  - VGG
  - Inception
  - MobileNet
- Custom CNN models were also tested.

## 🧪 Data Preprocessing & Augmentation
- Resized images to 224x224 pixels.
- Applied random flips, rotations, and zooms.
- Normalized pixel values to [0, 1].

## ⚙️ Hyperparameter Tuning
- Batch size: 32  
- Learning rate: 0.001 (with decay)  
- Optimizer: Adam  
- Epochs: 20  

## 📈 Evaluation Metric
- F1-score (micro average) on test predictions.  
- Visualized sample predictions and confusion matrices.  

## 📁 Output
- CSV file (`q1_submission.csv`) with image names and predicted categories.

## 🚀 How to Run
1. Clone the repository:
   ```bash
   git clone https://github.com/username/product-image-classification.git
   cd product-image-classification

    Install dependencies:

pip install -r requirements.txt

Run the training script:

python train.py

Generate predictions for the test set:

    python predict.py

    Submit the output CSV (q1_submission.csv).

🏆 Results

    Best Model: MobileNet with Transfer Learning
    F1-score (micro): 92.4%
