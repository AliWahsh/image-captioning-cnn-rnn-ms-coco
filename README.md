# A Deep Learning Framework for Image Captioning using CNN–RNN Architecture on MS COCO

**Advanced Machine Learning II — Project 2 (GIU)**

Course project for Advanced Machine Learning II. This repository implements an image captioning system on the **MS COCO 2014** dataset, where images are paired with human-written captions and a deep learning model learns to generate natural language descriptions for unseen images.

The framework combines a **Convolutional Neural Network (CNN)** for visual feature extraction with a **Recurrent Neural Network (RNN/LSTM)** for sequence generation. Experiments were conducted using **PyTorch** with GPU acceleration in notebook environments such as Google Colab and Kaggle.

## Contents

| File                       | Description                                                                                 |
| -------------------------- | ------------------------------------------------------------------------------------------- |
| `final.ipynb`              | Main notebook containing data preprocessing, model implementation, training, and evaluation |
| `README.md`                | Project overview and execution instructions                                                 |
| `.gitignore`               | Excludes datasets, checkpoints, virtual environments, and local artifacts                   |

## Model Architecture

### CNN Encoder

* Extracts high-level visual features from input images
* Uses pretrained convolutional networks for image representation

### RNN Decoder

* Generates captions word-by-word from encoded image features
* Learns language structure and contextual relationships between words

## Dataset

### MS COCO 2014 (Common Objects in Context)

The project uses the MS COCO dataset, one of the most widely used benchmarks for image captioning research.

Features:

* Large-scale real-world image collection
* Multiple human-annotated captions per image
* Diverse object categories and scenes
* Standard benchmark for caption generation tasks

## Prerequisites

* Python 3.10+ recommended
* PyTorch
* CUDA-enabled GPU (optional but recommended)
* Jupyter Notebook, VS Code, or Google Colab
* Kaggle account and API credentials if downloading data through `kagglehub`

If using Kaggle API credentials:

* Place `kaggle.json` in `~/.kaggle/`
* Do not commit credentials to the repository

## Running Locally

1. Create and activate a Python virtual environment.
2. Install the required dependencies.
3. Download and prepare the MS COCO dataset.
4. Open `final.ipynb` in Jupyter Lab, VS Code, or Colab.
5. Run notebook cells sequentially to reproduce training and evaluation results.

## Technologies Used

* Python
* PyTorch
* NumPy
* Pandas
* Matplotlib
* NLTK
* KaggleHub
* Jupyter Notebook
