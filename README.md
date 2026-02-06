# 🚗 Vehicle Recognizer

A powerful web application that uses deep learning to classify and identify 72 different types of vehicles from images. Built with FastAI and deployed on Hugging Face Spaces with a beautiful, modern web interface.

[![Live Demo](https://img.shields.io/badge/demo-live-brightgreen)](https://tmridwan.github.io/vehicle_classifier/)
[![Hugging Face](https://img.shields.io/badge/🤗-Hugging%20Face-yellow)](https://huggingface.co/spaces/tmridwan03/vehicle_recognizer)
[![License](https://img.shields.io/badge/license-MIT-blue.svg)](LICENSE)

## ✨ Features

- 🎯 **Accurate Classification**: Identifies 72 different vehicle types with high accuracy
- 📸 **Multiple Input Methods**: Upload images or capture photos directly from your camera
- 🌙 **Modern Dark UI**: Beautiful, responsive interface with gradient accents
- ⚡ **Fast Inference**: Quick predictions powered by FastAI and Hugging Face
- 📱 **Mobile Friendly**: Works seamlessly on desktop and mobile devices
- 🎨 **Real-time Preview**: See your image before classification

## 🚀 Live Demo

Visit the live application: [https://tmridwan.github.io/vehicle_classifier/](https://tmridwan.github.io/vehicle_classifier/)

## 🛠️ Technologies Used

- **Frontend**: HTML5, TailwindCSS, JavaScript (ES6+)
- **Machine Learning**: FastAI, PyTorch
- **Deployment**: 
  - GitHub Pages (Frontend)
  - Hugging Face Spaces (ML Model API)
- **API**: Gradio Client for seamless communication

## 📋 Vehicle Types

The model can identify 72 different vehicle types including:
- Cars (sedan, SUV, coupe, etc.)
- Trucks (pickup, dump, tow, etc.)
- Buses (school, city, coach, etc.)
- Motorcycles
- Heavy machinery (excavators, bulldozers, etc.)
- And many more!

## 🎯 How It Works

1. **Upload or Capture**: Choose an image from your device or use your camera to take a photo
2. **Preview**: See the selected image before processing
3. **Classify**: Click "Recognize Vehicle" to get predictions
4. **Results**: View the predicted vehicle type instantly

## 💻 Local Development

### Prerequisites

- Python 3.8+
- Node.js (for local frontend testing)
- Git

### Setup

1. Clone the repository:
```bash
git clone https://github.com/tmridwan/vehicle_classifier.git
cd vehicle_classifier
```

2. For the frontend (GitHub Pages):
   - Simply open `index.html` in your browser
   - Or use a local server:
   ```bash
   python -m http.server 8000
   ```

3. For the model (Hugging Face Space):
   - Visit [Hugging Face Spaces](https://huggingface.co/spaces)
   - Create a new Space with Gradio SDK
   - Upload `app.py` and `vehicle_model.pkl`

## 📁 Project Structure

```
vehicle_classifier/
├── index.html              # Main web interface
├── vehicle_recognizer.html # Alternative interface
├── app.py                  # Gradio app for Hugging Face (separate repo)
├── README.md              # Project documentation
├── LICENSE                # MIT License
└── _config.yml           # Jekyll configuration
```

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

1. Fork the project
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📝 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 👨‍💻 Author

**Ridwan**

- GitHub: [@tmridwan](https://github.com/tmridwan)
- Hugging Face: [@tmridwan03](https://huggingface.co/tmridwan03)

## 🙏 Acknowledgments

- [FastAI](https://www.fast.ai/) for the amazing deep learning library
- [Hugging Face](https://huggingface.co/) for hosting the model
- [Tailwind CSS](https://tailwindcss.com/) for the beautiful styling
- [Unsplash](https://unsplash.com/) for background images

## 📊 Model Information

- **Framework**: FastAI
- **Architecture**: ResNet-based CNN
- **Training Dataset**: Custom vehicle dataset with 72 classes
- **Accuracy**: High accuracy on validation set
- **Input**: RGB images (auto-resized)
- **Output**: Vehicle class prediction with confidence score

---

Made with ❤️ by [Ridwan](https://github.com/tmridwan)