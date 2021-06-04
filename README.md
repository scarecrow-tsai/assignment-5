# Assignment 5

The code drill down consists of 4 steps. In the first step we setup our train/test workflow. In the second step we reduce the number parameters of our model and try to maintain a high accuracy. In the third step we add regularization to the model to further boost the accuracy. Finally, we change the model definition, to increase capacity, once the test accuracy maxes out after the above 3 stages.

## 1. Setup

### Target

- Code a basic skeleton and establish a train/test workflow.
- Set base transforms.
- Create Dataset and Dataloaders.
- Write train and test loops.
- Get a baseline score.

### Results

- Parameters: `6,379,786`
- Best Train Accuracy: `99.945%`
- Best Test Accuracy: `99.29%`

### Analysis

- The model is huge for the mnist dataset.
- The model is overfitting.

## 2. Lighter Model

### Target

- Aggresively reduce number of parameters to under 10,000 while maintaining a similar accuracy.

### Results

- Parameters: `7,931`
- Best Train Accuracy: `98.02%`
- Best Test Accuracy: `98.06%`

### Analysis

- Slight underfitting.
- Model can be made better by adding regularization.

## 3. Regularization

### Target

- Add dropout.
- Add batchnorm.
- Add data augmentation.

### Results

- Parameters: `7,931`
- Best Train Accuracy: `98.99%`
- Best Test Accuracy: `98.79%`

### Analysis

- Slight overfitting.
- Can do better if we increase capacity.

## 4. Optimizer and Architecture

### Target

- Add more layers.
- Learning rate scheduler.

### Results

- Parameters: `9,933`
- Best Train Accuracy: `99.28%`
- Best Test Accuracy: `99.35%`

### Analysis

- More layers increase capacity and therefore the accuracy.
- Learning rate scheduler helps find a better minima.
