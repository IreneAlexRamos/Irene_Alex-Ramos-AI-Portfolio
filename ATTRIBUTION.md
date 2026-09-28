# Attribution and Data Sources

This portfolio includes coursework completed by Irene Alex Ramos for educational use. Several notebooks began with course or public tutorial templates; the completed exercises, experiments, saved outputs, and reflections document my learning.

## Course and Tutorial Materials

- The Chihuahua vs. Muffin workshop materials and example image dataset are based on the public [`patitimoner/workshop-chihuahua-vs-muffin`](https://github.com/patitimoner/workshop-chihuahua-vs-muffin) repository. The related portfolio notebooks preserve the original acknowledgments.
- Instructor-provided ITAI 1378 lab notebooks supplied the learning structure for image processing, classical machine learning, detection, and segmentation exercises.
- The image-processing notebook can retrieve the public [Vd-Orig sample image from Wikimedia Commons](https://commons.wikimedia.org/wiki/File:Vd-Orig.png); its saved run uses the notebook's generated fallback test pattern.

## Datasets and Models

- **Olivetti Faces:** loaded through [`sklearn.datasets.fetch_olivetti_faces`](https://scikit-learn.org/stable/modules/generated/sklearn.datasets.fetch_olivetti_faces.html); the dataset itself is not stored in this repository.
- **COCO / COCO8 examples:** accessed through the official [Ultralytics COCO8 documentation](https://docs.ultralytics.com/datasets/detect/coco8/) for classroom detection and fine-tuning exercises; the dataset is not stored in this repository.
- **Stanford Dogs Dataset:** planned data source for Gnasher Group, available from the [Stanford Dogs project page](http://vision.stanford.edu/aditya86/ImageNetDogs/); the dataset is not stored in this repository.
- **YOLO11 and SAM 2:** accessed through the [Ultralytics YOLO11 documentation](https://docs.ultralytics.com/models/yolo11/) and Python package. Model weights are downloaded at runtime and are not committed.
- **PyTorch and Torchvision pretrained weights:** used for instructional experiments and the planned EfficientNet-B0 transfer-learning workflow.

## Portfolio Policy

Public datasets, downloaded model weights, generated training folders, and other large files are intentionally excluded. Each project README explains how its data is accessed.

Images in project `results/` folders are exports of outputs already saved in the corresponding notebooks. They use the same credited data and sample images listed above.
