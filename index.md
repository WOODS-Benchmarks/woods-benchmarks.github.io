# WOODS: Benchmarks for Out-of-Distribution Generalization in Time Series

**Abstract** Deep learning models often fail to generalize well under distribution shifts. Understanding and overcoming these failures have led to a new research field on Out-of-Distribution (OOD) generalization. Despite being extensively studied for static computer vision tasks, OOD generalization has been severely underexplored for time series tasks. To shine a light on this gap, we present WOODS: ten challenging time series benchmarks covering a diverse range of data modalities, such as videos, brain recordings, and smart device sensory signals. We revise the existing OOD generalization algorithms for time series tasks and evaluate them using our systematic framework. Our experiments show a large room for improvement for empirical risk minimization and OOD generalization algorithms on our datasets, thus underscoring the new challenges posed by time series tasks.

- **Paper**: See our [preprint](https://arxiv.org/abs/2203.09978) for further details on the datasets and benchmarks.

- **Evaluation Framework**: Our fair and systematic evaluation framework can be found at [https://github.com/jc-audet/WOODS](https://github.com/jc-audet/WOODS).

- **Documentation**: Documentation on our framework is available at [woods.readthedocs.io](https://woods.readthedocs.io/en/latest/index.html). It covers the many functionalities of the framework such as how to download the dataset and how to run hyperparameter sweeps. It also details how you can add your own algorithm, and dataset to the framework.


### Datasets

WOODS currently consists of ten challenging time series benchmarks covering a diverse range of data modalities, such as videos, brain recordings, and smart device sensory signals.

<svg version="1.1" xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" viewBox="0 0 3600 2400">
  <image width="3600" height="2400" xlink:href="assets/Dataset_summary.png"></image>
</svg>

<br/><br/>


