FOOD RECOGNITION AND CALORIE ESTIMATION MODEL

*OVERVIEW:

This repository contains code for a machine learning model developed to recognize food items from images and estimate their calorie content. The model enables users to track their dietary intake and make informed food choices.

*CODE EXPLANATION:

1.MODEL SELECTION
   The code utilizes ResNet50, a deep convolutional neural network (CNN) architecture pre-trained on the ImageNet dataset. ResNet50 is chosen for its powerful feature extraction capabilities.

2.IMAGE PREPROCESSING:
     Images are preprocessed before being fed into the model. This involves resizing them to 256x256 pixels, performing a center crop to 224x224 pixels (as required by ResNet50), converting them to PyTorch tensors, and normalizing pixel values.

3.PREDICTION PROCESS
     The model predicts the food item in the image and estimates its probabilities using softmax activation. The predicted label is then mapped to the appropriate food item from a predefined list of ImageNet labels.

4.LABEL RETRIEVAL
     A JSON file containing ImageNet labels is fetched from a remote URL. These labels are used for interpreting the model's predictions.

5.EXAMPLE USAGE
     An example image of an orange is provided in the code for demonstration purposes. The model predicts the label "orange" along with its associated probabilities.
