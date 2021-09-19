# SkimLit
NLP model (trained on PubMed200k RCT dataset) to make reading medical abstracts (from pubmed etc) easier
---

The purpose of this notebook is to build an NLP model to make reading medical abstracts (from pubmed etc) easier.

The paper being implemented here is : [PubMed 200k RCT: a Dataset for Sequenctial Sentence Classification in Medical Abstracts](https://arxiv.org/abs/1710.06071)

Model used in the paper : [Neural networks for joint sentence classification in medical paper abstracts](https://arxiv.org/pdf/1612.05251.pdf)

### About the Dataset
PubMed 200k RCT,  dataset based on PubMed for sequential sentence classification. The dataset consists of approximately 200,000 abstracts of randomized controlled trials, totaling 2.3 million sentences. Each sentence of each abstract is labeled with their role in the abstract using one of the following classes: background, objective, method, result, or conclusion.

```
Dernoncourt, F., & Lee, J. Y. (2017).
Pubmed 200k rct: a dataset for sequential sentence classification in medical abstracts.
arXiv preprint arXiv:1710.06071.
```

---
### Modelling Experiments 
- Model 0: TF-IDF Multinomial Naivee Bayes classifier (baseline)
- Model 1: Conv1D with token embeddings
- Model 2: Feature Extraction with pretrained token embeddings
- Model 3: Conv1D with character embeddings
- Model 4: Combining pretrained token embeddings + characters embeddings (hybrid embedding layer)
- Model 5: Tribrid Transfer Learning with pretrained token embeddings + character embeddings + positional embeddings

---

### Things left to-do:
- MAKE EXAMPLE PREDICTIONS!!
- Add tensorboard callbacks 
- Train the model on the 200k dataset
- etc.


---
---
