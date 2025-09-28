# 🌟 IsThisReal.AI – AI-Generated Image Detection Browser Extension  

A **real-time browser extension** that detects whether an image is AI-generated or real using a deep learning model (Vision Transformer).  
This tool aims to combat misinformation by helping users instantly identify synthetic images while browsing social media or any web page.  

---

## 🚀 Features  

- 🖼️ **Hover-based detection** — no click or upload required  
- ⚡ **Real-time predictions** using a Vision Transformer model  
- 🧠 **Trained on 500,000+ images** (AI-generated + real)  
- 🌐 **Lightweight Chrome Extension** for seamless browsing  
- 🔍 **Flask-based backend** for model inference  

---

## 🛠️ Tech Stack  

### 💻 Frontend / Extension  
- JavaScript (Core logic)  
- HTML/CSS (UI)  
- Chrome Extension APIs  
- FileReader API (Image conversion to Base64)  
- DOM Manipulation  

### 🧠 Backend & Model  
- Python  
- Flask (API server)  
- PyTorch  
- Hugging Face Transformers  
- Vision Transformer (ViT)  
- Custom image datasets  
- Image augmentation (resizing, cropping, normalization)  

---

## 📊 Model Training  

- **Architecture:** ViT (Vision Transformer) from Hugging Face  
- **Dataset:** 500,000 images (250k real + 250k AI-generated)  
- **Training/Validation Split:** 75% / 25%  
- **Accuracy:** 🎯 **92.93%** on test data  
- Loss & Confusion matrix tracked for validation  

---

## 📂 Datasets Used  

1. Sharma AI vs Real Images Dataset  
   🔗 https://www.kaggle.com/datasets/harsh7489/sharma-ai-real-images-dataset/data  

2. Sharma AI vs Real Images Dataset V2  
   🔗 https://www.kaggle.com/datasets/harsh7489/sharma-ai-real-images-dataset-v2/data  

3. 140K Real and Fake Faces Dataset  
   🔗 https://www.kaggle.com/datasets/xhlulu/140k-real-and-fake-faces  

---

## 🖼️ How It Works (System Flow)  

1. User **hovers over an image** in the browser  
2. Image is **converted to Base64** using FileReader API  
3. Base64 image is **sent to the Flask server**  
4. **ViT model predicts** whether it's AI or Real  
5. **Result is displayed** on the image as a real-time overlay  

---

## 📌 Limitations  

- ⚠️ May underperform on AI models not seen during training  
- 📉 Accuracy drops for low-quality/compressed images  
- 🔒 Currently only supports binary classification (AI vs Real)  

---

## 🎥 Project Demo  

<p align="center">  
  👉 <a href="https://drive.google.com/file/d/15yEsrw0r3ITI3dvTBIkoP1-EzVGpctJn/view?usp=sharing" target="_blank"><b>Watch the Demo Video</b></a> 👈  
</p>  

---

## 🔮 Future Scope  

- 🏷️ Source model identification (DALL·E, MidJourney, etc.)  
- 🎬 Support for AI-generated videos and text  
- 🔧 Model fine-tuning with user feedback  

---
