---
title: "Knowledge Graphs"
excerpt: "Implemented graph neural network (GNNs) models including TransE, ComplEx and RotatE for triple
prediction in knowledge graphs and evaluated them on Hits@K, Mean Rank (MR) and Mean
Reciprocal Rank (MRR) metrics.<br/>"
collection: portfolio
---

“The Beatles were from Manchester!!” your friend exclaims, contradicting your Liverpudlian beliefs, as “Hey Jude!” comes on the radio. You get into an argument about where the Beatles were from, trying to prove that they were from Liverpool. But fortunately, it’s not ’99 and you can pull your phone out and ask Google “Where were the Beatles from?”, proving you right and leaving factual uncertainty to be a thing of the past.

But how did Google know the answer? To resolve such conflicts between you and your friends, Google converts information on the internet into graphs of facts aka knowledge graphs. For example, the relevant information that “The Beatles were from Liverpool” is encoded as a graph with the two entities “Beatles” and “Liverpool” as nodes and the relation “were from” as a directed edge between them.

When asked, where the Beatles were from, Google looks at the node for “ The Beatles” and traverses the relational edge “were from” to reach the entity node “Liverpool” to give you an answer. Such graphs are commonly used to represent a wide range of information like:

1. Factual information about the world. (The Beatles, were from, Liverpool), 
2. Biological information like drugs, their side effects and symptoms (Ibuprofen reduces inflammation)
3. Relationships between words in language like synonyms and antonyms (beautiful is a synonym of gorgeous)

Once a graph is fully constructed, it can be used to answer a variety of queries like “Which bands were from the same place as the Beatles?” (Pink Floyd for instance). Unfortunately, knowledge graphs are not complete, several relations are usually missing.

Completing a knowledge graph, and predicting missing relations is an open challenge. I explore some ways to tackle the challenge. 

[Project](https://github.com/A0308/Knowledge-Graph-Completion)