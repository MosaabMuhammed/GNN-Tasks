# GNN-Tasks
This repository contains examples of two graph neural network (GNN) tasks implemented using `PyTorch`, `PyTorch Lightning`, and `PyTorch Geometric`. The first example is a node-level classification task, and the second example is a graph-level classification task. The code is based on the PyTorch Geometric documentation and examples.

## Table of Contents
- Background
- Setup
- Tasks
- Contributing
- License


## Background
Graph neural networks (GNNs) are a type of neural network designed to handle graph-structured data. They have shown great success in a variety of tasks, such as node classification, link prediction, and graph classification. This repository provides examples of two common types of GNN tasks: node-level classification and graph-level classification.

The node-level classification task involves predicting the label of each node in a graph given its features and the graph structure. The graph-level classification task involves predicting the label of an entire graph given its features and structure.

## Setup
To run the code in this repository, you will need to have the following dependencies installed:

- Python 3
- PyTorch
- PyTorch Geometric
- PyTorch Lightning

## Tasks
### Node-Level Classification
In the node-level classification example, I used the Cora dataset, a citation network among papers.

The Cora consists of 2,708 scientific publications with links between each other representing the citation of one paper by another.

The task is to classify each publication into one of seven classes.

Each publication is represented by a bag-of-words vector. This means we have a vector of 1433 elements for each publication, where a 1 at feature i indicates that the i-th word of pre-defined dictionary is in the article.

The code for this example is contained in the `Semi_Supervised_Node_Classification.ipynb` file.

### Graph-Level Classification
The goal of graph classification is to classify an entire graph instead of single nodes or edges. Therefore, we are also given a dataset of multiple graphs that we need to classify based on some structural graph properties.

The most common task for graph classification is molecular property prediction, in which molcules are represented as graphs.

Each atom is lined to a node, and edges in the graph are the bonds between atoms.

The code for this example is contained in the `Graph_Classification.ipynb` file.

## Contributing
Contributions to this repository are welcome! If you find a bug or have an idea for an improvement, please open an issue or submit a pull request.

## License
This repository is licensed under the MIT License. See the LICENSE file for more information.
