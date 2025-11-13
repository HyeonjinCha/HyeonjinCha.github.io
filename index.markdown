---
layout: default
title: "Content-Aware Style Augmentation for Zero-shot Voice Conversion with Short Target Speech"
---

## Content-Aware Style Augmentation for Zero-shot Voice Conversion with Short Target Speech

### Authors
Hyeonjin Cha, Seyun Um, Miseul Kim, Changhwan Kim, Seungshin Lee and Hong-Goo Kang

### Proposed Method
![inference image](/assets/images/inference.jpg)

In this letter, we propose a neural zero-shot voice conversion (ZS-VC) system that simultaneously achieves high speaker similarity and speech intelligibility by incorporating a content-aware style generation module. 
Although recent neural ZS-VC systems have shown strong performance in either speaker similarity or speech intelligibility, attaining high performance in both remains challenging, especially when only a short target speech sample is available. 
We attribute this limitation to the *insufficient content problem*---where the linguistic content of the target speech fails to fully cover that of the source speech.
To address this issue, we introduce a method that augments the target speaker's style features for underrepresented content using self-supervised feature generation. 
Experimental results demonstrate that the proposed system, when integrated with the feature matching-based approach kNN-VC, outperforms existing methods in both key metrics.



### Samples
**Baseline**: kNN-VC, Phoneme Hallucinator (PH)

#### Female to female

| Source | Target (2 sec) | kNN-VC | PH | Proposed |
| ------ | ------ | ------ | --- | -------- |
| <audio controls><source src="/assets/audio/Female_to_female/F4970_src.wav" type="audio/wav"></audio> | <audio controls><source src="/assets/audio/Female_to_female/F5142_trg.wav" type="audio/wav"></audio> | <audio controls><source src="/assets/audio/Female_to_female/F4970_F5142_knn.wav" type="audio/wav"></audio> | <audio controls><source src="/assets/audio/Female_to_female/F4970_F5142_ph.wav" type="audio/wav"></audio> | <audio controls><source src="/assets/audio/Female_to_female/F4970_F5142_casa.wav" type="audio/wav"></audio> |
| ------ | ------ | ------ | --- | -------- |
| <audio controls><source src="/assets/audio/Female_to_female/F5142_src.wav" type="audio/wav"></audio> | <audio controls><source src="/assets/audio/Female_to_female/F5683_trg.wav" type="audio/wav"></audio> | <audio controls><source src="/assets/audio/Female_to_female/F5142_F5683_knn.wav" type="audio/wav"></audio> | <audio controls><source src="/assets/audio/Female_to_female/F5142_F5683_ph.wav" type="audio/wav"></audio> | <audio controls><source src="/assets/audio/Female_to_female/F5142_F5683_casa.wav" type="audio/wav"></audio> |

#### Male to female

| Source | Target (2sec) | kNN-VC | PH | Proposed |
| ------ | ------ | ------ | --- | -------- |
| <audio controls><source src="/assets/audio/Male_to_female/M1089_src.wav" type="audio/wav"></audio> | <audio controls><source src="/assets/audio/Male_to_female/F1580_trg.wav" type="audio/wav"></audio> | <audio controls><source src="/assets/audio/Male_to_female/M1089_F1580_knn.wav" type="audio/wav"></audio> | <audio controls><source src="/assets/audio/Male_to_female/M1089_F1580_ph.wav" type="audio/wav"></audio> | <audio controls><source src="/assets/audio/Male_to_female/M1089_F1580_casa.wav" type="audio/wav"></audio> |
| ------ | ------ | ------ | --- | -------- |
| <audio controls><source src="/assets/audio/Male_to_female/M7729_src.wav" type="audio/wav"></audio> | <audio controls><source src="/assets/audio/Male_to_female/F5683_trg.wav" type="audio/wav"></audio> | <audio controls><source src="/assets/audio/Male_to_female/M7729_F5683_knn.wav" type="audio/wav"></audio> | <audio controls><source src="/assets/audio/Male_to_female/M7729_F5683_ph.wav" type="audio/wav"></audio> | <audio controls><source src="/assets/audio/Male_to_female/M7729_F5683_casa.wav" type="audio/wav"></audio> |

#### Female to male

| Source | Target (2sec) | kNN-VC | PH | Proposed |
| ------ | ------ | ------ | --- | -------- |
| <audio controls><source src="/assets/audio/Female_to_male/F1580_src.wav" type="audio/wav"></audio> | <audio controls><source src="/assets/audio/Female_to_male/M1089_trg.wav" type="audio/wav"></audio> | <audio controls><source src="/assets/audio/Female_to_male/F1580_M1089_knn.wav" type="audio/wav"></audio> | <audio controls><source src="/assets/audio/Female_to_male/F1580_M1089_ph.wav" type="audio/wav"></audio> | <audio controls><source src="/assets/audio/Female_to_male/F1580_M1089_casa.wav" type="audio/wav"></audio> |
| ------ | ------ | ------ | --- | -------- |
| <audio controls><source src="/assets/audio/Female_to_male/F1995_src.wav" type="audio/wav"></audio> | <audio controls><source src="/assets/audio/Female_to_male/M2300_trg.wav" type="audio/wav"></audio> | <audio controls><source src="/assets/audio/Female_to_male/F1995_M2300_knn.wav" type="audio/wav"></audio> | <audio controls><source src="/assets/audio/Female_to_male/F1995_M2300_ph.wav" type="audio/wav"></audio> | <audio controls><source src="/assets/audio/Female_to_male/F1995_M2300_casa.wav" type="audio/wav"></audio> |

#### Male to male

| Source | Target (2sec) | kNN-VC | PH | Proposed |
| ------ | ------ | ------ | --- | -------- |
| <audio controls><source src="/assets/audio/Male_to_male/M7021_src.wav" type="audio/wav"></audio> | <audio controls><source src="/assets/audio/Male_to_male/M7127_trg.wav" type="audio/wav"></audio> | <audio controls><source src="/assets/audio/Male_to_male/M7021_M7127_knn.wav" type="audio/wav"></audio> | <audio controls><source src="/assets/audio/Male_to_male/M7021_M7127_ph.wav" type="audio/wav"></audio> | <audio controls><source src="/assets/audio/Male_to_male/M7021_M7127_casa.wav" type="audio/wav"></audio> |
| ------ | ------ | ------ | --- | -------- |
| <audio controls><source src="/assets/audio/Male_to_male/M8230_src.wav" type="audio/wav"></audio> | <audio controls><source src="/assets/audio/Male_to_male/M8455_trg.wav" type="audio/wav"></audio> | <audio controls><source src="/assets/audio/Male_to_male/M8230_M8455_knn.wav" type="audio/wav"></audio> | <audio controls><source src="/assets/audio/Male_to_male/M8230_M8455_ph.wav" type="audio/wav"></audio> | <audio controls><source src="/assets/audio/Male_to_male/M8230_M8455_casa.wav" type="audio/wav"></audio> |
