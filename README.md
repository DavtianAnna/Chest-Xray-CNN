# 🩻 Chest X-ray Classification using CNN  

This repository implements a **Convolutional Neural Network (CNN)** for classifying chest X-ray images as **Normal** or **Pneumonia (Abnormal)**.  
The model is built using **Keras (TensorFlow backend)**.  

---

## 🚀 Overview  

- **Goal** – Detect pneumonia from chest X-ray images  
- **Dataset** – [Chest X-ray dataset (Kaggle)](https://www.kaggle.com/paultimothymooney/chest-xray-pneumonia)  
- **Model** – Custom CNN Sequential architecture  
- **Output** – Two classes: `Normal` or `Pneumonia`  

---

## 🛠️ Tech Stack  

- Python 3.x  
- TensorFlow / Keras  
- NumPy  
- OpenCV  
- Matplotlib  
- Scikit-learn  

---

## 📂 Project Structure  


```

📁 Chest-Xray-CNN/
│── 📄 Untitled.ipynb           # Jupyter Notebook with full code
│── 📂 chest_xray/              # Dataset (train/test/val)
└── 📜 README.md                # Project documentation.

```

---

## 🧠 Model Architecture  

- **Input shape** – 256×256×1 (grayscale)  
- **Layers** –  
  - Conv2D → MaxPooling  
  - Conv2D → MaxPooling  
  - Conv2D → MaxPooling  
  - Conv2D → MaxPooling  
  - Flatten  
  - Dense (512, ReLU)  
  - Dense (256, ReLU)  
  - Dense (2, Sigmoid)  
- **Loss** – Binary Crossentropy  
- **Optimizer** – Adam (lr=0.001)  
- **Metrics** – Accuracy  

---

## 📊 Training  

- **Epochs** – 7  
- **Batch size** – 15  
- Train/validation/test split applied  
- Training history tracked with accuracy & validation accuracy plots  

---

## 🔍 Results  

- Validation accuracy ≈ **97–98%**  
- Accuracy & loss curves visualized**

---

## ▶️ How to Run  

```bash
# Clone the repository
git clone https://github.com/your-username/Chest-Xray-CNN.git
cd Chest-Xray-CNN

# Install dependencies
pip install -r requirements.txt

# Run the Jupyter notebook
jupyter notebook Untitled.ipynb
