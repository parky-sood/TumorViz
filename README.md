# 🧠 TumorViz

[![Python](https://img.shields.io/badge/Python-3.7%2B-blue.svg)](https://www.python.org/)
[![TensorFlow](https://img.shields.io/badge/TensorFlow-2.0%2B-orange.svg)](https://www.tensorflow.org/)
[![Streamlit](https://img.shields.io/badge/Streamlit-1.0%2B-red.svg)](https://streamlit.io/)

A deep learning project that uses transfer learning and custom CNN architectures to classify brain tumors from MRI scans into four categories: Glioma, Meningioma, Pituitary, and No Tumor.

## 🎯 Project Overview

This project implements two different deep learning approaches:

1. **Transfer Learning with Xception**: Leveraging a pre-trained model for enhanced accuracy
2. **Custom CNN**: A dedicated convolutional neural network built from scratch

Both models are deployed through a user-friendly Streamlit web interface that provides:

- Real-time tumor classification
- Confidence scores
- Saliency maps for model interpretability
- AI-generated explanations of the model's focus areas

## 📊 Model Architecture & Performance

### Transfer Learning Model (Xception)

- Pre-trained on ImageNet dataset
- 36 convolutional layers
- 21 million parameters
- Features:
  - Max pooling
  - Dropout layers for regularization
  - Softmax activation for classification
- Performance metrics:
  - High accuracy on test set
  - Robust against overfitting

### Custom CNN Model

- 4 convolutional layers
- 4.7 million parameters
- Architecture:
  - Multiple Conv2D layers with ReLU activation
  - MaxPooling2D layers
  - Dropout for regularization
  - Dense layers with L2 regularization
  - Softmax output layer

## 🛠️ Installation

```bash
# Clone the repository
git clone https://github.com/parky-sood/TumorViz.git
cd TumorViz

# Install required packages
pip install -r requirements.txt
```

## 📦 Dependencies

- tensorflow >= 2.0
- streamlit
- numpy
- pandas
- pillow
- plotly
- opencv-python
- google-generativeai
- python-dotenv

## 🚀 Usage

### Running the Web App

```bash
streamlit run app.py
```

## 🖥️ Web Interface Features

1. **Image Upload**: Support for jpg, jpeg, and png formats
2. **Model Selection**: Choose between Transfer Learning and Custom CNN
3. **Visualization**:
   - Original MRI scan
   - Saliency map highlighting model focus areas
4. **Results Display**:
   - Predicted tumor type
   - Confidence scores
   - Interactive probability chart
   - AI-generated explanation of the classification

## 📈 Data Processing

The project includes robust data handling:

- Image preprocessing and augmentation
- Brightness adjustment for training data
- Proper train/validation/test splits
- Standardized image sizing

## 🔍 Model Interpretability

- **Saliency Maps**: Visual explanation of model decisions
- **Region Focus**: Highlights critical areas in MRI scans
- **AI Explanations**: Generated using Google's Gemini model
- **Confidence Metrics**: Probability distribution across classes

## 👥 Contributing

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📧 Contact

Parikshit Sood - parikshitsood.com

Project Link: [https://github.com/parky-sood/TumorViz](https://github.com/parky-sood/TumorViz)
