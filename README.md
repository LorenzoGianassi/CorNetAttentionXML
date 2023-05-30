# CorNetAttentionXML

## Table of Contents  
- [About the Project](#1)  
- [Built with](#2)
- [Implementation](#3)
  - [Baselines](#4)

# About the Project <a name="1"/>
![](images/kmeans.png) <br/>
This is a Pytorch implementation of the paper  "[Correlation Networks for Extreme Multi-label Text Classification](https://www.semanticscholar.org/paper/Correlation-Networks-for-Extreme-Multi-label-Text-Xun-Jha/2528e161a0e2d4bdb2b0482ec5866a3914d0758b)" by *Guangxu Xun, Kishlay Jha, Jianhui Sun, Aidong Zhang*.

This project develops the **Correlation Networks** (_CorNet_) architecture for the **extreme multi-label text classification** (_XMTC_) task, where the objective is to tag an input text sequence with the most relevant subset of labels from an extremely large label set. XMTC can be found in many real-world applications, such as document tagging and product annotation.

Recently, deep learning models have achieved outstanding performances in XMTC tasks. However, these deep XMTC models ignore the useful correlation information among different labels. CorNet addresses this limitation by adding an extra CorNet module at the prediction layer of a deep model, which is able to learn label correlations, enhance raw label predictions with correlation knowledge and output augmented label predictions.

The goal of this project is to replicate the results obtained from a specific model among those shown in the paper mentioned above, specifically the **CorNetAttentionXML**, which represents an implementation of the Deep Model **AttentionXML** with the addition of the CorNet module in the hope of improving the performance.

# Built with <a name="2"/>
The project was implemented with a google colab given the need to use a good quality GPU.

Furthermore, it will not be necessary to go and download any of the libraries used in the code, since they are managed by the colab itself.

# Implementation <a name="3"/>
Within the project, two different datasets were used which differ on dimensionality:

- One medium-scale dataset: [AmazonCat-13k](https://drive.google.com/file/d/11Gfs4sazeV6u_lhC0Iw_cvC9-kK9KiXf/view)
- One small-scale dataset: [EUR-Lex](https://drive.google.com/file/d/15WSOexahaC-5kIcraYReFXR84TSuTejc/view)

## Baselines <a name="4"/>
This implementation is based on the work by [XunGuangxu](https://github.com/XunGuangxu) and the codes for the baseline model is adapted from the following repository available [here](https://github.com/XunGuangxu/CorNet).

# Authors
- **Lorenzo Gianassi**
# Acknowledgments
Machine Learning Project © Course held by Professor [Paolo Frasconi](https://www.unifi.it/p-doc2-2016-200006-F-3f2a3d2f332b2c-0.html) - Computer Engineering Master Degree @[University of Florence](https://www.unifi.it/changelang-eng.html)
