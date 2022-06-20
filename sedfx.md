---
layout: default
---

## SEDFx
- **Motivation:** In clinical settings, we train a model on the data gathered from a limited number of patients and hope this model will generalize to new patients in the future. However, this generalization between observed patients in the training dataset and new patients is not guaranteed. Distribution shifts caused by shifts in patient demographics (e.g., age, gender, and ethnicity) can cause the model to fail. We study age demographic shift with the SEDFx dataset. 

- **Problem:** We consider the sleep classification task from EEG measurements. The dataset has four source domains, where each domain contains data from participants of a certain age group. The goal is to generalize to an unseen age demographic.

- **Downloads:** The preprocessed data is available on [Academic Torrents](https://academictorrents.com/details/58ea303dce39ffe822bec7704f9eb65e4173defd) and via [Google Drive](https://drive.google.com/uc?id=15j_bsiOmMJb42mG712Vhv3jZ4MQSOgoT). It can also be directly downloaded through the [WOODS dataset download script](https://github.com/jc-audet/WOODS/blob/main/woods/scripts/download_datasets.py) by running the following command:
```sh
python -m woods.scripts.download_datasets SEDFx --data_path /path/to/data
```
- **Preprocessing** The preprocessing script can be found on the [WOODS preprocessing script](https://github.com/jc-audet/WOODS/blob/main/woods/scripts/fetch_and_preprocess.py). You can run the preprocessing yourself by running the following command:
```sh
python -m woods.scripts.fetch_and_preprocess SEDFx --data_path /path/to/data
```

### References

[1] Kemp, Bob, et al. "Analysis of a sleep-dependent neuronal feedback loop: the slow-wave microcontinuity of the EEG." IEEE Transactions on Biomedical Engineering 47.9 (2000): 1185-1194.

[2] Goldberger, Ary L., et al. "PhysioBank, PhysioToolkit, and PhysioNet: components of a new research resource for complex physiologic signals." circulation 101.23 (2000): e215-e220.

### License
This project is licensed under the [Open Data Commons Attribution license v1.0.](https://opendatacommons.org/licenses/by/summary/index.html)