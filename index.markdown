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
We attribute this limitation to the \textit{insufficient content problem}---where the linguistic content of the target speech fails to fully cover that of the source speech.
To address this issue, we introduce a method that augments the target speaker's style features for underrepresented content using self-supervised feature generation. 
Experimental results demonstrate that the proposed system, when integrated with the feature matching-based approach kNN-VC, outperforms existing methods in both key metrics.

### 샘플 오디오

아래 오디오를 재생해 보세요:

<audio controls>
  <source src="/assets/audio/sample.wav" type="audio/wav">
  Your browser does not support the audio element.
</audio>
