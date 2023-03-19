# SDSC4016 Fundamentals of Machine Learning II

SDSC4016 Homework 2:

- [On Kaggle](https://www.kaggle.com/competitions/sdsc4016-fundls-of-ml-2-hw2/overview)

## Description

Solve an image classification problem with CNN.

## Getting Started

### Dependencies

- Python
  - Python 3.10+
  - Jupyter
  - pytorch
  - torchvision

### Install mini-conda and mamba

```bash
wget https://repo.anaconda.com/miniconda/Miniconda3-latest-Linux-x86_64.sh
bash ./Miniconda3-latest-Linux-x86_64.sh
conda install mamba -n base -c conda-forge
```

### Set up conda environment

```bash
mamba create -n 4016hw2
mamba activate 4016hw2
```

### Installing dependencies

```bash
# conda or mamba
mamba install pytorch torchvision torchaudio pytorch-cuda=11.7 -c pytorch -c nvidia
mamba install -c conda-forge Jupyter ipykernel
mamba install -c conda-forge pandas numpy seaborn matplotlib scikit-learn tqdm
```

### Code

[Weak Baseline](src/HW2_Baseline.ipynb)

[Strong Baseline](src/model/efficientnetv2/HW2_efficientnetv2_lV8_final.ipynb)

<!-- ### Dataset

[Training set](data/training/)

[Testing set](data/testing/) -->

### Tested Result on Kaggle

[Results on Kaggle](md/kaggle.md)

### Final Score (Strong Baseline)

- Public: 0.90658
<!-- - Private: 0.89874 -->
