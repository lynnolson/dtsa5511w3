# dtsa5511w3

week 3 assignment for DTSA5511

<!-- ABOUT THE PROJECT -->
## About the assignment
This project applies convolutional networks to classify whether metastatic cancer is present in a histological slide. It's the Kaggle task [Histopathologic Cancer Detection](https://www.kaggle.com/competitions/histopathologic-cancer-detection/overview).

It was done for CU Boulder's DTSA5511 Introduction to Deep Learning.

The methods covered include
- Traditional convolutional networks (CNNs)
- ResNets


### Dependencies

The code was developed with Python 3.10.4 and the following libraries and versions:

- numpy==1.24.3
- pandas==2.0.3
- skimage==0.21.0
- sklearn==1.3.0
- torch==2.0.1+cu117
- torchvision==0.15.2+cu117
- wandb==0.15.9

You will need a [Weights and Biases](https://wandb.ai/site) account.

The full environment setting can be installed through:
```
conda env create -f conda-environment.yaml
conda activate msds
```

### Data

The [data](https://www.kaggle.com/competitions/histopathologic-cancer-detection/data) used was downloaded from Kaggle.  I don't include it here because it's too large.

### Usage

All code may be found and run in the notebook cancer_hist.ipynb.  The models were trained on a A100 GPU with 48GB of memory. They can be trained on something much smaller but still would need a GPU.  I also load all images into memory for speed (consumes over 7GB.)
