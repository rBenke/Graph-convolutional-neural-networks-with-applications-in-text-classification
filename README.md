# Graph convolutional neural networks with applications in text classification.
> Master thesis repository

## Table of contents
* [BBC text categorization](#BBC)
* [Graph Convolutional Network](#GCN)
* [TextGCN](#TextGCN)
* [DocumentGCN](#DocumentGCN)
* [Resuls](#Results)
* [Repository description](#Repository-description)
## BBC text categorization
>Text documents are one of the richest sources of data for businesses.
>
>We’ll use a public dataset from the BBC comprised of 2225 articles, each labeled under one of 5 categories: business, entertainment, politics, sport or tech.
>
>The dataset is broken into 1490 records for training and 735 for testing. The goal will be to build a system that can accurately classify previously unseen news >articles into the right category.
>
>The competition is evaluated using Accuracy as a metric.

## Graph Convolutional Network

## TextGCN
![TextGCN](img/TextGCN.png)

## DocumentGCN
![DocumentGCN](img/DocumentGCN.png)

## Resuls

| Model        | Accuracy (%) | Learning Time (s)  |
|:------------:|:------------:|:------------------:|
| DocumentGCN  |  **98.6**    |     195.95         |
| TextGCN      |    48.4      |     336.73         |
|              |              |                    |
| BERT         |    97.3      |     2045.0         |
| BiLSTM       |    95.0      |     3266.0         |
| NaiveBayes   |    96.4      |   **0.0038**       | 

## Repository description


## Contact
Created by [Robert Benke](https://www.linkedin.com/in/robert-benke-396b56175/) - feel free to contact me!
