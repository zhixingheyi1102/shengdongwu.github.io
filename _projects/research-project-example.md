---
title: "Neural Decoding Algorithm for Limb Movement Intent from Porcine ECoG Signals"
excerpt: "A neural decoding algorithm for analyzing electrocorticography (ECoG) signals during pig locomotion to decode limb movement intent"
type: research
image: 2-cover.png
collection: projects
tags:
  - Neural Decoding
  - Machine Learning
  - BCI
  - Signal Processing
priority: 1
---

A neural decoding algorithm has been developed to analyze electrocorticography (ECoG) signals during pig locomotion, along with synchronously recorded limb joint angle data, to decode limb movement intent.

<div class="center-image">
  <img src="../../images/projects/research/2-cover.png" alt="图片描述">
</div>

<style>
.center-image {
  text-align: center;
  margin: 20px 0;
}

.center-image img {
  max-width: 100%;
  height: auto;
  border-radius: 4px;
}
</style>

The core of the algorithm employs a cascaded U-Net architecture. This design astutely leverages the intrinsic synergistic relationships between different joints, drawing inspiration from the neuroscientific concept of spinal cord central pattern generators (CPGs) that control rhythmic movements. Mathematically, this approach effectively narrows the model's solution space, improving prediction efficiency. During training, a Scheduled Sampling strategy was introduced, where the model uses its own previous predictions as input 50% of the time and the ground truth labels the other 50%. This method helps mitigate discrepancies in data distribution between training and testing phases, thereby enhancing the model's generalization ability. 

<div class="center-image">
  <img src="../../images/projects/research/unet.png" alt="图片描述">
</div>

<style>
.center-image {
  text-align: center;
  margin: 20px 0;
}

.center-image img {
  max-width: 100%;
  height: auto;
  border-radius: 4px;
}
</style>

Experimental results demonstrate that this method can effectively decode movement trajectories from ECoG signals. The predicted trajectories show a high degree of concordance with the actual trajectories across multiple joints, with Pearson correlation coefficients typically ranging from 0.84 to 0.90. Even in more challenging data segments, such as instances where joint correlations were 0.78 and 0.54, the model maintained strong overall predictive performance, thus validating the effectiveness of the proposed algorithm. 

<div class="center-image">
  <img src="../../images/projects/research/result.png" alt="图片描述">
</div>

<style>
.center-image {
  text-align: center;
  margin: 20px 0;
}

.center-image img {
  max-width: 100%;
  height: auto;
  border-radius: 4px;
}
</style>
