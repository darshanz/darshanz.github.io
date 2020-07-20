---
title: 'Spectral Clustering - Intro'
date: 2018-12-20
permalink: /posts/2018/12/spectral_clustring_intro/
tags:
  - clustering, ML, graph
  - ML
  - Clustering
---

This is the first part of the multiple blogs on Spectral Clustering. I will write a few blogs related to basic concepts in Spectral clustering in this series. Below are the links to all the parts of this series.  
  

 1. Spectral Clustering - Intro  
 2.  Spectral Clustering - Basic Ideas

 
**1. Spectral Clustering - Intro**  
  

To start with spectral clustering, let’s first see what clustering is.

Clustering is a technique used for automatically grouping the data-points into a number of clusters based on their similarity so that less similar points fall under different clusters.

Clustering is basically done by grouping the points into clusters based on some distance measure, so that the points in same cluster have a small distance from one another. However, proximity is not always the relationship between the data points. Sometimes geometrical relation is also important. Spectral clustering is based on such relationships.

_How does spectral clustering fit into the world of machine learning?_

Firstly, machine learning techniques are broadly classified into supervised and unsupervised (of course there is semi-supervised too, but let’s not go into that now) machine learning. To put it simply, supervised learning involves the use of labeled training data and the unsupervised learning deals with the unlabeled data.

Clustering is an unsupervised technique. Among the most popular clustering techniques, we have K-means, Gaussian Mixture Model, Expectation Maximization(EM), Spectral Clustering etc.

Yes, that where Spectral Clustering lies in the big picture. Spectral clustering is performed in Graph Data.

In next blog, I will try to write something about the Graph Theory and Basic ideas needed before jumping into theory of Spectral clustering.
