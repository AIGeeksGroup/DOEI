# DOEI
This is the code repository for the paper:

> **DOEI: Dual Optimization of Embedding Information for Attention-Enhanced Class Activation Maps**
> 
>[Hongjie Zhu](https://github.com/Potato2187/), [Zeyu Zhang](https://steve-zeyu-zhang.github.io/)†, Guansong Pang, Xu Wang, Shimin Wen, Yu Bai, Daji Ergu, [Ying Cai](https://ieeexplore.ieee.org/author/37087137422)* and [Yang Zhao](https://yangyangkiki.github.io/)
>
>*Corresponding author. †Project lead.
>
>[**[arXiv]**](https://arxiv.org/abs/2502.15885) [**[Paper with Code]**](https://paperswithcode.com/paper/doei-dual-optimization-of-embedding)

![项目相关的描述](image.png)

## Citation

```
@article{zhu2025doei,
  title={DOEI: Dual Optimization of Embedding Information for Attention-Enhanced Class Activation Maps},
  author={Zhu, Hongjie and Zhang, Zeyu and Pang, Guansong and Wang, Xu and Wen, Shimin and Bai, Yu and Ergu, Daji and Cai, Ying and Zhao, Yang},
  journal={arXiv preprint arXiv:2502.15885},
  year={2025}
}
```

## Introduction
Weakly supervised semantic segmentation (WSSS) typically utilizes limited semantic annotations to obtain initial Class Activation Maps (CAMs). However, due to the inadequate coupling between class activation responses and semantic information in high-dimensional space, the CAM is prone to object co-occurrence or under-activation, resulting in inferior recognition accuracy. To tackle this issue, we propose DOEI, Dual Optimization of Embedding Information, a novel approach that reconstructs embedding representations through semantic-aware attention weight matrices to optimize the expression capability of embedding information. Specifically, DOEI amplifies tokens with high confidence and suppresses those with low confidence during the class-to-patch interaction. This alignment of activation responses with semantic information strengthens the propagation and decoupling of target features, enabling the generated embeddings to more accurately represent target features in high-level semantic space. In addition, we propose a hybrid-feature alignment module in DOEI that combines RGB values, embedding-guided features, and self-attention weights to increase the reliability of candidate tokens. Comprehensive experiments show that DOEI is an effective plug-and-play module that empowers state-of-the-art visual transformer-based WSSS models to significantly improve the quality of CAMs and segmentation performance on popular benchmarks, including PASCAl VOC (+3.6%, +1.5%, +1.2% mIoU) and MS COCO (+1.2%, +1.6% mIoU).

## Environment Setup

To set up the environment for DOEI, follow these steps:

```sh
# create a clean conda environment from scratch
conda create --name DOEI python=3.7
conda activate DOEI

# install pip
conda install ipython
conda install pip

# install required packages
pip install -r requirements.txt
```
