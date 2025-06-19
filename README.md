

---

## 🧠 Brain Tumor Detection via Unsupervised Learning

📎 **Access the Project**:
[🔗 Click to Open in Google Colab](https://colab.research.google.com/drive/11R1bG-d_B-FABjwu0t3cWTWevYCk6DDX)

---

### 🔍 Project Overview

This project applies unsupervised learning to MRI brain scans for clustering and pattern analysis. By integrating **PCA** for dimensionality reduction and **K-Means clustering**, it groups MRI images by visual similarities—helpful in detecting anomalies like tumors without manual labeling.

---

## 💻 Project Demonstration

### ➤ Overview

Live demo using image clustering and visualization techniques.

### ➤ Demonstration Details

* **Image Preprocessing**: Grayscale conversion, resizing (128x128), and flattening.
* **PCA Compression**: Reduced feature dimensions from 16,384 to 50.
* **K-Means Clustering**: Segments MRI scans into 4 clusters.
* **Cluster Visualization**: 2D PCA visualization of clustered samples.
* **Silhouette Scores**: Quantitative performance measure of clustering.

---

## 📄 Project Documentation

### ➤ System Architecture

* Input: Unlabeled MRI scans from Training and Testing folders.
* Process: Load → Normalize → PCA → KMeans
* Output: Cluster label visualization, Silhouette Scores

### ➤ Code Modules

* `load_images`: Loads grayscale MRI images and labels.
* `plot_sample_images`: Displays random sample per class.
* `PCA`: Reduces high-dimensional image vectors.
* `KMeans`: Unsupervised classification into clusters.
* `plot_clusters`, `visualize_cluster_results`: Visualization.

### ➤ User Guide

* Upload MRI data to `/content/drive/MyDrive/dataset/Training` and `/Testing`.
* Update path in the script if needed.
* Run in [Google Colab](https://colab.research.google.com/drive/11R1bG-d_B-FABjwu0t3cWTWevYCk6DDX).

### ➤ Admin Guide

* Add more folders (e.g., Glioma, Meningioma).
* Adjust `NUM_CLUSTERS`, `IMG_SIZE`, and PCA components as needed.

### ➤ Testing Reports

* ✅ Successfully visualized clustered MRI images
* ✅ Silhouette Score \~0.5–0.6 shows moderate cluster quality
* ✅ Verified proper functioning of PCA & KMeans pipeline

---

## 🔁 Feedback and Final Adjustments

* **Feedback**: Evaluate clustering clarity on real data
* **Optimizations**:

  * Adjust PCA components for more detailed clusters
  * Tweak cluster count (k) based on use-case
* **Final Testing**:

  * Test system on additional MRI sets
  * Compare cluster assignments with actual tumor labels (optional)

---

## 📊 Final Project Report

### ➤ Summary

* MRI clustering using PCA + KMeans
* No labels required
* Visual output and numeric score-based validation

### ➤ Development Phases

1. Data preprocessing (resize, grayscale)
2. PCA transformation
3. KMeans clustering
4. Cluster visualization
5. Evaluation

### ➤ Challenges & Solutions

| Challenge                   | Solution                                      |
| --------------------------- | --------------------------------------------- |
| High-dimensional input      | PCA to 50 components                          |
| Non-uniform image sizes     | Resize to 128x128                             |
| Lack of ground truth labels | Used unsupervised learning + Silhouette Score |

---

## 🔧 Handover and Future Scope

* **Next Steps**:

  * Integrate Autoencoders for smarter compression
  * Add GUI or web interface
  * Test with labeled clinical MRI sets
* **Enhancements**:

  * Multi-modal MRI support (T1, FLAIR, etc.)
  * Label-based cluster validation

---

## ✅ Output Summary

| Feature              | Details                                                                                   |
| -------------------- | ----------------------------------------------------------------------------------------- |
| Input Size           | 128x128 grayscale                                                                         |
| Clustering Algorithm | KMeans (k=4)                                                                              |
| Compression          | PCA (50 components)                                                                       |
| Evaluation Metric    | Silhouette Score (\~0.5–0.6)                                                              |
| Tools Used           | OpenCV, PCA, scikit-learn, matplotlib                                                     |
| Runtime Environment  | [Google Colab](https://colab.research.google.com/drive/11R1bG-d_B-FABjwu0t3cWTWevYCk6DDX) |

---

