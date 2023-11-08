---
title: "Predicting Drug Interactions with Graph Neural Networks:"
excerpt: "Used the Graph Isomorphism Network on the ogbl-ddi
dataset for drug-drug interactions and evaluated them on best val Hits@20 score over 2 runs"
collection: portfolio
---

To investigate drug-drug interactions, I have applied graph ML techniques to the ogbl-ddi dataset, a homogeneous, unweighted, and undirected graph representing a drug-drug interaction network. This graph contains 4,267 nodes and 1,334,889 edges. Nodes represent FDA-approved or experimental drugs, and edges represent potential interactions between drugs.
We want to use graph structure information to predict whether two nodes (drugs) share an edge (interaction). We don’t know anything about the drugs or the nature of their interactions: we only know whether two “anonymous” drugs interact or don’t interact. Somehow, we need to generate meaningful representations for nodes in our graph: after obtaining these representations, we can feed them into a neural network to predict the existence of an edge between any 2 nodes. Ultimately, we’d like to use graph neural network methods to build the following training and prediction pipeline:

![Pipeline](./images/Pipeline.png)