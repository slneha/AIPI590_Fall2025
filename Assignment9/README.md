# Interpreting a Convolutional Neural Network on X vs O Classification

This repository contains an experiment designed to understand and interpret how a small convolutional neural network learns to discriminate between two simple image classes: X and O. Instead of treating the CNN as a black box, the notebook walks through a series of probing methods that expose what individual convolutional filters compute, how activations relate to each class, and which internal components are truly causal for the model's predictions.

---

## Project Overview

The network is trained on images containing hand-drawn X and O shapes. After training, a set of interpretability techniques is applied to examine the internal computation of the first convolutional layer and the classification head:

• visualizing learned convolutional kernels  
• visualizing per-filter activation maps on example images  
• comparing mean Global Average Pooling (GAP) activations per class  
• computing correlations between learned filters and hand-crafted templates  
• probing channel importance by scaling feature maps  
• probing polarity importance using half-clamp tests

Together, these analyses build a concrete picture of what features the network uses and how classification emerges from low-level patterns.
