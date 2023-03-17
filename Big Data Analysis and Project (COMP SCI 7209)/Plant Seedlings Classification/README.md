# Plant Seedlings Classification

This project aimed to build a prediction model which is capable to classify the species of a plant from a photo. Near 5,000 images of plants belonging to 12 species were provided as training data. The images were preprocessed with Gaussian Blur and color mask before feeding into the models. Six Convolutional Neural Network models were selected and trained to perform the task. 

1. A CNN model built from scratch 
2. VGG16
3. ResNet50
4. Inception-v3
5. Xception 
6. EfficientNetB0
 
The above models were trained with un-augmented images and augmented images. Model (2)-(5) were fine-tuned after trained with augmented images. Model (1)-(5) suffered from over-fitting, while model (6) had a fair performance. 

## Data

The dataset is available at Kaggle (https://www.kaggle.com/competitions/plant-seedlings-classification/data). Gaussian Blur and HSV color space masks were applied to the images to isolate the plants in the photos to aim for better outcome.

## Results

Training and validation accuracy and loss were plotted for each model, and confusion matrix was used to visualize the performance of model (6).
