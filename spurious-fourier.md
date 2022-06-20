---
layout: default
---

## Spurious-Fourier: <br>Spurious features encoded in the frequency domain
- **Motivation:** Consider the task of distinguishing cows and camels in pictures. We train a deep learning model to minimize the empirical risk on a labeled dataset. However, the dataset is heavily tainted by selection bias, as the vast majority of cow images were taken in green pastures, and the vast majority of camel images were taken in sandy areas. At test time, we observe that our deep learning model consistently and confidently classifies images of cows on sandy beaches as camels. We conclude that the model successfully minimized the empirical risk over the training dataset by leveraging the selection bias, thus classifying green backgrounds as cows and beige backgrounds as camels. We propose the Spurious-Fourier dataset as an adaptation of the cow or camel classification problem to time series.

- **Problem:** We create a dataset composed of one-dimensional signals, where the task is to perform binary classification based on the frequency characteristics. Signals are constructed from Fourier spectra with one low-frequency peak (L<sub>A</sub>=2Hz or L<sub>B</sub>=4Hz) and one high-frequency peak (H<sub>A</sub>=7Hz or H<sub>B</sub>=9Hz), see Figure 2. Domains D<sup>d</sup>|<sub>d in {10%, 80%, 90%}</sub> contain signal-label pairs, where the label is a noisy function of the low- and high-frequencies such that low-frequency peaks bear a varying correlation of d with the label and high-frequency peaks bear an invariant correlation of 75% with the label.
