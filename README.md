# Awesome-Speech-Pretraining
Paper, Code and Statistics for Self-Supervised Learning and Pre-Training on Speech.

🌟 represents important papers. 

## Papers

### 2018
- 🌟 CPC: [Representation Learning with Contrastive Predictive Coding](https://arxiv.org/abs/1807.03748) - *A Oord et al*, `arXiv 2018`

### 2019

- 🌟 APC: [An Unsupervised Autoregressive Model for Speech Representation Learning](https://arxiv.org/abs/1904.03240) - *YA Chung et al*, `INTERSPEECH 2019`
- 🌟 [wav2vec: Unsupervised Pre-training for Speech Recognition](https://arxiv.org/abs/1904.05862) - *S Schneider et al*, `INTERSPEECH 2019`
- 🌟 [vq-wav2vec: Self-Supervised Learning of Discrete Speech Representations](https://arxiv.org/abs/1910.05453) - *A Baevski et al*, `arXiv 2019, ICLR 2020`
- MPC: [Improving Transformer-based Speech Recognition Using Unsupervised Pre-training](https://arxiv.org/abs/1910.09932)  - *D Jiang et al*, `arXiv 2019`

### 2020

- Bidir CPC: [Learning robust and multilingual speech representations](https://arxiv.org/abs/2001.11128) - *K Kawakami et al*, `EMNLP 2020`
- Multi-target APC: [Improved speech representations with multi-target autoregressive predictive coding](https://arxiv.org/abs/2004.05274) - *YA Chung et al*, `ACL 2020`
- Modified CPC: [Unsupervised pretraining transfers well across languages](https://arxiv.org/abs/2002.02848) - *M Riviere et al*, `ICASSP 2020`
- [Mockingjay: Unsupervised speech representation learning with deep bidirectional transformer encoders](https://arxiv.org/abs/1910.12638) - *AT Liu et al*, `ICASSP 2020`
- vq-wav2vec-FT: [Effectiveness of self-supervised pre-training for asr](https://ieeexplore.ieee.org/abstract/document/9054224/) - *A Baevski et al*, `ICASSP 2020`
- DeCoAR: [Deep contextualized acoustic representations for semi-supervised speech recognition](https://arxiv.org/abs/1912.01679) - *S Ling et al*, `ICASSP 2020`
- [Improved noisy student training for automatic speech recognition](https://arxiv.org/abs/2005.09629) - *DS Park et al*, `INTERSPEECH 2020`
- 🌟 [wav2vec 2.0: A framework for self-supervised learning of speech representations](https://arxiv.org/abs/2006.11477) - *A Baevski et al*, `NeurIPS 2020`
- Multi-lingual wav2vec 2.0: [Unsupervised cross-lingual representation learning for speech recognition](https://arxiv.org/abs/2006.13979) - *A Conneau et al*, `arXiv 2020`
- Self-Training  wav2vec 2.0: [Self-training and Pre-training are Complementary for Speech Recognition](https://arxiv.org/abs/2010.11430)  - *Q Xu et al*, `arXiv 2020, ICASSP 2021`
- [Decoar 2.0: Deep contextualized acoustic representations with vector quantization](https://arxiv.org/abs/2012.06659)`arXiv 2020`
- [Pushing the limits of semi-supervised learning for automatic speech recognition](https://arxiv.org/abs/2010.10504) - *Y Zhang et al*, `arXiv 2020`

### 2021

- [Unispeech: Unified speech representation learning with labeled and unlabeled data](https://arxiv.org/abs/2101.07597)- *C Wang et al*, `ACL 2021`
- [Tera: Self-supervised learning of transformer encoder representation for speech](https://ieeexplore.ieee.org/abstract/document/9478264/) - *AT Liu et al*, `TASLP 2020`

- [Robust wav2vec 2.0: Analyzing Domain Shift in Self-Supervised Pre-Training](https://arxiv.org/abs/2104.01027) - *WN Hsu et al*, `arXiv 2021`
- Zero-shot wav2vec 2.0: [Simple and Effective Zero-shot Cross-lingual Phoneme Recognition](https://arxiv.org/abs/2109.11680) - *Q Xu et al*, `arXiv 2021`
- 🌟 wav2vec-U: [Unsupervised Speech Recognition](https://arxiv.org/abs/2105.11084) - *A Baevski et al*, `NeurIPS 2021`
- 🌟 [HuBERT: Self-Supervised Speech Representation Learning by Masked Prediction of Hidden Units](https://arxiv.org/abs/2106.07447) - *WN Hsu et al*, `TASLP 2021`
- 🌟 [SUPERB: Speech processing Universal PERformance Benchmark](https://arxiv.org/abs/2105.01051) - *S Yang et al*, `arXiv 2021`
- [Speecht5: Unified-modal encoder-decoder pre-training for spoken language processing](https://arxiv.org/abs/2110.07205) - *J Ao et al*, `arXiv 2021`
- [Wavlm: Large-scale self-supervised pre-training for full stack speech processing](https://arxiv.org/abs/2110.13900) - *S Chen et al*, `arXiv 2021`

- [Bigssl: Exploring the frontier of large-scale semi-supervised learning for automatic speech recognition](https://arxiv.org/abs/2109.13226) - *Y Zhang et al*, `arXiv 2021`

### 2022

- [data2vec: A General Framework for Self-supervised Learning in Speech, Vision and Language](https://ai.facebook.com/research/data2vec-a-general-framework-for-self-supervised-learning-in-speech-vision-and-language) - *A Baevski et al*, `arXiv 2022`

### Special: SSL for TTS

- [Unsupervised acoustic unit discovery for speech synthesis using discrete latent-variable neural networks](https://arxiv.org/abs/1904.07556) - *R Eloff et al*, `INTERSPEECH 2019`
- [Unsupervised Learning For Sequence-to-sequence Text-to-speech For Low-resource Languages](https://arxiv.org/abs/2008.04549) - *H Zhang et al*, `INTERSPEECH 2020`



## Statistics

Statistics on speech pretraining. 

### wav2vec 2.0

#### Pre-training

| Size  | Transformer                                         | Samples           | Batch Size | Train Time                                                   |
| ----- | --------------------------------------------------- | ----------------- | ---------- | ------------------------------------------------------------ |
| BASE  | 12 blocks, model dimension 768, FFN 3072, 8 heads   | 1.4m(cropped)/GPU | 1.6h       | 400k updates, 64 V100 * 1.6d                                 |
| LARGE | 24 blocks, model dimension 1024, FFN 4096, 16 heads | 1.2m(cropped)/GPU | 2.7h       | 250k updates, 128 V100 * 2.3d(Librispeech)<br />600k updates, 128 V100 * 5.2d(LibriVox) |

### wav2vec-u

| Method                    | Feature Extractor | Batch Size                             | Train Time                                                   |
| ------------------------- | ----------------- | -------------------------------------- | ------------------------------------------------------------ |
| wav2vec-U                 | wav2vec 2.0 LARGE | 160 unlabeled audio + 160 text samples | 150k steps, single V100 * 12h                                |
| wav2vec-U + self training | wav2vec 2.0 LARGE | /                                      | 80k updates, 8 V100(Librispeech)<br />13k updates, 4V100(TIMIT) |

### HuBERT
