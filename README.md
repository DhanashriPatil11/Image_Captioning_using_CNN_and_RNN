# 🧠 Image Captioning using CNN + RNN

This project is part of my **TA3 submission** and focuses on generating captions for images using **deep learning techniques**. It combines **Convolutional Neural Networks (CNN)** for feature extraction and **Recurrent Neural Networks (RNN)** with **LSTM** for caption generation.

---

## 🗂️ Project Overview

- ✅ Uses **InceptionV3** (a pre-trained CNN) to extract features from images  
- ✅ Employs **LSTM** (Long Short-Term Memory) network to generate meaningful captions  
- ✅ Trained on a subset (500 images) of the [Flickr8k Dataset](https://www.kaggle.com/datasets/adityajn105/flickr8k)  
- ✅ Implemented in **Google Colab** using **Kaggle API** to load the dataset  

---

## 📥 Dataset Download (via Kaggle API)

1. Go to your [Kaggle Account Settings](https://www.kaggle.com/account)  
2. Scroll down and click **Create New API Token**  
3. Download `kaggle.json`, then upload it to Colab and run:

```python
from google.colab import files
files.upload()  # Upload kaggle.json

!mkdir -p ~/.kaggle
!cp kaggle.json ~/.kaggle/
!chmod 600 ~/.kaggle/kaggle.json

!kaggle datasets download -d adityajn105/flickr8k
!unzip -q flickr8k.zip
```

---

## 🚀 How to Run the Project

1. **Open the Colab notebook provided in the repo.**
2. **Run all cells sequentially to:**
   - ✅ Load and preprocess dataset
   - ✅ Extract image features using InceptionV3
   - ✅ Train the LSTM model
   - ✅ Generate image captions on unseen data

---

## 📊 Project Workflow

```
Dataset (Flickr8k) ➜ Preprocessing ➜ Feature Extraction (CNN - InceptionV3) ➜
Tokenization + Padding ➜ LSTM Model Training ➜ Caption Generation
```

---

## 🛠️ Tech Stack

| Category         | Tools & Frameworks                  |
|------------------|------------------------------------|
| Language         | Python                             |
| Deep Learning    | TensorFlow, Keras                  |
| CNN Architecture | InceptionV3 (Pre-trained on ImageNet) |
| Sequence Model   | LSTM (Long Short-Term Memory)      |
| Platform         | Google Colab                       |
| Data Source      | Flickr8k via Kaggle API            |

---

## 📸 Sample Image 

> ![image](https://github.com/user-attachments/assets/2b784090-8d77-4e13-bc27-77b7ec0bda4c)

## 📸 Sample Output Captions
> ![image](https://github.com/user-attachments/assets/37d329d9-4387-4253-bc39-e1d140d2f2e6)


*(Outputs will vary based on model training and sample images)*

---

## ✍️ Author

**Dhanashri Patil**  

---

⭐ Feel free to fork, star, or open issues if you find the project useful or want to contribute!

---

