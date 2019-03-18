# Glyph-based-Chinese-Character-Embedding
This is the research project on glyph-based Chinese character embedding. Preparing for EMNLP 2019.<br><br>

This work idea is based on a recent paper https://arxiv.org/abs/1901.10125. In this paper, a CNN model is used to learn glyph-level features of Chinese characters and forced to embed glyphs into the semantic vector space. However, its model architecture is not fully utilizing the rich information enclosed in Chinese character glyphs, as its auxilliary objective is set as a pure image classification task.<br><br>

In our project, we propose to design three tailored auxilliary objectives that specifically aim at respectively extracting graphical, semantical and phonetical features from glyphs. These three tasks are: 1) radical and stroke decomposition task, 2) character definition prediction task, and 3) initial/final prediction task. To enable parameter sharing and reduce overfitting, we also propose to add a multi-headed attention layer on top of the CNN model. This is similar to the idea of multi-task learning.
