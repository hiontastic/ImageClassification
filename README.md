# ImageClassification Procedure Overview
                              Author: Yao Zhang
                              
## Description
This project aims to enhance the current weather detection mechanism by developing an optimal prediction model using deep learning Convolutional Neural Networks (CNN). It provides a complementary approach to traditional forecast models by incorporating live pictures of weather patterns to capture and classify upcoming weather swiftly. The model offers valuable and timely information about imminent weather changes, serving as an enhancement to the existing weather detection approach.

## Data Source
https://www.kaggle.com/datasets/somesh24/multiclass-images-for-weather-classification

## Base Model
VGG-16 with “GlobalAveragePooling2D” and “Dense” layers

## The Enhanced Model
VGG-16 with “GlobalAveragePooling2D” and “Dense” layers,  added by Data Augmentation, dropout rate, L2 regularization.

### Results overview

      Training and Validation Loss
![Training_and_Validation_loss](https://github.com/hiontastic/ImageClassification/assets/129336225/9c99123c-6c96-45d5-a861-03a483fa191e)
      
      
      Training, Testing and Validation Accuracy
![Training_validation_testing_accuracy](https://github.com/hiontastic/ImageClassification/assets/129336225/aa572ab3-7e54-4570-a34e-4a74ac550048)


## Model Selection Criteria
1. Model accuraccy
2. Model's ability to generalize on unseen data, i.e. no serious overfitting nor underfitting problems present
3. Computation Resources Efficient

Thus, a hyperparameter tuning is conducted to determine the optimal hyperparameters seeking for the best performance model.  

## The Optimal Model
VGG-16 with “GlobalAveragePooling2D” and “Dense” layers, with optimal regularizations/ hyperparameters epoch=30, batch size=16, dropout_rate=0.3, L2 regularization value=0.001, along with Data Augmentation aiming to provide additional training examples to address the overfitting problems.

## Model Structure
![optimalVGG16](https://github.com/hiontastic/ImageClassification/assets/129336225/6dc33034-3109-4046-9d3f-b5a4d188d555)

## Final Model's Accuracy=93.78%

