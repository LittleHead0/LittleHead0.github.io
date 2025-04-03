---
permalink: /
title: "Muxin Zhou"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---
Hi everyone! I’m Muxin Zhou (周慕歆), a second-year master’s student in Machine Learning Department, at Mohamed bin Zayed University of Artificial Intelligence. I obtained Bachelor’s degree from Peking University, majored in Computer Science. My research mainly focus on Robotic tactile perception.

I feel honored to be advised by Prof. Dezhen Song and Dr. Gus Xia at Mohamed bin Zayed University of Artificial Intelligence. I was advised by Dr. Zhiqiang Shen during my first year of master's studies.

You can find my [CV](./assets/MuxinZhou_Resume.pdf) here.


Email: muxin dot zhou@mbzuai dot ac dot ae / [Github](https://github.com/LittleHead0) 

# Projects
## [Self-supervised Dataset Distillation: A Good Compression Is All You Need](https://arxiv.org/abs/2404.07976)
Dataset distillation aims to compress information from a large-scale original dataset to a new compact dataset while striving to preserve the utmost degree of the original data informational essence. Previous studies have predominantly concentrated on aligning the intermediate statistics between the original and distilled data, such as weight trajectory, features, gradient, BatchNorm, etc. In this work, we consider addressing this task through the new lens of model informativeness in the compression stage on the original dataset pretraining. We observe that with the prior state-of-the-art SRe2L, as model sizes increase, it becomes increasingly challenging for supervised pretrained models to recover learned information during data synthesis, as the channel-wise mean and variance inside the model are flatting and less informative. We further notice that larger variances in BN statistics from self-supervised models enable larger loss signals to update the recovered data by gradients, enjoying more informativeness during synthesis. Building on this observation, we introduce SC-DD, a simple yet effective Self-supervised Compression framework for Dataset Distillation that facilitates diverse information compression and recovery compared to traditional supervised learning schemes, further reaps the potential of large pretrained models with enhanced capabilities. Extensive experiments are conducted on CIFAR-100, Tiny-ImageNet and ImageNet-1K datasets to demonstrate the superiority of our proposed approach. The proposed SC-DD outperforms all previous state-of-the-art supervised dataset distillation methods when employing larger models, such as SRe2L, MTT, TESLA, DC, CAFE, etc., by large margins under the same recovery and post-training budgets

## [Generalized Large-Scale Data Condensation via Various Backbone and Statistical Matching](https://arxiv.org/abs/2311.17950)
The lightweight "local-match-global" matching introduced by SRe2L successfully creates a distilled dataset with comprehensive information on the full 224x224 ImageNet-1k. However, this one-sided approach is limited to a particular backbone, layer, and statistics, which limits the improvement of the generalization of a distilled dataset. We suggest that sufficient and various "local-match-global" matching are more precise and effective than a single one and has the ability to create a distilled dataset with richer information and better generalization. We call this perspective "generalized matching" and propose Generalized Various Backbone and Statistical Matching (G-VBSM) in this work, which aims to create a synthetic dataset with densities, ensuring consistency with the complete dataset across various backbones, layers, and statistics. As experimentally demonstrated, G-VBSM is the first algorithm to obtain strong performance across both small-scale and large-scale datasets. Specifically, G-VBSM achieves a performance of 38.7% on CIFAR-100 with 128-width ConvNet, 47.6% on Tiny-ImageNet with ResNet18, and 31.4% on the full 224x224 ImageNet-1k with ResNet18, under images per class (IPC) 10, 50, and 10, respectively. These results surpass all SOTA methods by margins of 3.9%, 6.5%, and 10.1%, respectively.

