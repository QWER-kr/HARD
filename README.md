# HARD: Hardware-Aware Lightweight Real-Time Semantic Segmentation Model Deployable from Edge to GPU
This repository contains the official Pytorch implementation of training & evaluation code and the pretrained models for [HARD](https://openaccess.thecvf.com/content/ACCV2024/html/Kwon_HARD__Hardware-Aware_lightweight_Real-time_semantic_segmentation_model_Deployable_from_ACCV_2024_paper.html)(ACCV24)🔥

## Installation
We alse can use MMSegmentation v0.26.0 as the codebase.

### Environment Installation
**Normal Pytorch Semantic Segmenation Code**
```
conda create -n HARD python=3.8
conda activate HARD
conda install pytorch==1.11.0 torchvision==0.12.0 torchaudio==0.11.0 cudatoolkit=11.3 -c pytorch

pip install matplotlib
```

**MMSegmentation Code**
```
conda create -n HARD_MMSeg python=3.8
conda activate HARD_MMSeg
conda install pytorch==1.11.0 torchvision==0.12.0 torchaudio==0.11.0 cudatoolkit=11.3 -c pytorch

pip install mmcv-full==1.6.0 -f https://download.openmmlab.com/mmcv/dist/cu113/torch1.11.0/index.html
pip install timm
pip install matplotlib
pip install prettytable
pip install einops
```

## Results and models

### Cityscapes
| Method   | mIoU(ss) | FPS(torch) |Model    |
| -------- | -------- | ---------- |---------|
| HARD-GPU | 73.8     | 315        |-|
| HARD-S   | 72.8     | 427        |-|
| HARD-XS  | 69.6     | 532        |-|
| HARD-XXS | 64.1     | 533        |-|

### CamVid
| Method   | mIoU(ss) | FPS(torch) |Model    |
| -------- | -------- | ---------- |---------|
| HARD-S   | 76.3     | 424        |-|
| HARD-XS  | 75.8     | 530        |-|
| HARD-XXS | 74.4     | 532        |-|
| HARD-Edge| 57.3     | -          |-|

### COCO-Stuff-10k
| Method   | mIoU(ss) | FPS(torch) |Model    |
| -------- | -------- | ---------- |---------|
| HARD-GPU | 41.0     | 271        |-|
| HARD-S   | 37.0     | 358        |-|
| HARD-XS  | 33.1     | 527        |-|
| HARD-XXS | 23.8     | 527        |-|

## Evaluation

## Training

## Speed

## Citation

If you find this work helpful to your research, please consider citing the paper:

```bibtex
@InProceedings{Kwon_2024_ACCV,
    author    = {Kwon, YoungWook and Kim, WanSoo and Kim, HyunJin},
    title     = {HARD : Hardware-Aware lightweight Real-time semantic segmentation model Deployable from Edge to GPU},
    booktitle = {Proceedings of the Asian Conference on Computer Vision (ACCV)},
    month     = {December},
    year      = {2024},
    pages     = {3552-3569}
}
```

## Acknowledgement
