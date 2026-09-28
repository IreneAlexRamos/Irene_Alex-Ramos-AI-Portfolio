# Irene Alex Ramos | Applied AI Portfolio

## About Me

I am an Applied AI and Robotics student at Houston Community College with a growing focus on computer vision, machine learning, and robotics. My background in veterinary care and physical security shapes the problems I am most interested in solving: practical systems that can interpret visual information, support people, and operate responsibly in the real world.

This repository presents completed coursework, runnable Jupyter notebooks, documented results, and projects in progress.

## Technical Skills

- **Programming and workflow:** Python, Jupyter Notebook, Google Colab, Git, GitHub
- **Machine learning:** supervised learning, feature engineering, train/validation/test splits, cross-validation, overfitting analysis, model evaluation
- **Computer vision:** image processing, HOG, LBP, CNNs, object detection, instance segmentation
- **Libraries and frameworks:** PyTorch, Torchvision, OpenCV, NumPy, scikit-learn, scikit-image, Pillow, Matplotlib, Ultralytics
- **Models and tools:** EfficientNet-B0, YOLO11, SAM 2

## Featured Work

| Project | What I did | Selected result |
| --- | --- | --- |
| [CNN: Chihuahua vs. Muffin](Computer-Vision-ITAI-1378/06-CNN-Chihuahua-vs-Muffin/) | Built and evaluated a PyTorch convolutional neural network on a difficult two-class image task | 90.0% final validation accuracy; 100% peak accuracy on the small validation set |
| [Classical ML Face Recognition](Computer-Vision-ITAI-1378/04-Classical-ML-Face-Recognition/) | Compared HOG and LBP features with SVM and Random Forest classifiers | SVM + HOG reached 96.3% validation accuracy with the smallest observed generalization gap |
| [Object Detection and Segmentation](Computer-Vision-ITAI-1378/07-Object-Detection-and-Segmentation/) | Used YOLO11 and SAM 2 for detection and segmentation, then explored evaluation and fine-tuning | COCO8 learning exercise reached 0.844 mAP50 after five epochs |
| [Gnasher Group](Computer-Vision-ITAI-1378/08-Gnasher-Group-Midterm/) | Designed an EfficientNet-B0 transfer-learning application that predicts a dog's AKC group | Midterm blueprint and implementation plan in progress |

> Metrics are reported from the saved notebook outputs. Small classroom datasets are useful for learning, but these results should not be interpreted as production benchmarks.

## Courses

### [Computer Vision and AI — ITAI 1378](Computer-Vision-ITAI-1378/)

Coursework covers digital images, color models, OpenCV processing, classical feature extraction, supervised machine learning, convolutional neural networks, object detection, image segmentation, and responsible evaluation. The course folder contains every completed artifact supplied for this portfolio, including the original `.ipynb` notebooks with visible outputs.

Additional courses and projects will be added as the Applied AI and Robotics program continues.

## Running the Notebooks

The notebooks were completed in Google Colab and retain their saved outputs.

1. Open a project folder and select its `.ipynb` file.
2. Download the notebook or open it in Google Colab.
3. In Colab, select **Runtime → Run all**.
4. Follow any notebook-specific data instructions in that project's README.

For a local environment, use Python 3.10+ and install the shared dependencies:

```bash
python -m pip install -r requirements.txt
jupyter notebook
```

Some notebooks use Colab-specific helpers or download model weights at runtime, so Colab is the recommended environment.

## Contact

- GitHub: [github.com/IreneAlexRamos](https://github.com/IreneAlexRamos)

<!-- Before final submission, add a professional email address and LinkedIn URL here. -->

## Attribution

Several assignments began with instructor- or tutorial-provided lab templates and were completed with my code, experiments, outputs, and written reflections. Dataset, framework, and tutorial credits are listed in [ATTRIBUTION.md](ATTRIBUTION.md) and in the notebooks themselves.
