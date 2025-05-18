# 🧠 HippocampusSegmenation with Attention U-Net

This project leverages an Attention U-Net architecture to perform precise segmentation of the hippocampus in MRI images. The attention mechanism enhances the model's ability to focus on relevant regions, improving segmentation accuracy for structures like the hippocampus.


## 📊 Model Overview

The Attention U-Net model enhances the traditional U-Net by integrating attention gates (AGs) into the skip connections. These AGs enable the network to focus on pertinent regions of the input image, suppressing irrelevant features and improving segmentation performance. This approach is particularly beneficial for medical imaging tasks where the target structures vary in shape and size.

The concept is inspired by the paper: [Attention U-Net: Learning Where to Look for the Pancreas](https://arxiv.org/abs/1804.03999) by Oktay et al.

## 🧪 Dataset

The model is trained and evaluated on MRI scans with corresponding hippocampus segmentation labels. While the specific dataset isn't mentioned, commonly used datasets for such tasks include the Medical Segmentation Decathlon or the ADNI dataset. Ensure you have access to a suitable dataset and adjust the data loading and preprocessing steps in the notebook accordingly.

## 🚀 Getting Started

### Prerequisites

Ensure you have the following installed:

* Python 3.6 or higher
* Jupyter Notebook
* TensorFlow or PyTorch
* NumPy
* Matplotlib
* Scikit-learn

### Installation

1. Clone the repository:

   ```bash
   git clone https://github.com/angelinaghimire/HippocampusSegmenation.git
   cd HippocampusSegmenation
   ```

2. Install dependencies:

   ```bash
   pip install -r requirements.txt
   ```

   *Note: If `requirements.txt` is not provided, manually install the necessary packages.*

3. Run the notebook:

   ```bash
   jupyter notebook AttentionUnet_HippocampusSegmentation.ipynb
   ```

## 📈 Results

The notebook provides visualizations of the segmentation results, comparing the predicted masks against the ground truth. Evaluation metrics such as Dice coefficient and Intersection over Union (IoU) are used to assess model performance.

---

For more details, refer to the [Attention U-Net paper](https://arxiv.org/abs/1804.03999).
