---
layout: default
---

## HHAR: <br>Human activity recognition across smart devices
- **Motivation:** The intrinsic biases from inaccurate and poorly calibrated sensors of smart devices, along with the accumulated biases from everyday use makes human activity recognition a notoriously difficult task when task when done across devices. Contrary to static tasks where uninformative features can often be segmented out from the input features (e.g., background when classifying an animal from an image), invariant features in time series are often highly convoluted with other spurious features. We study the ability of models to ignore spurious information from complex signals with the HHAR dataset.

- **Problem:** We consider the human activity classification task from accelerometer and gyroscope measurements of smartphones and smartwatches. The dataset has five source domains, where each domain contains data gathered with a different device. The goal is to generalize to unseen smart devices.

- **Downloads:** The preprocessed data is available on [Academic Torrents](https://academictorrents.com/details/f48f38de06b3cd560fb90307b5a1997a12bcc29c) and via [Google Drive](https://drive.google.com/uc?id=1Z3IcrCE-o77p4YrvkCy-Y-0CgCyxVHet). It can also be directly downloaded through the [WOODS dataset download script](https://github.com/jc-audet/WOODS/blob/main/woods/scripts/download_datasets.py) by running the following command:
```sh
python -m woods.scripts.download_datasets HHAR --data_path /path/to/data
```
- **Preprocessing** The preprocessing script can be found on the [WOODS preprocessing script](https://github.com/jc-audet/WOODS/blob/main/woods/scripts/fetch_and_preprocess.py). You can run the preprocessing yourself by running the following command:
```sh
python -m woods.scripts.fetch_and_preprocess HHAR --data_path /path/to/data
```

### References

[1] Stisen, Allan, et al. "Smart devices are different: Assessing and mitigatingmobile sensing heterogeneities for activity recognition." Proceedings of the 13th ACM conference on embedded networked sensor systems. 2015.

[2] Dua, D. and Graff, C. (2019). UCI Machine Learning Repository [http://archive.ics.uci.edu/ml]. Irvine, CA: University of California, School of Information and Computer Science.

### License
This dataset is licensed under the [https://opendatacommons.org/licenses/by/summary/index.html](https://creativecommons.org/licenses/by-nc-sa/4.0/legalcode)
