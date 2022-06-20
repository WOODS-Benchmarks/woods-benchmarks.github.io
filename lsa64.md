---
layout: default
---

## LSA64
- **Motivation:** Communication is an individualistic way to convey information through different media: text, speech, body language, and many others. However, some media are more distinctive and challenging than others. For example, text communication has less inter-individual variability than body language or speech. If deep learning systems hope to interact with humans effectively, models need to generalize to new and evolving mannerisms, accents, and other subtle variations in communication that significantly impact the meaning of the message conveyed. We study the ability of models to recognize information coming from unseen individuals with the LSA64 dataset.

- **Problem:** We consider the video classification of signed words in Argentinian Sign Language. The dataset has five source domains, where each domain contains videos of different signers. The goal is to generalize to unseen signers.

- **Downloads:** The preprocessed data is available on [Academic Torrents](https://academictorrents.com/details/704bf5981eb337cae7cb518c3abb9d7b6bdf3e49) and via [Google Drive](https://drive.google.com/uc?id=1YwwSg8Dt178ySp3ht_BLJwl5j5s_IU1m). It can also be directly downloaded through the [WOODS dataset download script](https://github.com/jc-audet/WOODS/blob/main/woods/scripts/download_datasets.py) by running the following command:
```sh
python -m woods.scripts.download_datasets LSA64 --data_path /path/to/data
```

### References

[1] Ronchetti, Franco, et al. "LSA64: an Argentinian sign language dataset." XXII Congreso Argentino de Ciencias de la Computación (CACIC 2016).. 2016.

### License
This dataset is licensed under the [Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License](https://creativecommons.org/licenses/by-nc-sa/4.0)
