---
title: 'Spectral Clusterng Basics'
date: 2018-12-21
permalink: /posts/2018/12/spectral_clustering_basics/
tags:
  - Clustering, ML
  - ML
  - Clustering
---

This is the second part of the multiple blogs on Spectral Clustering. Following are the links to all the parts of this series.  
  
1. Spectral Clustering - Intro
2. Spectral Clustering - Basic Ideas  
3.  
  
**Spectral Clustering - Basic Concepts**  
 
The data can be represented in different ways. Tabular data and graph data are common ways to represent the data.
- _Tabular data:_  The data is organized into tables. Each table having a specific format arranged in fixed number of columns.
- _Graph Data:_  Graph representation of the data involves organization of data in the form of nodes and edges. Where nodes store the information or the property while the edges represent the relationship between the nodes.

_Graph_

A graph consists of a set of nodes(V) and a set of edges(E) to represent the relation between the nodes.

[![](https://2.bp.blogspot.com/-VUCu8exYqSo/XByuCbB9GAI/AAAAAAAAYaQ/VEC9IzKhfq0gJEcKo55-ifA701Lc-y3hQCLcBGAs/s320/example%2Bgraph.png)](https://2.bp.blogspot.com/-VUCu8exYqSo/XByuCbB9GAI/AAAAAAAAYaQ/VEC9IzKhfq0gJEcKo55-ifA701Lc-y3hQCLcBGAs/s1600/example%2Bgraph.png)

Fig 1. Example graph with 5 vertices and 5 edges

```
G = {V, E}

V = {v1, v2, v3, v4, v5, v6, …}

E = {e1, e2, e3, e4, e5, …}
```
 
Where, V is a set of vertices and E is a set of edges.

_Common Terminologies_
The common terminologies and concepts which will be applicable in spectral clustering are,

_Adjacency Matrix(W):_ A graph can be represented as a two-dimensional array of size V x V, where V is a number of vertices. Both rows and columns of the adjacency are labeled by the vertices hence making it a square matrix and symmetric. The element (wij) of the adjacency matrix indicate whether the two vertices are adjacent (connected by a common edge.) or not. The example graph shown in fig 1. can be represented as an Adjacency Matrix as below.

[![](https://2.bp.blogspot.com/-Z0L9rb80LJI/XByuX11xK2I/AAAAAAAAYaY/TrzwRf5Z6nsPNIl2DEkC6yEmR1X05b_9wCLcBGAs/s320/adjacency%2Bmatrix.png)](https://2.bp.blogspot.com/-Z0L9rb80LJI/XByuX11xK2I/AAAAAAAAYaY/TrzwRf5Z6nsPNIl2DEkC6yEmR1X05b_9wCLcBGAs/s1600/adjacency%2Bmatrix.png)

Fig 2. Adjacency Matrix for the example graph in fig 1

_Degree of a vertex(di):_  Degree of a vertex is the number of edges that touch the vertex. For example, in the example graph above. The degree of vertex v1 is 2. The degree of a vertex is the sum of the elements of a row or a column of an adjacency matrix corresponding to the vertex.
```
di = w11 + w12 + w13+ w14 …….
```


[![](https://2.bp.blogspot.com/-zVwm5P9nzN4/XByvXoUCnaI/AAAAAAAAYak/Kd6Ztvfj8o8eiGWVee3i3FHt34zNDKkWwCLcBGAs/s640/degree%2Bof%2Bvertex.png)](https://2.bp.blogspot.com/-zVwm5P9nzN4/XByvXoUCnaI/AAAAAAAAYak/Kd6Ztvfj8o8eiGWVee3i3FHt34zNDKkWwCLcBGAs/s1600/degree%2Bof%2Bvertex.png)

  

Fig 3. Degree of vertices of the example graph shown above.

  

_Degree Matrix(D):_  A degree matrix is a diagonal matrix with the information about the degree of the vertices. The size of the matrix is also VxV.

  

[![](https://2.bp.blogspot.com/-wQVj-yjIoms/XByvqQ9-FnI/AAAAAAAAYas/5neSFNpjgWAlFUEF4W0LsuNRqhRCwbEFQCLcBGAs/s320/degreematrix.png)](https://2.bp.blogspot.com/-wQVj-yjIoms/XByvqQ9-FnI/AAAAAAAAYas/5neSFNpjgWAlFUEF4W0LsuNRqhRCwbEFQCLcBGAs/s1600/degreematrix.png)

Fig. 4 Degree Matrix

_Laplacian Matrix (L)_: A Laplacian of a graph is given by the D – W, where D is a diagonal matrix formed from the vertex degrees and W is an adjacency matrix.


These are the basic concepts of Graph theory applicable to Spectral Clustering.

I will next write about the Spectral Clustering in the next Part of this blog series.
