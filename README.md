# Music_Genre_Classification_Through_Deep_Learning

This project focuses on building a **music genre classification system** using the **GTZAN dataset**. The task is to classify 10 different music genres based on audio spectrograms using deep learning models.

## 📁 Dataset

We used the **GTZAN dataset**, which contains:
- 10 genres (`blues`, `classical`, `country`, `disco`, `hiphop`, `jazz`, `metal`, `pop`, `reggae`, `rock`)
- 100 audio files per genre (total: 1000 samples)
- Each audio file: 30 seconds long, sampled at 22,050 Hz

The dataset was converted into spectrogram images for training.

## 🧠 Models Used

Three different deep learning models were implemented and compared:

### 1️⃣ Custom CNN
- A convolutional neural network built from scratch
- Consists of convolutional, pooling, and dense layers
- Lightweight and fast

### 2️⃣ VGG16 (Transfer Learning)
- Pretrained on ImageNet
- Last layers fine-tuned for classification
- Good performance with deeper feature extraction

### 3️⃣ ResNet18 (Transfer Learning)
- Pretrained on ImageNet
- Skip connections help with vanishing gradient
- Balanced depth and performance