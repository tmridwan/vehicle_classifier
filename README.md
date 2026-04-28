# 🚗 Vehicle Classification using Deep Learning

A complete end-to-end deep learning project that classifies vehicle images using a pretrained CNN model and provides an interactive web interface for real-time predictions.

---

## 📌 Overview

This project uses a Convolutional Neural Network (CNN) built with **fastai** and **PyTorch** to classify different types of vehicles (e.g., car, bus, truck, etc.).

It includes:

* 📊 Model training notebook
* 🧠 Pretrained model (`.pkl`)
* 🌐 Web app using Gradio for real-time predictions

---

## 🧠 How It Works

1. Images are collected and organized into labeled folders
2. A pretrained CNN model (ConvNeXt) is fine-tuned on the dataset
3. The trained model is saved as `vehicle_model.pkl`
4. A Gradio app loads the model and predicts vehicle types from user-uploaded images

---

## 📂 Project Structure

```
vehicle/
│
├── app.py                     # Gradio web app
├── vehicle_model.pkl          # Trained model
├── requirements.txt           # Dependencies
├── runtime.txt                # Runtime config (for deployment)
│
├── data/                      # Training dataset
├── models/                    # Saved models (optional)
├── notebooks/
│   └── vehicle_types.ipynb    # Training notebook
│
├── vehicle_dataloader_v0.pkl  # Saved dataloader
└── README.md
```

---

## 🚀 Features

* ✅ Image classification using deep learning
* ✅ Pretrained model (ConvNeXt via timm)
* ✅ Real-time prediction via web UI
* ✅ Batch image prediction support
* ✅ Image preprocessing (resize, auto-contrast)
* ✅ Error handling for invalid images

---

## 🛠️ Tech Stack

* **fastai** – High-level deep learning framework
* **PyTorch** – Backend for model training
* **timm** – Pretrained models (ConvNeXt)
* **Gradio** – Web interface for deployment
* **Pillow (PIL)** – Image processing

---

## ⚙️ Installation

### 1. Clone the repository

```bash
git clone <your-repo-url>
cd vehicle
```

### 2. Create virtual environment (optional but recommended)

```bash
python -m venv venv
source venv/bin/activate   # Linux/Mac
venv\Scripts\activate      # Windows
```

### 3. Install dependencies

```bash
pip install -r requirements.txt
```

---

## ▶️ Run the App

```bash
python app.py
```

Then open your browser at:

```
http://localhost:7860
```

---

## 📸 Usage

* Upload an image or use your webcam
* Adjust preprocessing settings (optional)
* View:

  * Top prediction
  * Top 5 probabilities
  * Processed image preview

---

## 🧪 Model Training

Training is done in:

```
notebooks/vehicle_types.ipynb
```

Steps:

* Data loading using DataBlock
* Image preprocessing
* Model creation using `vision_learner`
* Fine-tuning pretrained ConvNeXt model
* Saving model using `model.save()` / `export()`

---

## 📊 Example Output

```
Top Prediction: Car
Confidence: 0.92
```

---

## 🔥 Key Concepts Used

* Convolutional Neural Networks (CNN)
* Transfer Learning
* DataBlock API (fastai)
* Image preprocessing
* Model deployment

---

## ⚠️ Notes

* Ensure `vehicle_model.pkl` is in the same directory as `app.py`
* Large model size (~700MB) may take time to load initially
* HEIC images require `pillow-heif` (optional)

---

## 👨‍💻 Author

Taiob Md Ridwan

---

## 📜 License

This project is open-source and available under the MIT License.
