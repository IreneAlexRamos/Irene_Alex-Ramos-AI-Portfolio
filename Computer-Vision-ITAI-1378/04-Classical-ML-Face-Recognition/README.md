# Classical Machine Learning for Face Recognition

## Problem Statement

This project asks how well classical feature extractors and machine learning classifiers can identify people from a small face-image dataset, and how evaluation choices reveal overfitting.

## Approach

The notebook loads the Olivetti Faces dataset, splits 400 images into training (240), validation (80), and test (80) sets, and compares:

- Histogram of Oriented Gradients (HOG) for shape and edge information
- Local Binary Patterns (LBP) for texture information
- Support Vector Machines (SVM)
- Random Forest classifiers
- A deliberate overfitting demonstration and five-fold cross-validation exercise

## Results

| Model | Training accuracy | Validation accuracy | Gap |
| --- | ---: | ---: | ---: |
| SVM + HOG | 100.0% | **96.3%** | **3.7 points** |
| SVM + LBP | 57.1% | 41.2% | 15.8 points |
| Random Forest + HOG | 100.0% | 88.7% | 11.3 points |
| Random Forest + LBP | 100.0% | 38.8% | 61.3 points |

SVM + HOG was selected from the displayed validation results. A separate cross-validation exercise produced a mean score of 77.9% ± 7.5%, reinforcing that a single split can give an optimistic estimate. The notebook does not display a final held-out test score, so none is claimed here.

## Key Findings

- HOG captured more useful face structure than LBP in this experiment.
- Perfect training accuracy did not guarantee good generalization.
- The train/validation gap made severe Random Forest + LBP overfitting visible.
- Small datasets require cautious interpretation, cross-validation, and additional data before deployment.

## Technologies Used

Python, scikit-learn, scikit-image, NumPy, OpenCV, Matplotlib, and Seaborn.

## Data

The notebook loads Olivetti Faces through `sklearn.datasets.fetch_olivetti_faces()`. The public dataset is not committed to GitHub.

## File

- [Classical-ML-Face-Recognition.ipynb](Classical-ML-Face-Recognition.ipynb)

## How to Run

Open the notebook in Google Colab and run all cells. An internet connection is needed the first time scikit-learn downloads the dataset.
