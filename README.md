# Zero-Shot Category-Level Object Pose Estimation

This repository contains Pytorch code for the paper **Zero-Shot Category-Level Object Pose Estimation (Goodwin et al., 2020)** [[arxiv]](https://arxiv.org/abs/2204.03635).

![alt text](/readme/main.jpg?raw=true "Zero-Shot Category-Level Object Pose Estimation")

## Installation
* Make environment:
`conda env create -f environment.yml`

* Install Pillow < 7.0 with `pip` to overcome a `torchvision` bug:
`pip install 'pillow<7'`

* Install Pytorch3D from Github:
`pip install "git+https://github.com/facebookresearch/pytorch3d.git@stable"`

Install the `zsp` python package implemented in this repo with `pip install -e .`

## Dataset
This work uses the Common Objects in 3D (CO3D) dataset. The repo for this dataset, with download instructions, is [here](https://github.com/facebookresearch/co3d). 

This dataset contains 18,619 multi-frame sequences capturing different instances of 50 object categories. For full dataset is around 1.4TB. For evaluation in this work, we manually annotated 10 sequences from each of 20 categories with ground-truth poses (these annotations are found under `data/class_labels`). The relevant subset of the dataset is thus smaller at around ~15GB. If you are struggling to download the entire CO3D dataset, please contact me and I will try to share this subset with you.

<!-- ## Running the code
Once you have followed  -->