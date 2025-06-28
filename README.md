# Week 2 Update
    -> retrained model with more train dataset to predict the correct output
    -> use array images to predict the output
    -> after retrained the model the accuaracy increase from 0.6 to 0.8 





# 🗑️ Garbage Classification using Convolutional Neural Networks (CNN)

This project uses a Convolutional Neural Network (CNN) model to classify garbage images into categories such as cardboard, glass, metal, paper, plastic, and trash. The model is trained on a publicly available dataset and can be deployed in smart bins or recycling systems.

---

## 📁 Dataset

**Dataset Used:** [TrashNet](https://github.com/garythung/trashnet)

**Categories:**
- Cardboard
- Glass
- Metal
- Paper
- Plastic
- Trash


Upload this dataset to your Google Drive and mount it in your Google Colab notebook.

---

## ⚙️ Technologies Used

| Technology     | Purpose                          |
|----------------|----------------------------------|
| Python         | Core programming language        |
| CNN            | Image classification model       |
| Google Colab   | Development & training platform  |
| Matplotlib     | Training accuracy visualization  |

---

## 🧠 Features

- Uses image data from real garbage categories
- Classifies images into 6 categories
- Trained using CNN with TensorFlow/Keras
- Achieves 85–95% accuracy depending on epochs
- Includes custom image prediction support
- Model saved as `.h5` file for reuse

---

## 🚀 How to Run (in Google Colab)

1. Upload the TrashNet dataset to Google Drive.
2. Mount Google Drive:
```python
from google.colab import drive
drive.mount('/content/drive')

Preprocess images using ImageDataGenerator with rescaling and resizing.

Build CNN model using Conv2D, MaxPooling2D, and Dense layers.

Train model with model.fit().

Save model:

model.save("garbage_classifier_model.h5")

Test prediction on new image:
model.predict(new_image_tensor)


