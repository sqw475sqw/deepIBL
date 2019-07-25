
# Stochastic Attraction-Repulsion Embedding for Large Scale Localization

This contains the code and model for training ground-view geo-localization method described in: Stochastic Attraction-Repulsion Embedding for Large Scale Localization, ICCV2019. 

![alt text](./pipeline.png)

# Abstract
This paper tackles the problem of large-scale image-based localization (IBL) where the spatial location of a query image is determined by finding out the most similar reference images in a large database.  For solving this problem, a critical task is to learn discriminative image representation that captures informative information relevant for localization. We propose a novel representation learning method having higher location-discriminating power. It provides the following contributions: 1) we represent a place (location) as a set of exemplar images depicting the same landmarks and aim to maximize similarities among intra-place images while minimizing similarities among inter-place images; 2) we model a similarity measure as a probability distribution on $L_2$-metric distances between intra-place and inter-place image representations; 3) we propose a new Stochastic Attraction and Repulsion Embedding (SARE) loss function minimizing the KL divergence between the learned and the actual probability distributions; 4) we give theoretical comparisons between SARE, triplet ranking and contrastive losses. It provides insights into why SARE is better by analyzing gradients. Our SARE loss is easy to implement and pluggable to any CNN. Experiments show that the method improves localization performance on standard benchmarks by a large margin.  Demonstrating the broad applicability of our method, we obtain the $3^{rd}$ place out of 209 teams in the 2018 Google Landmark Retrieval Challenge \cite{Google_Landmark}. Our code and model are available at \url{https://github.com/Liumouliu/deepIBL}


This code is developed based on MatConvNet.

You first need to download the NetVLAD code (https://github.com/Relja/netvlad), then run our training methods. 


If you use our codes or models in your research, please cite:

@article{liu2018deep,
  title={Deep Stochastic Attraction and Repulsion Embedding for Image Based Localization},
  author={Liu, Liu and Li, Hongdong and Dai, Yuchao},
  journal={arXiv preprint arXiv:1808.08779},
  year={2018}
}


Our pre-trained model by Gaussian kernel defined SARE loss (Our-Ind.) is available at:

https://drive.google.com/file/d/1riu7rJEH4Eh5vhQ_tM8dBtUfwhKilqhq/view?usp=sharing

If you need more pre-trained models, Please contact me. (Liu.Liu@anu.edu.au) 

