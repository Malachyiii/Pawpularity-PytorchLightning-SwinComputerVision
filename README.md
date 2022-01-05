# Pawpularity-PytorchLightning-SwinComputerVision
This project is my entrance to the Kaggle [Pawpularity](https://www.kaggle.com/c/petfinder-pawpularity-score) competition. It utilizes Pytorch Lightning to fit a 10-Fold Swin Transformer computervision model to predict pet cuteness scores from images.

## PyTorch Pawpularity

This file is meant to be run in Google Colab. It fits a 10-fold Swin-Small 224x224 image neural network to predict the pet's pawpularity score. It utilizes Weights and Biases to track performance, and saves the best fit model from each fold to your google drive.

## SwinSm-224x64-10Folds

This notebook is used to make predictions on a test set on Kaggle. It loads each model, makes predictions on the dataset, then takes the average of the 10 folds as the prediction.
