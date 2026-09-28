# Neural Network Image Classifier: Chihuahua vs. Muffin

## Problem Statement

Chihuahua faces and muffin tops can share similar colors, edges, and textures. This workshop uses the intentionally difficult pair to test the limitations of a fully connected neural network on image data.

## Approach

Images are resized to 224 × 224, converted to tensors, normalized, and flattened before entering a PyTorch multilayer perceptron. The notebook trains the model, tracks loss and accuracy, visualizes predictions, experiments with hyperparameters, and makes an initial comparison with convolutional layers.

## Results

- Baseline model after three epochs: 60.0% validation accuracy
- Ten-epoch dense-network experiment: 56.7% validation accuracy
- Small convolutional improvement experiment: 63.3% validation accuracy

Predictions often stayed close to 50/50 confidence, illustrating why flattening an image discards valuable spatial relationships.

## Key Findings

- Adding dense layers does not solve the loss of image structure caused by flattening.
- Confidence scores provide useful diagnostic evidence beyond a single accuracy number.
- Convolutional layers are a more appropriate architecture for learning edges, textures, and shapes.

## Technologies Used

Python, PyTorch, Torchvision, Pillow, Matplotlib, and Google Colab.

## Data

The tutorial dataset contains 120 training images and 30 validation images. It is downloaded at runtime from the credited public Chihuahua vs. Muffin workshop repository and is not duplicated here.

## Files

- [MLP-Chihuahua-vs-Muffin.ipynb](MLP-Chihuahua-vs-Muffin.ipynb)
- [MLP-Classifier-Reflection.pdf](MLP-Classifier-Reflection.pdf)

## How to Run

Open the notebook in Google Colab and run all cells. The notebook downloads the workshop resources and creates its data loaders during execution.
