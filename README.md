# Sign Language Classification with CNN/VGG19 and Explainable AI

This repository contains the code and supporting files for a sign language recognition project based on deep learning and Explainable Artificial Intelligence (XAI).

This work is associated with the following publication:
> El-Qoraychy, Fatima-Zahrae, et al. "Explainable AI for sign language recognition models: Integrating Grad-Cam LIME and Integrated Gradients." *PLoS One* 20.12 (2025): e0336481.

## Overview

The goal of this project is to classify sign language images using a deep learning model based on CNN/VGG19 and to explain the model predictions using XAI methods.
The project was initially developed on Kaggle/Jupyter Notebook. The main notebook contains the Python implementation used for preprocessing, prediction, classification, visualization, and explainability.

## Repository Structure

```text
sign-language-classification-cnn-vgg19-XAI/
│
├── sign-language-classification-cnn-vgg19.ipynb
├── lbl_binarizer.pkl
├── README.md
└── requirements.txt
```

## Files Description

### `sign-language-classification-cnn-vgg19.ipynb`

This is the main Python/Jupyter notebook of the project.

It contains the workflow for sign language classification, including:
- importing the required Python libraries;
- loading image data;
- preprocessing images before prediction;
- using a CNN/VGG19-based deep learning model;
- generating predictions for sign language classes;
- converting model outputs into readable class labels;
- visualizing classification results;
- applying explainability methods such as Grad-CAM, LIME, and Integrated Gradients.

### `lbl_binarizer.pkl`

This file contains the saved label binarizer used during the classification process.
The neural network produces numerical outputs. The label binarizer is required to convert these numerical outputs back into the correct sign language labels, such as letters.
This file must be kept with the notebook because predictions may be incorrectly interpreted without the same label mapping used during training.

### `requirements.txt`

This file lists the Python packages required to run the notebook.

## Model File

The trained model file is not included in this GitHub repository if it exceeds the GitHub upload limit.
For this reason, the trained model should be stored externally.
```text
Model link: https://www.kaggle.com/models/fatimaelqoraychy/model
```
## Dataset

```text
Dataset link: https://www.kaggle.com/datasets/fatimaelqoraychy/dataset
Dataset test: https://www.kaggle.com/datasets/fatimaelqoraychy/letter
```
## Installation
Clone the repository:

```bash
git clone https://github.com/YOUR_USERNAME/sign-language-classification-cnn-vgg19-XAI.git
cd sign-language-classification-cnn-vgg19-XAI
```
Install the required packages:

```bash
pip install -r requirements.txt
```

## How to Run

Open the notebook with Jupyter Notebook:

```bash
jupyter notebook sign-language-classification-cnn-vgg19.ipynb
```

Then run the cells step by step.

You can also run the notebook on Kaggle or Google Colab.

Before running the notebook, make sure that these files are available in the correct path:

```text
sign-language-classification-cnn-vgg19.ipynb
lbl_binarizer.pkl
```

If the trained model is stored externally, download it first from the model link and place it in the same folder or adapt the path inside the notebook.

## Explainable AI Methods

This project focuses not only on classification but also on explainability. XAI methods help understand why the model makes a specific prediction.

The explainability methods associated with this work include:

- **Grad-CAM**: highlights the regions of the image that strongly influenced the CNN prediction;
- **LIME**: explains individual predictions by analyzing the effect of local image perturbations;
- **Integrated Gradients**: attributes the prediction to input features by integrating gradients along a path from a baseline image to the input image.
These methods are useful for interpreting deep learning models, especially in sensitive applications such as sign language recognition.

## Citation
If you use this work, please cite the following paper:

```bibtex
@article{10.1371/journal.pone.0336481,
    doi = {10.1371/journal.pone.0336481},
    author = {El-Qoraychy, Fatima-Zahrae AND Mualla, Yazan AND Zhao, Hui AND Dridi, Mahjoub AND Créput, Jean-Charles AND Longo, Luca},
    journal = {PLOS ONE},
    publisher = {Public Library of Science},
    title = {Explainable AI for sign language recognition models: Integrating Grad-Cam LIME and Integrated Gradients},
    year = {2025},
    month = {12},
    volume = {20},
    url = {https://doi.org/10.1371/journal.pone.0336481},
    pages = {1-24},
    number = {12}
}
```
Plain-text citation:
```text
El-Qoraychy, Fatima-Zahrae, et al. "Explainable AI for sign language recognition models: Integrating Grad-Cam LIME and Integrated Gradients." PLoS One 20.12 (2025): e0336481.
```

## License

This repository is shared for academic and research purposes.
