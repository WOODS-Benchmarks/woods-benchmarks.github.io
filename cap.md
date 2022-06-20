---
layout: default
---

## CAP
- **Motivation:** A recurrent problem in computational medicine is that models trained on data from a given recording device will not generalize to data coming from another device, even when both devices are from a similar equipment provider. Failure to generalize to unseen machines can cause critical issues for clinical practice because a false sense of confidence in a model could lead to a false diagnosis. We study these machinery-induced distribution shifts with the CAP dataset.
- **Problem:** We consider the sleep stage classification task from electroencephalographic (EEG) measurements. The dataset has five source domains, where each domain contains data gathered with a different machine. The goal is to generalize to unseen machines.
- **Downloads:** The preprocessed data is available on [Academic Torrents](https://academictorrents.com/details/500d0c473108ef72e01b0f8037251b09331467f9) and via [Google Drive](https://drive.google.com/uc?id=1NFwX2CqLrenWF4az0c6J-OglAoD48PAT). It can also be directly downloaded through the [WOODS dataset download script](https://github.com/jc-audet/WOODS/blob/main/woods/scripts/download_datasets.py) by running the following command:
```sh
python -m woods.scripts.download_datasets CAP --data_path /path/to/data
```
- **Preprocessing** The preprocessing script can be found on the [WOODS preprocessing script](https://github.com/jc-audet/WOODS/blob/main/woods/scripts/fetch_and_preprocess.py). You can run the preprocessing yourself by running the following command:

```sh
python -m woods.scripts.fetch_and_preprocess CAP --data_path /path/to/data
```

### References

[1] Terzano, Mario Giovanni, et al. "Atlas, rules, and recording techniques for the scoring of cyclic alternating pattern (CAP) in human sleep." Sleep medicine 3.2 (2002): 187-199.

[2] Goldberger, Ary L., et al. "PhysioBank, PhysioToolkit, and PhysioNet: components of a new research resource for complex physiologic signals." circulation 101.23 (2000): e215-e220.

### License
This dataset is licensed under the [Open Data Commons Attribution license v1.0.](https://opendatacommons.org/licenses/by/summary/index.html)