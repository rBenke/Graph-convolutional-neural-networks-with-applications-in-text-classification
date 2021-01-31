# Graph convolutional neural networks with applications in text classification.
> Master thesis repository

## Table of contents
* [BBC text categorization](#BBC)
* [Graph Convolutional Network](#GCN)
* [TextGCN](#TextGCN)
* [DocumentGCN](#DocumentGCN)
* [Results](#Results)
* [Repository description](#Repository-description)
## BBC text categorization
>Text documents are one of the richest sources of data for businesses.
>
>We’ll use a public dataset from the BBC comprised of 2225 articles, each labeled under one of 5 categories: business, entertainment, politics, sport or tech.
>
>The dataset is broken into 1490 records for training and 735 for testing. The goal will be to build a system that can accurately classify previously unseen news articles into the right category.
>
>The competition is evaluated using Accuracy as a metric.

## Graph Convolutional Network

## TextGCN
![TextGCN](img/TextGCN.png)

## DocumentGCN
![DocumentGCN](img/DocumentGCN.png)

## Results

| Model        | Accuracy (%) | Learning Time (s)  |
|:------------:|:------------:|:------------------:|
| DocumentGCN  |  **98.6**    |     195.95         |
| TextGCN      |    48.4      |     336.73         |
|              |              |                    |
| BERT         |    97.3      |     2045.0         |
| BiLSTM       |    95.0      |     3266.0         |
| NaiveBayes   |    96.4      |   **0.0038**       | 

## Repository description
Steps for reproducing the results:
* run the data/load_raw_data.ipynb -- it will create a feather file with all the documents in single dataframe and download the word2vec model.
* TextGCN:
    * prepare the heterogenous word-document graph for the whole corpus with TextGCN/text2graph.ipynb
    * learn the model and make predictions with TextGCN/TextGCN.ipynb
* DocumentGCN
    * prepare the graph for every document in the corpus with DocumentGCN/text2graphs.ipynb
    * learn the model and make predictions with DocumentGCN/DocumentGCN.ipynb
* Non-graph-oriented models are contained in the NB&DNN folder.

## Contact
Created by [Robert Benke](https://www.linkedin.com/in/robert-benke-396b56175/) - feel free to contact me!
