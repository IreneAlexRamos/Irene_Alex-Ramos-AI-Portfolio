# Gnasher Group: AI Dog Breed Group Finder

**Status:** Completed midterm proposal. Model implementation and measured evaluation are still in progress and are not presented here as finished results.

## Problem Statement

People often have difficulty identifying a dog's breed group, particularly when different breeds share similar visual features. This can limit the practical guidance available to pet owners, adopters, veterinary teams, and shelter professionals.

## Approach

Gnasher Group will accept a single dog photograph and predict one of the seven American Kennel Club groups: Sporting, Hound, Working, Terrier, Toy, Non-Sporting, or Herding. The application will return the predicted group and a confidence score.

The proposal defines the following technical plan:

- **Task:** multi-class image classification
- **Model:** EfficientNet-B0 with ImageNet transfer learning
- **Framework:** PyTorch and Torchvision
- **Environment:** Google Colab
- **Data:** Stanford Dogs, with 120 breed labels mapped to seven AKC groups
- **Planned subset:** approximately 7,000 balanced images, capped near 1,000 per group
- **Split:** 70% training, 15% validation, and 15% testing

## Results

The completed deliverable is the midterm proposal and implementation blueprint. It defines the problem, data mapping, model choice, evaluation targets, risks, and staged development plan. No model has been trained for this portfolio artifact, so no accuracy or inference-time result is claimed.

## Key Findings

- Transfer learning is a practical starting point for a limited course timeline.
- Mapping 120 breed labels to seven AKC groups requires careful, documented label preparation.
- Similar-looking breeds and class imbalance are likely to be the main technical challenges.
- Confidence scores and error analysis are important because visual appearance alone cannot confirm a dog's breed.

## Technologies Used

Planned stack: Python, PyTorch, Torchvision, EfficientNet-B0, Google Colab, transfer learning, data augmentation, and confusion-matrix analysis.

## Data

The proposed public data source is the [Stanford Dogs Dataset](http://vision.stanford.edu/aditya86/ImageNetDogs/), which will be downloaded during implementation rather than committed to this portfolio.

## Success Criteria

- At least 85% accuracy on unseen test images
- Average inference under one second per image on a Colab GPU
- Confusion-matrix analysis and review of three to five incorrect predictions

## Risks and Mitigations

- Similar-looking breeds may confuse the model; the interface can display the top two predictions and flag low confidence.
- Class imbalance may distort results; balancing, class weights, and augmentation are planned.
- The classifier predicts a group from visual appearance and is not a substitute for genetic testing or professional veterinary advice.

## Files

- [Gnasher-Group-Proposal.pdf](Gnasher-Group-Proposal.pdf)
- [Gnasher Group project repository](https://github.com/IreneAlexRamos/itai1378-project)

## How to Run

This portfolio folder contains the completed proposal, not a runnable model. Open the linked PDF to review the design. Dataset preparation, training, evaluation, and prediction instructions will be added to the separate project repository as each implementation milestone is completed.

## Next Steps

Prepare the label map and balanced subset, train the EfficientNet-B0 baseline, review the confusion matrix and incorrect predictions, then document the measured results without replacing the proposal's original scope.
