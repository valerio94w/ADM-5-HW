# ADM-HW5

# Homework 5 - Visit the Wikipedia hyperlinks graph!

In this assignment, we perform an analysis of the Wikipedia Hyperlink graph. In particular, given extra information about the categories to which an article belongs to, we are curious to rank the articles according to some criteria.

For this purpose, we use the Wikipedia graph released by the SNAP group, but the reduced version.

More details about the task on the following [link](https://github.com/CriMenghini/ADM-2018/blob/master/Homework_5/README.md).

![snap graph](http://yifanhu.net/GALLERY/GRAPHS/GIF_SMALL/SNAP@as-735.gif)


1. First, we have downloaded  [Wikicat hyperlink graph data](https://drive.google.com/file/d/1ghPJ4g6XMCUDFQ2JPqAVveLyytG8gBfL/view?usp=sharing).  It is a reduced version of the one on SNAP. Every row is an edge, the two elements are the nodes (source and destination).
2.  From [this](https://snap.stanford.edu/data/wiki-topcats.html) page we downloaded:
	-  `wiki-topcats-categories.txt.gz` (the list of the articles which belong to each category)
	-  `wiki-topcats-page-names.txt.gz` (the names of the articles and its identification number)

The main goal was to answer the following research questions:

[RQ1] Build the graph [G=(V, E)] , where V is the set of articles and E the hyperlinks among them, and provide its basic information:

* If it is direct or not
* The number of nodes
* The number of edges
* The average node degree. Is the graph dense?

[RQ2]

1. Building Block Ranking
    > Based on the implementation of the **shortest path** algorithm( **Breadth First Search** algorithm) compare sample number of nodes of C0-input category with all nodes in all the other Ci categories in order to build the **block ranking**. 

2. Ranking nodes of each category in the created block ranking vector and selecting top 3 and finding article names for it

## The repository contains the following files:

1. __`Homework 5 - RQ1 pre-check up.ipynb`__:
      > In this notebook, we decided to put just the exploration of research question 1 and the conclusions we made. Based on that we can use the right networkx method in the making of a graph and to double check the results and conclusions we made.
      
2. __`Homework 5 - RQ1 and RQ2.ipynb`__:
      > A notebook with all the steps: reading data and making of a graph, calculating short distance paths, building block ranking and ranking nodes of each category.


## Authors are:

*  **Dusica Stepic** 
*  **Valerio Antonini**
