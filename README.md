# Multi-Label Relation-Extraction
### AdaElectra — Adaptive pooling based approach with Electra model for Multi Label Relation Classification

In this project, I present an <i>Adaptive pooling based method on top of Electra model — AdaElectra </i> in order to classify relations. The proposed model — AdaElectra achieves F1 score of <b>0.88 </b> on the NYT29 dataset

The complete documentation of the project can be found [here](https://github.com/Aditya-shahh/Multi-Label-Relation-Extraction/blob/main/Relation%20Extraction.pdf)

### Dataset

In this project, I use the NYT29 dataset. This dataset is derived from the New York Times dataset. It has 29 relation types which are shown in the ```relation.txt``` file. We have splited the whole dataset into training (63,306 sentences with 78,973 relation tuples), development (7,033
sentences) and test (4,006 sentences and 5,859 relation tuples) sets. 

Each set consists of a ```.sent``` file containing all source sentences, and a ```.tup``` file indicating the relation tuples from each of the
source sentence. Each sentence comes with one or more relation tuples in the form of <i>(entity 1; entity 2;relation)</i>.  Multiple tuples are separated with |.

A sample sentence and its corresponding relation tuples are shown below: <br>

<b>Sentence:</b> then terrorism struck again , this time in the indonesia capital of jakarta. <br>
<b>Relation Tuples </b>(separated by |): <br>
jakarta ; indonesia ; /location/administrative division/country | indonesia ; jakarta ; /location/country/capital | indonesia ; jakarta ; /location/country/administrative divisions

Given all the entity pairs, the task is to classify each pair of entities of a sentence to a particular relation type or other (indicating
no relation between the two entity mentions).


### Code
The source code for this project can be found at ```Relation Classification.ipynb```. 

