---
layout: default
---

## AusElec: <br>Emotion recognition across different conversational emotion shifts 
- **Motivation:** Speakers tend to maintain an emotional state over a conversation. However, external stimuli can invoke a shift in the emotional state of speakers. Such emotion shift are often sparsely represented in the data, making it hard for models to classify them adequately. Recent work on emotion recognition models show the failure of existing models to adapt to those emotion shift. We study the performance of models on emotional shift with the IEMOCAP dataset.

- **Problem:** We consider the emotion recognition task. The dataset has 11 time domains, where each domain contains data from a different emotion shift during conversations. The goal is to perform well on all conversational emotion shifts.

- **Download & preprocess:** The IEMOCAP is only accessible through the <a href="https://sail.usc.edu/iemocap/iemocap_release.htm">IEMOCAP website</a>. You will need to adhere to their license agreement to get access to the raw data, and then run the preprocessing script by running the following command:
```sh
python -m woods.scripts.fetch_and_preprocess IEMOCAP --data_path /path/to/downloaded/data
```

### References

[1] Busso, Carlos, et al. "IEMOCAP: Interactive emotional dyadic motion capture database." Language resources and evaluation 42.4 (2008): 335-359.

### License
This dataset is licensed under its own [license](https://sail.usc.edu/iemocap/iemocap_release.htm). 
