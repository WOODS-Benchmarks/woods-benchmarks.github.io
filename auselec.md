---
layout: default
---

## AusElec: <br>Forecasting of energy consumption throughout the year
- **Motivation:** Seasonality is the property of time series where recurring characteristics appear every cycle of a fixed period, e.g., weekly. A common practice in the forecasting field is to provide models with additional information, e.g., day of week in order to allow models to leverage seasonality for better predictions. However, holidays is a seasonality of time series that is very sparse which models often fail to capture. We study the performance of models on sparse seasonality with the AusElec dataset.

- **Problem:** We consider the electricity consumption forecasting task. The dataset has 13 time domains, where each domain contains data from different months and holidays. The goal is to perform well on all seasonalities.

- **Downloads:** The preprocessed data is available through Huggingface <a href="https://huggingface.co/datasets/monash_tsf">monash_tsf</a> dataset and through <a href="https://zenodo.org/record/4659727#.Yquiu9LMJhE">Zenodo</a>. It can also be directly downloaded through the <a href="https://github.com/jc-audet/WOODS">WOODS repository</a> by running the following command:
```sh
python -m woods.scripts.download_datasets AusElec --data_path /path/to/data
```

### References

[1] Hyndman, Rob J., and George Athanasopoulos. Forecasting: principles and practice. OTexts, 2018.

[2] Godahewa, Rakshitha, et al. "Monash time series forecasting archive." arXiv preprint arXiv:2105.06643 (2021).

### License
This dataset is licensed under the [Creative Commons Attribution 4.0 International License](https://creativecommons.org/licenses/by/4.0/)
