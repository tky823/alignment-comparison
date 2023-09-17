---
title: A COMPARATIVE STUDY OF TEXT-SPEECH ALIGNMENT METHODS FOR EMOTIONAL SPEECH SYNTHESIS
layout: default
---

# Authors

Takuya Hasumi, Yuma Shirahata, Ryuichi Yamamoto, Welly Naptali,
Eunwoo Song, Kentaro Tachibana, Jae-Min Kim

# Abstract

In this paper, we investigate the performance of various text-speech alignment methods to build a high-quality emotional parallel text-to-speech (TTS) system. Generally, there are three types of strategies to obtain alignments between the recordings and the corresponding transcriptions: 1) Manual annotation of alignment by experts. 2) Estimation of alignment by an external text-speech aligner. 3) Acquisition of alignment through unsupervised alignment learning. Although the comparison of these methods has been performed on reading-style speech datasets in some previous works, their performance on emotional speech synthesis, where the dataset has a wide variety of pronunciation and prosody, has not been thoroughly investigated. To shed light on this matter, we conduct a comprehensive study on text-speech alignment strategies from both objective and subjective criteria on emotional TTS tasks. In addition, we further propose a semi-supervised alignment learning approach as one of the comparison methods. In this approach, the alignment module is pre-trained with a small amount of annotated data and then fine-tuned with a large amount of unannotated data. Main findings from experimental results include that the semi-supervised approach, which uses only 4% of annotated data, significantly improves the training stability of the unsupervised approach. Moreover, it achieves comparable performance to a model that employs fully annotated duration labels and the alignments extracted from a strong external forced aligner.

# Audio Samples

## Neutral Style

| Model | Sample 1 (Female) | Sample 2 (Male) |
|:-:|:-:|:-:|
| Reference | <audio controls src="samples/Reference/neutral/fkdo04979.wav"></audio> | <audio controls src="samples/Reference/neutral/mksk04983.wav"></audio> |
| Period-VITS (manual) | <audio controls src="samples/Period-VITS_manual/neutral/fkdo04979.wav"></audio> | <audio controls src="samples/Period-VITS_manual/neutral/mksk04983.wav"></audio> |
| Period-VITS (external) | <audio controls src="samples/Period-VITS_external/neutral/fkdo04979.wav"></audio> | <audio controls src="samples/Period-VITS_external/neutral/mksk04983.wav"></audio> |
| Semi-Period-VITS | <audio controls src="samples/Semi-RAD-Period-VITS/neutral/fkdo04979.wav"></audio> | <audio controls src="samples/Semi-RAD-Period-VITS/neutral/mksk04983.wav"></audio> |
| Un-Period-VITS | <audio controls src="samples/RAD-Period-VITS/neutral/fkdo04979.wav"></audio> | <audio controls src="samples/RAD-Period-VITS/neutral/mksk04983.wav"></audio> |

## Happiness Style

| Model | Sample 1 (Female) | Sample 2 (Male) |
|:-:|:-:|:-:|
| Reference | <audio controls src="samples/Reference/happy/fkdo41271.wav"></audio> | <audio controls src="samples/Reference/happy/mksk41204.wav"></audio> |
| Period-VITS (manual) | <audio controls src="samples/Period-VITS_manual/happy/fkdo41271.wav"></audio> | <audio controls src="samples/Period-VITS_manual/happy/mksk41204.wav"></audio> |
| Period-VITS (external) | <audio controls src="samples/Period-VITS_external/happy/fkdo41271.wav"></audio> | <audio controls src="samples/Period-VITS_external/happy/mksk41204.wav"></audio> |
| Semi-Period-VITS | <audio controls src="samples/Semi-RAD-Period-VITS/happy/fkdo41271.wav"></audio> | <audio controls src="samples/Semi-RAD-Period-VITS/happy/mksk41204.wav"></audio> |
| Un-Period-VITS | <audio controls src="samples/RAD-Period-VITS/happy/fkdo41271.wav"></audio> | <audio controls src="samples/RAD-Period-VITS/happy/mksk41204.wav"></audio> |

## Sadness Style

| Model | Sample 1 (Female) | Sample 2 (Male) |
|:-:|:-:|:-:|
| Reference | <audio controls src="samples/Reference/sad/fkdo51172.wav"></audio> | <audio controls src="samples/Reference/sad/mksk51196.wav"></audio> |
| Period-VITS (manual) | <audio controls src="samples/Period-VITS_manual/sad/fkdo51172.wav"></audio> | <audio controls src="samples/Period-VITS_manual/sad/mksk51196.wav"></audio> |
| Period-VITS (external) | <audio controls src="samples/Period-VITS_external/sad/fkdo51172.wav"></audio> | <audio controls src="samples/Period-VITS_external/sad/mksk51196.wav"></audio> |
| Semi-Period-VITS | <audio controls src="samples/Semi-RAD-Period-VITS/sad/fkdo51172.wav"></audio> | <audio controls src="samples/Semi-RAD-Period-VITS/sad/mksk51196.wav"></audio> |
| Un-Period-VITS | <audio controls src="samples/RAD-Period-VITS/sad/fkdo51172.wav"></audio> | <audio controls src="samples/RAD-Period-VITS/sad/mksk51196.wav"></audio> |

# References

- [1] Y. Shirahata, et al., "Period VITS: Variational inference with explicit pitch modeling for end-to-end emotional speech synthesis," in **Proc. ICASSP**, 2023, pp.1-5.
- [2] K. J. Shih, et al., "RAD-TTS: Parallel frlo-based TTS with robust alignment learning and diverse synthesis.", in **ICML workshop**, 2021.
