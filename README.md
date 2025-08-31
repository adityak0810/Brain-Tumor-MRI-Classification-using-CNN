# Brain-Tumor-MRI-Classification-using-CNN
A Multi-Class Brain Tumor Classifier using Convolutional Neural Network using Python and Pytorch Deep Learning Framework


# Dataset
The dataset used is the Brain Tumor MRI Dataset from Kaggle. It includes MRI images grouped into four categories:

Glioma: A type of tumor that occurs in the brain and spinal cord.
Meningioma: Usually benign tumors arising from the meninges (membranes covering the brain and spinal cord).
Pituitary Tumor: Tumors located in the pituitary gland at the base of the brain.
No Tumor: MRI images without any visible tumors.
The dataset is organized into 'Training' and 'Testing' directories, enabling a clear separation for model training and evaluation.

# Objective
The goal of this project is to develop a model that can accurately classify brain MRI images into one of the four categories, assisting in the early detection and diagnosis of brain tumors.

# Methodology
Data Preprocessing
Image Augmentation: To enhance the model's generalization, various techniques such as rotation, flipping, and zooming were applied to create a more robust dataset for training.
Normalization: All images were resized and normalized to ensure consistency in input dimensions and pixel scaling.
Data Splitting: Training and testing data were kept separate as provided in the dataset structure.
Model Architecture
A CNN-based architecture was used for image classification, with transfer learning approaches explored using architectures like EfficientNet and VGG16. Fine-tuning was also performed to achieve optimal accuracy.

# Training Strategy
Loss Function: Categorical Cross-Entropy
Metrics: F1-Score, Precision, Recall, and Accuracy
Evaluation: Training and validation loss and metrics were stored and plotted to visualize model performance across epochs.

# Results
The final model achieved a 96% accuracy on the test set, demonstrating its effectiveness in distinguishing between the four tumor categories. Additional metrics, including F1-Score, Precision, and Recall, further confirm the model’s reliability in accurately classifying MRI images.

# Conclusion
This brain tumor classification model represents a significant step toward automated diagnostics using deep learning, potentially supporting clinical decision-making and improving patient outcomes.
