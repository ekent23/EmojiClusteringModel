# EmojiClusteringModel

An unsupervised machine learning project that compares vision-based and text-based AI clustering of emojis against human perceptual groupings.

## 🎯 Project Overview

This project investigates whether AI clusters emojis the way humans do. Using 3,793 Apple emojis, two unsupervised clustering models were compared — one vision-based and one text-based — against human card-sort data collected through a custom web interface. Results were evaluated using pairwise F1 scores.

This research was completed as part of the NASA Delaware Space Grant Consortium internship at Delaware State University under the mentorship of Dr. Kong.

## 📦 Dataset

The emoji images used in this project were sourced from the open-source [emoji-data repository](https://github.com/iamcal/emoji-data) by iamcal.

Specifically, the **Apple-style emoji images** located in the `img-apple-64` folder were used. The dataset consists of **3,793 PNG emoji images**, each resized to 64×64 pixels.

All images are used for **educational and research purposes** in accordance with the repository's license.

## 🛠️ Technologies Used

- **Python 3.11**
- **TensorFlow / Keras** – For CNN feature extraction (EfficientNetB3)
- **SentenceTransformers (all-MiniLM-L6-v2)** – For semantic text embedding
- **scikit-learn** – For K-Means clustering and Silhouette Method
- **NumPy** – For numerical operations
- **Matplotlib** – For visualization
- **Pillow (PIL)** – For image processing

## 📊 Methodology

1. **Vision Extraction**: EfficientNetB3 converts each emoji image into a 1,536-dimensional feature vector capturing visual characteristics like color, shape, and texture.
2. **Text Extraction**: SentenceTransformer (all-MiniLM-L6-v2) converts each emoji's name into a 384-dimensional semantic vector, where similar meanings are close together in vector space.
3. **Clustering**: K-Means clustering is applied to both feature sets. The Silhouette Method was used to find the optimal number of clusters — 48 for vision, 43 for text.
4. **Human Baseline**: A custom web interface presented 60 random emojis to participants for manual grouping (card-sort study).
5. **Evaluation**: Pairwise F1 scores measure agreement between each AI model's groupings and the human groupings.

## 📈 Results

| Model | Average F1 Score |
|---|---|
| Vision (EfficientNetB3) | 0.275 |
| Text (SentenceTransformer) | 0.416 |
| **Improvement** | **+51%** |

The text-based model significantly outperformed the vision model, indicating that humans categorize emojis based on semantic meaning rather than visual appearance.

## 👤 Author

**Ebonee Kent**  
Junior, Information Technology — Delaware State University  
NASA Delaware Space Grant Consortium Research Intern

## 🙏 Acknowledgements

This research was supported by the Delaware Space Grant College and Fellowship Program (NASA Grant 80NSSC20M0045). Thanks to Delaware State University for computational resources and to all card-sort study participants.

