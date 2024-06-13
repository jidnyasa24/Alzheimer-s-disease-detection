# Alzheimer-s-disease-detection

Early detection of Alzheimer's disease is essential for effective treatment and management. Traditional diagnostic methods are often time-consuming and prone to human error. There was a need for an automated, accurate, and efficient diagnostic tool for Alzheimer's disease using brain MRI images.

The objective was to develop a machine learning model capable of accurately classifying MRI scans into four categories: Non-Demented, Very Mild Demented, Mild Demented, and Moderate Demented. This required handling a complex dataset, designing a robust neural network architecture, and ensuring the model's performance and reliability.

1. Data Preparation:
   - Collected and preprocessed MRI images, including resizing to 224x224 pixels and normalizing pixel values.
   - Applied data augmentation techniques such as rotation, zoom, and flipping to enhance the training dataset and mitigate overfitting.

2. Model Development:
   - Utilized the VGG19 network pre-trained on ImageNet, with modifications for the specific task. The top layers of VGG19 were replaced with custom layers, including an Average Pooling layer, Dense layers, and Dropout layers to improve generalization.
   - Implemented the model using TensorFlow and Keras libraries.

3. Training and Evaluation:
   - Compiled the model with the Adam optimizer and categorical cross-entropy loss function.
   - Employed data augmentation for training and validation using ImageDataGenerator.
   - Trained the model with early stopping and checkpointing to save the best performing model.
   - Evaluated the model using accuracy, precision, recall, and F1-score, and generated confusion matrices and classification reports.

4. Visualization and Deployment:
   - Plotted training and validation accuracy and loss to visualize the model's learning curve.
   - Developed a Flask web application to allow users to upload MRI images for real-time prediction of Alzheimer's disease stages.

The project resulted in a highly accurate model for detecting Alzheimer's disease from MRI images, with strong performance across all evaluation metrics. The automated tool can aid in early diagnosis and treatment planning for Alzheimer's patients, significantly improving diagnostic efficiency and accuracy in clinical settings. The successful deployment of this model through a user-friendly web application provides a valuable resource for healthcare professionals.
