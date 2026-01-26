


# EmojiClusteringModel

An unsupervised machine learning project that clusters emoji images using CNN-based feature extraction and K-Means clustering.

## 🎯 Project Overview

This project uses a pre-trained MobileNetV2 convolutional neural network to extract visual features from 3,793 emoji images, then applies K-Means clustering to group similar emojis together.

## 📦 Dataset

The emoji images used in this project were sourced from the open-source
[emoji-data repository](https://github.com/iamcal/emoji-data) by iamcal.

Specifically, the **Apple-style emoji images** located in the
`img-apple-64` folder were used. The dataset consists of **3,793 PNG emoji images**,
each resized to 64×64 pixels.

All images are used for **educational and research purposes** in accordance
with the repository’s license.


## 🛠️ Technologies Used

- **Python 3.11**
- **TensorFlow 2.15.0** - For CNN feature extraction (MobileNetV2)
- **scikit-learn** - For K-Means clustering
- **NumPy** - For numerical operations
- **Matplotlib** - For visualization
- **PIL** - For image processing


## 📊 Methodology

1. **Data Collection**: 3,793 Apple-style emoji images (PNG format) sourced from the
   `img-apple-64` folder of the open-source emoji-data repository
2. **Feature Extraction**: Used pre-trained MobileNetV2 CNN to convert each emoji into a 1,280-dimensional feature vector
3. **Clustering**: Applied K-Means algorithm to group emojis into 10 clusters based on visual similarity"



## 👤 Author 

Ebonee Kent


