# A Prototype-Neighbor Network for Few-Shot Classification .

# Installation

Install packages using pip:

```python
$ pip install -r requirements.txt
```

# Pre-trained Models

All pre-trained models of training Algorithms can be found [here](https://drive.google.com/drive/folders/1U8zoehc7WpTbEZjhSZ5Ufey-uCV4f3Xn?usp=drive_link).

# Dataset Preparation

## miniImageNet:



Download [miniImageNet.zip](https://drive.google.com/file/d/1QEbHFIOKIM9KmId175QaLK-r22kgd7br/view) and extract it.

## tieredImageNet:



The data we used here is preprocessed by the repo of [FRN](https://github.com/Tsingularity/FRN).

## CUB:



Download [`CUB.rar`](https://drive.google.com/drive/my-drive) and extract it.

# Training and Testing



The basic configurations are defined in configs/.

1.To train PNKNN on 5-way 5-shot miniImageNet benchmark

```python
python main.py --cfg './configs/PN_KNN/miniImageNet_res12_5way-5shot.yaml' --is_train 1 --tag main 
```

2.To test PNKNN on 5-way 5-shot miniImageNet benchmark

```python
python main.py --cfg './configs/evaluation/mini_res12_PNKNN_5way-5shot.yaml' --is_train 0 --tag test 
```



# Acknowlegements

Our implementation is based on the the official implementation of [CloserLookAgainFewShot](https://github.com/Frankluox/CloserLookAgainFewShot)
