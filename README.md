# t-MoCo-v2
## Official PyTorch implementation of [Your Contrastive Learning is Secretly Doing Stochastic Neighbor Embedding](https://arxiv.org/abs/2205.14814) (ICLR 2023)

Contrastive learning, especially self-supervised contrastive learning (SSCL), has achieved great success in extracting powerful features from unlabeled data. In this work, we contribute to the theoretical understanding of SSCL and uncover its connection to the classic data visualization method, stochastic neighbor embedding (SNE) (Hinton & Roweis, 2002), whose goal is to preserve pairwise distances. From the perspective of preserving neighboring information, SSCL can be viewed as a special case of SNE with the input space pairwise similarities specified by data augmentation. The
established correspondence facilitates deeper theoretical understanding of learned features of SSCL, as well as methodological guidelines for practical improvement. Specifically, through the lens of SNE, we provide novel analysis on domain-agnostic augmentations, implicit bias and robustness of learned features. To illustrate the practical advantage, we demonstrate that the modifications from SNE to t-SNE (Van der Maaten & Hinton, 2008) can also be adopted in the SSCL setting, achieving significant improvement in both in-distribution and out-of-distribution generalization.

## Setup
This repo provides the code for t-MoCo-v2, and is based on [MoCo](https://github.com/facebookresearch/moco). The same change can be directly made to SimCLR to reprocude t-SimCLR.

Please follow the setup of MoCo.

## Run
Training t-MoCo-v2 from scratch:
```
bash script/moco_tsne_pena0_tdf10_t5.sh
```


## Citation
If you find the code useful for your research, please consider citing
```
@inproceedings{hu2022your,
  title={Your Contrastive Learning Is Secretly Doing Stochastic Neighbor Embedding},
  author={Hu, Tianyang and Zhili, LIU and Zhou, Fengwei and Wang, Wenjia and Huang, Weiran},
  booktitle={ICLR},
  year={2023}
}
```
