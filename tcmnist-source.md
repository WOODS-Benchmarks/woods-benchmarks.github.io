---
layout: default
---

## Temporal Colored MNIST with source domains: <br>A study of domain definitions in sequential data

- **Motivation:** In light of the previously mentioned cow or camel classification problem, Arjovsky et al. (2020) proposed the CMNIST dataset as a synthetic investigation of this problem. We extend this widely used dataset to time series, where we explore new domain formulations in time series.

- **Problem:** In Temporal Colored MNIST with source domains (TCMNIST-Source), we create a binary classification task of video frames. Videos are sequences of four colored MNIST digits where the goal is to predict whether the sum of the current and previous digits in the sequence is odd or even, see Figure 3(a). Prediction is made for all frames except for the first one. The label is a noisy function of the digit and color, such that the color bears a varying correlation of d with the label of the frame, and the digit sums bears an invariant correlation of 75% with the label of the frame. Domains are created such that the color correlation is constant among the frames of a video, but varies between video from different domains d in {10%, 80%, 90%}.
