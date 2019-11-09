# Hierarchical Multi-Label Text Classification

This repository is my research project, and it is accepted by CIKM'19.

The main objective of the project is to solve the hierarchical multi-label text classification (**HMTC**) problem. Different from the multi-label text classification, HMTC assigns each instance (object) into multiple categories and these categories are stored in a hierarchy structure, is a fundamental but challenging task of numerous applications.

## Requirements

- Python 3.6
- Tensorflow 1.10 +
- Numpy
- Gensim

## Introduction

Many real-world applications organize data in a hierarchical structure, where classes are specialized into subclasses or grouped into superclasses. For example, an electronic document (e.g. web-pages, digital libraries, patents and e-mails) is associated with multiple categories and all these categories are stored hierarchically in a **tree** or **Direct Acyclic Graph (DAG)**. 

It provides an elegant way to show the characteristics of data and a multi-dimensional perspective to tackle the classification problem via hierarchy structure. 

![](https://farm8.staticflickr.com/7806/31717892987_e2e851eaaf_o.png)

The Figure shows an example of predefined labels in hierarchical multi-label classification of documents in patent texts. 

- Documents are shown as colored rectangles, labels as rounded rectangles. 
- Circles in the rounded rectangles indicate that the corresponding document has been assigned the label. 
- Arrows indicate a hierarchical structure between labels.

## Data

See data format in `data` folder which including the data sample files.

### Text Segment

You can use `jieba` package if you are going to deal with the Chinese text data.

### Data Format

This repository can be used in other datasets (text classification) in two ways:
1. Modify your datasets into the same format of the sample.
2. Modify the data preprocess code in `data_helpers.py`.

Anyway, it should depend on what your data and task are.

### Pre-trained Word Vectors

You can pre-training your word vectors(based on your corpus) in many ways:
- Use `gensim` package to pre-train data.
- Use `glove` tools to pre-train data.
- Even can use a **fasttext** network to pre-train data.

## Network Structure

![](https://live.staticflickr.com/65535/48647692206_2e5e6e7f13_o.png)

## Reference

**If you want to follow the paper or utilize the code, please note the following info in your work:** 

> @inproceedings{Huang:2019:HMT:3357384.3357885,
>
> author = {Huang, Wei and Chen, Enhong and Liu, Qi and Chen, Yuying and Huang, Zai and Liu, Yang and Zhao, Zhou and Zhang, Dan and Wang, Shijin},
>
> title = {Hierarchical Multi-label Text Classification: An Attention-based Recurrent Network Approach},
>
> booktitle = {Proceedings of the 28th ACM International Conference on Information and Knowledge Management},
>
> year = {2019},
>
> isbn = {978-1-4503-6976-3},
>
> pages = {1051--1060},
>
> numpages = {10},
>
> url = {http://doi.acm.org/10.1145/3357384.3357885},
>
> doi = {10.1145/3357384.3357885},
>
> acmid = {3357885},
>
> publisher = {ACM}
>
> } 

---

## About Me

黄威，Randolph

SCU SE Bachelor; USTC CS Master

Email: chinawolfman@hotmail.com

My Blog: [randolph.pro](http://randolph.pro)

LinkedIn: [randolph's linkedin](https://www.linkedin.com/in/randolph-%E9%BB%84%E5%A8%81/)
