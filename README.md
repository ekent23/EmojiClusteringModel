


# EmojiClusteringModel

An unsupervised machine learning project that clusters emoji images using CNN-based feature extraction and K-Means clustering.

## 🎯 Project Overview

This project uses a pre-trained MobileNetV2 convolutional neural network to extract visual features from 3,793 emoji images. It then applies K-Means clustering to group visually similar emojis together, making it easier to explore patterns in emoji usage and design.

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
- **TensorFlow 2.15.0** – For CNN feature extraction (MobileNetV2)
- **scikit-learn** – For K-Means clustering
- **NumPy** – For numerical operations
- **Matplotlib** – For visualization
- **Pillow (PIL)** – For image processing


## 📊 Methodology

1. **Data Collection**: 3,793 Apple-style emoji images (PNG format) sourced from the
   `img-apple-64` folder of the open-source emoji-data repository
2. **Feature Extraction**: Each emoji is converted into a 1,280-dimensional feature vector using the pre-trained MobileNetV2 CNN (without the classifier feature).
3. **Clustering**: The K-Means algorithm is applied to group emojis based on visual similarity. The project uses 50 clusters by default, but this can be adjusted.
4. **Visualization**: Random emojis from each cluster are displayed in a grid, and the final figure is saved as results.png.

## Example Output


![alt text](https://github.com/ekent23/EmojiClusteringModel/edit/main/results.png)results.png "Results")


## 👤 Author 

Ebonee Kent


