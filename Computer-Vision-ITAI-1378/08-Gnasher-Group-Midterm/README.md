# Gnasher Group: AI Dog Breed Group Finder

## Problem Statement

People often have difficulty identifying a dog's breed group, particularly when different breeds share similar visual features. This can limit the practical guidance available to pet owners, adopters, veterinary teams, and shelter professionals.

## Proposed Solution

Gnasher Group will accept a single dog photograph and predict one of the seven American Kennel Club groups: Sporting, Hound, Working, Terrier, Toy, Non-Sporting, or Herding. The application will return the predicted group and a confidence score.

## Technical Approach

- **Task:** multi-class image classification
- **Model:** EfficientNet-B0 with ImageNet transfer learning
- **Framework:** PyTorch and Torchvision
- **Environment:** Google Colab
- **Data:** Stanford Dogs, with 120 breed labels mapped to seven AKC groups
- **Planned subset:** approximately 7,000 balanced images, capped near 1,000 per group
- **Split:** 70% training, 15% validation, and 15% testing

## Success Criteria

- At least 85% accuracy on unseen test images
- Average inference under one second per image on a Colab GPU
- Confusion-matrix analysis and review of three to five incorrect predictions

## Risks and Mitigations

- Similar-looking breeds may confuse the model; the interface can display the top two predictions and flag low confidence.
- Class imbalance may distort results; balancing, class weights, and augmentation are planned.
- The classifier predicts a group from visual appearance and is not a substitute for genetic testing or professional veterinary advice.

## Current Status

The project is in the blueprint stage. This folder contains the proposal; code and measured results will be added after implementation rather than claimed in advance.

## Files and Links

- [Gnasher-Group-Proposal.pdf](Gnasher-Group-Proposal.pdf)
- [Gnasher Group project repository](https://github.com/IreneAlexRamos/itai1378-project)
- [Stanford Dogs Dataset](http://vision.stanford.edu/aditya86/ImageNetDogs/)

## Planned Run Instructions

The implementation will use Google Colab. Dataset preparation, training, evaluation, and prediction instructions will be documented in the project repository as each milestone is completed.
