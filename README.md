# 🖋️ Handwriting Signature Verification using Siamese Networks

This project implements a **Siamese Neural Network** to distinguish between genuine and forged handwritten signatures. It leverages deep learning techniques to build a robust signature verification system, suitable for applications in identity validation and forgery detection.

---

## 🚀 Features

* **📁 Dataset Handling**: Downloads and organizes signature image datasets from *KaggleHub*.
* **🔍 Data Exploration**: Examines and visualizes the directory structure (real vs. forged).
* **🔗 Pair Generation**: Creates positive (genuine-genuine) and negative (genuine-forged) image pairs for training.
* **🖼️ Image Preprocessing**: Loads, resizes, grayscales, and normalizes signature images.
* **📈 Data Augmentation**: Enhances dataset with techniques like:

  * Rotation
  * Width/height shifting
  * Shearing
  * Zooming
  * Brightness adjustment
  * Horizontal flipping
* **🧠 Siamese Network Architecture**: Uses a custom CNN encoder with twin networks to learn image similarity.
* **📉 Contrastive Loss**: Trains with a custom contrastive loss function to separate similar/dissimilar pairs in embedding space.
* **🔄 Batch Generation**: Efficiently batches image pairs with corresponding labels.
* **📊 Model Training**: Includes:

  * EarlyStopping
  * ReduceLROnPlateau
* **📉 Performance Visualization**: Plots training loss and accuracy for analysis.

---

## 🛠️ Technologies Used

* **Python 3**
* **TensorFlow / Keras** – Deep learning framework
* **OpenCV (`cv2`)** – Image preprocessing
* **NumPy** – Numerical operations
* **Matplotlib** – Visualizations
* **KaggleHub** – Dataset downloader

---

## 📚 Dataset

* **Name**: *Handwriting Signature Datasets*
* **Source**: [KaggleHub]([https://www.kaggle.com/datasets](https://www.kaggle.com/datasets/mostafaeltalawy/handwriting-signature))
* **Description**: Real and forged signature images categorized by signer identity.

---

## 📦 Installation & Usage

### 1. Install Requirements

```bash
pip install tensorflow opencv-python numpy matplotlib kagglehub
```

### 2. Run the Notebook

* Download and open `DSAI_308_Final_Project_DS2.ipynb` in Jupyter Notebook or JupyterLab.
* Run each cell sequentially.

> 💡 **Note**: If you're running outside Kaggle, you'll need to authenticate with the Kaggle API. Place your `kaggle.json` in the correct directory or authenticate manually.

---

## 📈 Sample Output

* Visualized pairings (genuine vs. forged)
* Siamese network loss curve
* Accuracy plots showing training progress

