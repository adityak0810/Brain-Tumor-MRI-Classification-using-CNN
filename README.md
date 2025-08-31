
# Brain Tumor MRI Classification using CNN

A multi-class brain tumor classifier using a Convolutional Neural Network (CNN) with the PyTorch deep learning framework. This project aims to accurately classify brain MRI images into four categories: glioma, meningioma, pituitary tumor, and no tumor.

## About The Project

This project focuses on the development of a deep learning model for the classification of brain tumors from MRI scans. Early and accurate diagnosis of brain tumors is crucial for effective treatment planning and improving patient outcomes. By leveraging the power of Convolutional Neural Networks, this project provides an automated and reliable solution for distinguishing between different types of brain tumors and identifying healthy brain scans.

## Dataset

The dataset used in this project is the [Brain Tumor MRI Dataset](https://www.kaggle.com/datasets/masoudnickparvar/brain-tumor-mri-dataset) from Kaggle. It contains MRI images categorized into four classes:

  * **Glioma:** A common type of tumor that originates in the glial cells of the brain or spinal cord.
  * **Meningioma:** Tumors that arise from the meninges, the membranes that surround the brain and spinal cord.
  * **Pituitary Tumor:** Tumors that develop in the pituitary gland, a small gland at the base of the brain.
  * **No Tumor:** MRI images of healthy brains without any signs of tumors.

The dataset is pre-divided into `Training` and `Testing` sets, which simplifies the process of training and evaluating the model.

## Methodology

The project follows a systematic approach to building and evaluating the brain tumor classification model:

1.  **Data Preprocessing:**

      * **Image Augmentation:** To prevent overfitting and improve the model's ability to generalize, various data augmentation techniques were applied. These include random rotations, horizontal flips, and resized crops.
      * **Normalization:** All images were resized to a consistent dimension and normalized to ensure that the pixel values have a similar scale.

2.  **Model Architecture:**

      * A Convolutional Neural Network (CNN) was designed and implemented using PyTorch.
      * Transfer learning with pre-trained models like **EfficientNet** and **VGG16** was explored to leverage the features learned from large-scale image datasets. The models were fine-tuned on the brain tumor dataset to achieve optimal performance.

3.  **Training and Evaluation:**

      * **Loss Function:** Categorical Cross-Entropy was used as the loss function, which is suitable for multi-class classification problems.
      * **Optimizer:** The Adam optimizer was used to update the model's weights during training.
      * **Metrics:** The model's performance was evaluated using the following metrics:
          * Accuracy
          * F1-Score
          * Precision
          * Recall

## Results

The final model achieved an impressive **96% accuracy** on the test set, demonstrating its effectiveness in accurately classifying brain tumor MRI images.

