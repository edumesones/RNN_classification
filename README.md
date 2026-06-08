# CNN Image Classification — Cats vs Dogs

A convolutional neural network (Keras / TensorFlow) that classifies images as **cat or
dog**. A compact, classic computer-vision example covering the full flow: data loading
from a folder structure, CNN training, and prediction on unseen images.

## Dataset layout
```
dataset/
├── training_set/      cats/  dogs/      ← used to train
├── test_set/          cats/  dogs/      ← used to validate
└── single_prediction/                  ← loose images to test the trained model
```
Keep this structure: the image generators read the class from the subfolder name.

## Model
A CNN (convolution + pooling blocks → flatten → dense) trained with Keras
`ImageDataGenerator` for augmentation, ending in a sigmoid unit for binary
classification.

## Tech stack
Python · Keras · TensorFlow

## Run it
```bash
pip install tensorflow keras
# open the notebook and run all cells; point single_prediction/ at your own images to test
```

> Note: despite the repo name, the architecture is a **CNN** (the canonical model for
> image classification), not an RNN.
