---
title: "Self-supervised Dataset Distillation: A Good Compression Is All You Need"
collection: Arxiv
permalink: https://arxiv.org/abs/2404.07976
excerpt: 'This paper is about the number 1. The number 2 is left for future work.'
date: 2024
venue: 'Journal 1'
paperurl: 'https://arxiv.org/abs/2404.07976'
citation: Zhou, M., Yin, Z., Shao, S., & Shen, Z. (2024). Self-supervised dataset distillation: A good compression is all you need. arXiv preprint arXiv:2404.07976.
---

Dataset distillation aims to compress information from a large-scale original dataset to a new compact dataset while striving to preserve the utmost degree of the original data informational essence. Previous studies have predominantly concentrated on aligning the intermediate statistics between the original and distilled data, such as weight trajectory, features, gradient, BatchNorm, etc. In this work, we consider addressing this task through the new lens of model informativeness in the compression stage on the original dataset pretraining. We observe that with the prior state-of-the-art SRe2L, as model sizes increase, it becomes increasingly challenging for supervised pretrained models to recover learned information during data synthesis, as the channel-wise mean and variance inside the model are flatting and less informative. We further notice that larger variances in BN statistics from self-supervised models enable larger loss signals to update the recovered data by gradients, enjoying more informativeness during synthesis. Building on this observation, we introduce SC-DD, a simple yet effective Self-supervised Compression framework for Dataset Distillation that facilitates diverse information compression and recovery compared to traditional supervised learning schemes, further reaps the potential of large pretrained models with enhanced capabilities. Extensive experiments are conducted on CIFAR-100, Tiny-ImageNet and ImageNet-1K datasets to demonstrate the superiority of our proposed approach. The proposed SC-DD outperforms all previous state-of-the-art supervised dataset distillation methods when employing larger models, such as SRe2L, MTT, TESLA, DC, CAFE, etc., by large margins under the same recovery and post-training budgets. 
