# Image Classification Hackathon: Identifying Icon Types in Datasets
## Description
Participated in an image classification competition hosted by Dacon, where the task was to classify different types of icons in a dataset using machine learning and computer vision techniques. The challenge involved working with a variety of icon types and required the use of advanced deep learning techniques to achieve high classification accuracy. The competition aimed to develop AI algorithms for automatic icon classification, which can innovate various fields such as image search enhancement, UI design improvement, and digital document auto-tagging.

Competition Details: Dacon Image Classification Hackathon

Technologies Used
Python

PyTorch

Convolutional Neural Networks (CNNs)

Residual Blocks

Inception Blocks

Batch Normalization

## Model Architecture
The model architecture utilized a combination of CNN layers, residual blocks, and inception blocks, with batch normalization and dropout for regularization. The model's final layers included a fully connected (FC) layer and output layer for classifying the icons into 10 distinct categories.

Data Preprocessing and Loading
Data Loading: The data was loaded from train.csv and test.csv files.

Data Splitting: The training data was split into training and validation sets using train_test_split, ensuring stratification by label to maintain class balance.

Optimization and Learning Rate Scheduler
Optimizer: The Adam optimization algorithm was used to update the model's parameters.

Learning Rate Scheduler: A ReduceLROnPlateau scheduler was employed to adjust the learning rate, ensuring optimal performance by reducing the learning rate when the loss plateaus.

Early Stopping and Evaluation
Early Stopping: Training was halted when the validation accuracy stopped improving, preventing unnecessary overfitting.

Evaluation Metrics: The model's performance was evaluated based on training accuracy and validation accuracy.

Training & Performance
Epochs: 30

Training Accuracy: 100%

Validation Accuracy: 92.86%

Loss at Epoch 15: 0.0005

Batch Size: 16

Early Stopping: Triggered after achieving the highest validation accuracy

## Note: The model showed excellent performance during training but exhibited signs of overfitting, as evidenced by the high training accuracy (100%) compared to the validation accuracy (92.86%).

## Improvements & Future Updates
Despite the excellent performance during training, the model exhibited signs of overfitting due to the high training accuracy (100%) compared to the validation accuracy (92.86%). To address this, the following strategies will be implemented to improve generalization:

Data Augmentation: Although data augmentation techniques (e.g., random rotations, flips) could not be applied due to competition rules prohibiting the use of external data, these methods will be explored in future projects to enhance model generalization.

L2 Regularization: This will be used to prevent the model from assigning too much importance to specific features, thus aiding in generalization.

Model Architecture Optimization: The model's architecture will be re-examined to explore potential improvements in generalization performance.

These strategies aim to enhance both training and validation performance in future iterations.

## Conclusion
The model performed well but will undergo further optimization to handle overfitting and improve its ability to generalize to unseen data. The applied improvements, including dropout, data augmentation, regularization, and adjusted learning rates, are expected to enhance both training and validation performance in future iterations.
