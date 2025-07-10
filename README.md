# Handwritten Digit Recognition with MNIST  
**TensorFlow · Deep Learning · Image Prediction**

This project implements a simple deep learning model that trains on the MNIST dataset of handwritten digits to recognize and classify numbers (0–9).  
After training, it evaluates performance on test data and predicts digits from custom image inputs.

---

## 📌 How It Works

### 1. Load Dataset  
- Loads 60,000 training and 10,000 testing images from `tf.keras.datasets.mnist`.

### 2. Normalize  
- Input data (28x28 grayscale images) is normalized to improve learning efficiency.

### 3. Build Model  
A basic neural network with:
- `Flatten` layer for 1D conversion  
- Two `Dense` layers with ReLU activation  
- `Dense` output layer with softmax for 10-class classification

### 4. Train Model  
- Trains over 3 epochs  
- Uses Adam optimizer and sparse categorical cross-entropy loss

### 5. Save & Load Model  
- Saves the trained model as `handwritten.h5`  
- Reloads the model for predictions

### 6. Evaluate  
- Evaluates performance on test set  
- Prints test loss and accuracy

### 7. Predict  
- Loops through images in the `digits/` directory  
- Preprocesses each image using OpenCV  
- Predicts the most probable digit

---

## 📌 Features

- Clean and simple digit classification pipeline  
- Fast training (small model & dataset)  
- Real image prediction using OpenCV  
- Model saving and reuse with `.h5` format

---

## ❌ Limitations

- Basic model — not state-of-the-art accuracy  
- Only supports grayscale `.png` images for predictions  
- No error handling for badly formatted or sized images  


---



