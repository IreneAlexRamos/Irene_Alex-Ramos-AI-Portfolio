# Attribution and Data Sources

This portfolio includes coursework completed by Irene Alex Ramos for educational use. Several notebooks began with course or public tutorial templates; the completed exercises, experiments, saved outputs, and reflections document my learning.

## Course and Tutorial Materials

- The Chihuahua vs. Muffin workshop materials and example image dataset are based on the public [`patitimoner/workshop-chihuahua-vs-muffin`](https://github.com/patitimoner/workshop-chihuahua-vs-muffin) repository. The related portfolio notebooks preserve the original acknowledgments.
- Instructor-provided ITAI 1378 lab notebooks supplied the learning structure for image processing, classical machine learning, detection, and segmentation exercises.

## Datasets and Models

- **Olivetti Faces:** loaded through [`sklearn.datasets.fetch_olivetti_faces`](https://scikit-learn.org/stable/modules/generated/sklearn.datasets.fetch_olivetti_faces.html); the dataset itself is not stored in this repository.
- **COCO / COCO8 examples:** accessed through Ultralytics for classroom detection and fine-tuning exercises; the dataset is not stored in this repository.
- **Stanford Dogs Dataset:** planned data source for Gnasher Group, available from the [Stanford Dogs project page](http://vision.stanford.edu/aditya86/ImageNetDogs/); the dataset is not stored in this repository.
- **YOLO11 and SAM 2:** accessed through the [Ultralytics](https://docs.ultralytics.com/) Python package. Model weights are downloaded at runtime and are not committed.
- **PyTorch and Torchvision pretrained weights:** used for instructional experiments and the planned EfficientNet-B0 transfer-learning workflow.

## Portfolio Policy

Public datasets, downloaded model weights, generated training folders, and other large files are intentionally excluded. Each project README explains how its data is accessed.
