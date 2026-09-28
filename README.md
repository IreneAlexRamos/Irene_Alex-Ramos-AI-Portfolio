# Irene Alex Ramos | Applied AI & Robotics Portfolio

*Building practical AI with roots in animal care, security, and real-world problem solving.*

## Hi, I'm Alex

I'm an Applied AI and Robotics student at Houston Community College with a growing focus on computer vision, machine learning, and robotics.

My path into technology has not been completely traditional. Before focusing on AI, I worked in veterinary care and physical security. Those experiences still shape the kinds of problems I want to solve. I am especially interested in technology that can help animals, improve safety, support people, and work responsibly in the real world.

This portfolio follows what I am learning as I build those skills. It includes completed coursework, runnable Jupyter notebooks, honest reflections, documented results, and projects that are still growing. I do not expect every experiment to be perfect—the mistakes, unexpected results, and improvements are part of the story too.

## What I'm Working Toward

My goal is to build a career that combines AI, computer vision, and eventually robotics. I enjoy taking a problem from an idea to a working experiment, comparing approaches, and figuring out why a model behaves the way it does. Over time, I want to apply those skills to animal care, safety, and other problems that matter outside of the classroom.

## Featured Work

| Project | What I did | Selected result |
| --- | --- | --- |
| [CNN: Chihuahua vs. Muffin](Computer-Vision-ITAI-1378/06-CNN-Chihuahua-vs-Muffin/) | Built and evaluated a PyTorch convolutional neural network on a difficult two-class image task | 90.0% final validation accuracy; 100% peak accuracy on the small validation set |
| [Classical ML Face Recognition](Computer-Vision-ITAI-1378/04-Classical-ML-Face-Recognition/) | Compared HOG and LBP features with SVM and Random Forest classifiers | SVM + HOG reached 96.3% validation accuracy with the smallest observed generalization gap |
| [Object Detection and Segmentation](Computer-Vision-ITAI-1378/07-Object-Detection-and-Segmentation/) | Used YOLO11 and SAM 2 for detection and segmentation, then explored evaluation and fine-tuning | COCO8 learning exercise reached 0.844 mAP50 after five epochs |
| [Gnasher Group](Computer-Vision-ITAI-1378/08-Gnasher-Group-Midterm/) | Designed an EfficientNet-B0 transfer-learning application that predicts a dog's AKC group | Midterm blueprint and implementation plan in progress |

> Metrics are reported from the saved notebook outputs. Small classroom datasets are useful for learning, but these results should not be interpreted as production benchmarks.

## What These Projects Taught Me

- **A better model starts with understanding the problem.** My first dense neural-network experiments on Chihuahua-versus-muffin images reached only about 57–60% validation accuracy. Moving to a CNN made the importance of spatial image features much more concrete and improved the final validation result to 90%.
- **The most complicated approach is not always the best one.** In the classical face-recognition exercise, SVM with HOG features produced the strongest validation result and the smallest observed generalization gap among the tested combinations.
- **Metrics need context.** Small datasets can be useful for testing a pipeline, but high scores on them do not automatically mean a model is ready for the real world. Learning to question results has become just as important to me as improving them.
- **Computer vision involves trade-offs.** Detection and segmentation work helped me see how confidence thresholds, recall, precision, speed, and the cost of missed hazards affect real safety decisions.

## Currently Building: Gnasher Group

Gnasher Group is the project that connects most directly to my veterinary-care background. The goal is to take a dog image and predict its American Kennel Club group using transfer learning. The idea grew from seeing how easily similar-looking breeds can be confused and wanting to explore how computer vision might organize visual information in a useful way.

The current portfolio includes the project blueprint and implementation plan. My next steps are to prepare the dataset, train the first model, evaluate where it struggles, and turn the plan into a working prototype.

## Technical Skills

- **Programming and workflow:** Python, Jupyter Notebook, Google Colab, Git, GitHub
- **Machine learning:** supervised learning, feature engineering, train/validation/test splits, cross-validation, overfitting analysis, model evaluation
- **Computer vision:** image processing, HOG, LBP, CNNs, object detection, instance segmentation
- **Libraries and frameworks:** PyTorch, Torchvision, OpenCV, NumPy, scikit-learn, scikit-image, Pillow, Matplotlib, Ultralytics
- **Models and tools:** EfficientNet-B0, YOLO11, SAM 2

## Coursework

### [Computer Vision and AI — ITAI 1378](Computer-Vision-ITAI-1378/)

This course took me from the basic structure of digital images through color models, OpenCV processing, classical feature extraction, supervised machine learning, convolutional neural networks, object detection, image segmentation, and responsible evaluation.

The course folder contains every completed artifact included in this portfolio, including the original `.ipynb` notebooks with their saved outputs. Additional courses and projects will be added as I continue through the Applied AI and Robotics program.

## Running the Notebooks

I completed these notebooks in Google Colab and kept their saved outputs so the results can be reviewed without rerunning every experiment.

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
