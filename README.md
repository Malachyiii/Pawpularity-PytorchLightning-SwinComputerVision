# Pawpularity-PytorchLightning-SwinComputerVision
This project contains different versions of the notebooks I submitted to the Kaggle [Pawpularity](https://www.kaggle.com/c/petfinder-pawpularity-score) competition. It utilizes Swin Transformer computervision models to predict pet cuteness scores from images.

# Highest Scoring Notebook (Silver Medal, Rank 126/3545, Private Leaderboard RMSE of 17.04)

My highest scoring notebook was based on a 12 model stratified K-Fold structure. 1/3 of the models were fit with mixup, 1/3 with cutmix, and 1/3 with neither. These 12 models than made predictions using test-time augmentation, and the average of the 12 models was the prediction. Though this notebook didn't score well on the public leaderboard, it proved to be highly generalizable when the private leaderboard was released, earning me a silver medal.

# Other Notebooks

## PyTorch Pawpularity

This file is meant to be run in Google Colab. It fits a 10-fold Swin-Small 224x224 image neural network to predict the pet's pawpularity score. It utilizes Weights and Biases to track performance, and saves the best fit model from each fold to your google drive.

## SwinSm-224x64-10Folds

This notebook is used to make predictions on a test set on Kaggle. It loads each model, makes predictions on the dataset, then takes the average of the 10 folds as the prediction.
