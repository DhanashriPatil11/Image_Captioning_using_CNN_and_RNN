# 🧠 Image Captioning using CNN + RNN

This is my TA3 project implemented using Google Colab, which generates captions for images using deep learning (CNN + RNN) on a subset of the Flickr8k dataset.

## 🗂 Project Overview

- Uses **CNN (InceptionV3)** to extract image features
- Uses **LSTM (RNN)** to generate captions
- Dataset: [Flickr8k](https://www.kaggle.com/datasets/adityajn105/flickr8k)
- Data loaded using **Kaggle API**, only 500 images used

## 📥 Dataset Download (via Kaggle API)

1. Go to [Kaggle > My Account](https://www.kaggle.com/account)
2. Click **Create API Token** → you'll get `kaggle.json`
3. Upload `kaggle.json` in Colab and run:

```python
from google.colab import files
files.upload()  # upload kaggle.json

!mkdir -p ~/.kaggle
!cp kaggle.json ~/.kaggle/
!chmod 600 ~/.kaggle/kaggle.json
!kaggle datasets download -d adityajn105/flickr8k
!unzip -q flickr8k.zip

---

## 🚀 How to Run
Open the notebook in Google Colab

Run cells in order to:

Load and preprocess dataset

Extract image features using InceptionV3

Train LSTM model

Generate captions for test images

---

## 🛠 Tech Stack
Python, TensorFlow, Keras

InceptionV3, LSTM

Google Colab, Kaggle API

---

## 👩‍💻 Author
Dhanashri Patil

