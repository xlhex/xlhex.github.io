---
layout:     post
title:      "Dynamic Programming Encoding forSubword Segmentation in Neural Machine Translation"
categories: [MT]
tags:       [MT]
---

Since it was introduced in 2016 by Sennrich et al. (2016) and Schuster et al. (2012) subword representation has been popularised in the NLP field across multiple tasks such as machine translation (MT), document summarization (DS) and language modelling (LM) etc. Basically, subwords aim at addressing the out-of-vocabulary (OOV) issue. OOV has been a common problem in MT tasks, especially in neural MT (NMT) systems, due to the limited vocabulary with at most tens of thousands of entries. Concretely, OOVs can cause a significant drop in terms of translation quality, owing to the information missing within a context.

One solution to this issue is to use a fully character-level NMT (Lee et al. 2016, Cherry et al. 2018). However, character representation also suffers from two drawbacks: 1) a deeper architecture for the linguistic compositions, and 2) larger modelling latency.

Subwords sidestep the aforementioned issues through maintaining a good balance between complete words and characters. Specifically, common words will be preserved, while unseen or rare words are split into subwords. For instance, “unconscious” is segmented as “un” and “conscious”.

Byte Pair Encoding (BPE) starts from individual characters, then utilizes a compression algorithm to merge the most frequent units until reach the predefined limit, while wordpiece and unigram language model (Kudo 2017) apply language model to characters to form their subwords. These approaches can dramatically reduce the size of vocabulary to moderate volume such as 32K or 16K.

Empirically, one might notice that owing to the different merge algorithms adopted by these techniques, a word can have multiple valid segmentations as shown in figure 1. Specifically, “unconscious” can be split in: {“uncon”, “scious”}, {“un”, “con”, “scious”}, or {“un”, “conscious”}.
