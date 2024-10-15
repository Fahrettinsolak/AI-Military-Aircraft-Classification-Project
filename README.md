# Military Aircraft Image Classification Project Using Custom DataSet (With Transfer Learning)

This project focuses on classifying military aircraft images using **Transfer Learning** with the **VGG16** model. The dataset utilized is a custom collection derived from the [MTARSI](https://zenodo.org/record/3464319#.YUiSrrgzaUk) dataset, containing five classes of military aircraft.

## Project Overview

The goal of this project is to accurately classify images of military aircraft by leveraging the pre-trained VGG16 model. We fine-tuned the model to work specifically with our dataset, which contains images of five different aircraft types.

### Dataset Information
The dataset consists of:
- **Training set**: 1812 images spread across 5 classes.
- **Testing set**: 100 images for model evaluation.

Each image is resized to 224x224 pixels to fit the input requirements of the VGG16 model.

### Model Architecture
We used **VGG16**, a popular deep learning model, pre-trained on the ImageNet dataset. The model was fine-tuned by replacing the final output layer to adapt it to the 5 classes in our dataset. All other layers of VGG16 were frozen to preserve the pre-trained weights.

### Prediction Process
After training, the model can predict the type of aircraft in new images. The input images are preprocessed to match the VGG16 input format, and the model outputs a predicted class with a confidence score.

### Results
The model achieved a validation accuracy of approximately **87%** on unseen test data. The fine-tuned VGG16 model performed well across all classes, demonstrating the power of Transfer Learning in image classification tasks. 

## Conclusion
This project illustrates the effectiveness of using **Transfer Learning** with the **VGG16** model for classifying military aircraft images. The model achieves high accuracy and can be further improved by fine-tuning more layers or expanding the dataset. This approach highlights the value of leveraging pre-trained models for specialized tasks with limited data.

## How to Run the Project
1. Prepare the dataset by organizing the images into training and testing directories.
2. Install the necessary dependencies such as TensorFlow and Keras.
3. Train the model using the provided dataset.
4. Use the trained model to classify new images of military aircraft.

## Requirements
- TensorFlow
- Keras
- NumPy
- PIL (Python Imaging Library)


