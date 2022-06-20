---
layout: default
---

## PCL
- **Motivation:** Aside from changes in the recording device and shifts in patient demographics, human intervention in the data gathering process is another contributing factor to the distribution shift that can lead to failure of clinical models (e.g., Camelyon17). This challenge is especially prevalent in temporal medical data (e.g., EEG, MEG, and others) because recording devices are complex tools greatly affected by nonlinear effects and modulations. These effects are often caused by context and preparations made before the recording. We study these procedural shifts with the PCL dataset. 

- **Problem:** We consider the motor imagery task from electroencephalographic (EEG) measurements. The dataset has three source domains, where each domain contains a dataset from a different research group carrying out the same task. The goal is to generalize to unseen data gathering processes.

- **Downloads:** The preprocessed data is available on [Academic Torrents](https://academictorrents.com/details/e8b0a24177988f9c3f8c3c63a8212546f67a25a3) and via [Google Drive](https://drive.google.com/uc?id=118DNxHpzeJwVTM22wzZhSiOuDsno0nay). It can also be directly downloaded through the [WOODS dataset download script](https://github.com/jc-audet/WOODS/blob/main/woods/scripts/download_datasets.py) by running the following command:
```sh
python -m woods.scripts.download_datasets PCL --data_path /path/to/data
```
- **Preprocessing** The preprocessing script can be found on the [WOODS preprocessing script](https://github.com/jc-audet/WOODS/blob/main/woods/scripts/fetch_and_preprocess.py). You can run the preprocessing yourself by running the following command:
```sh
python -m woods.scripts.fetch_and_preprocess PCL --data_path /path/to/data
```

### References

[1] Lee, Min-Ho, et al. "EEG dataset and OpenBMI toolbox for three BCI paradigms: An investigation into BCI illiteracy." GigaScience 8.5 (2019): giz002.

[2] Schalk, Gerwin, et al. "BCI2000: a general-purpose brain-computer interface (BCI) system." IEEE Transactions on biomedical engineering 51.6 (2004): 1034-1043.

[3] Cho, Hohyun, et al. "EEG datasets for motor imagery brain–computer interface." GigaScience 6.7 (2017): gix034.

[4] Jayaram, Vinay, and Alexandre Barachant. "MOABB: trustworthy algorithm benchmarking for BCIs." Journal of neural engineering 15.6 (2018): 066011.

### License
The Schalk, Gerwin, et al. (2004) dataset is licensed under the [Open Data Commons Attribution license v1.0.](https://opendatacommons.org/licenses/by/summary/index.html)
The  Lee, Min-Ho, et al. (2019) dataset is licensed under the [No Rights Reserved license](https://creativecommons.org/share-your-work/public-domain/cc0)
The Cho, Hohyun, et al. (2017) dataset is licensed under the [CC0 1.0 Universal Public Domain Dedication license](https://creativecommons.org/publicdomain/zero/1.0/)
