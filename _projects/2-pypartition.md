---
title: "pypartition"
excerpt: "This is the code used for the paper Practical Low-Dimensional Halfspace Range Space Sampling. <br/><img src='/images/trap_cutting.png'>"
collection: projects
---
Cuttings, partition trees, Akcan sampling, and ham sandwich tree codes for generating small samples for halfspaces. This is code from the paper "Practical Low Dimensional HalfSpace Range Space Sampling". It can be used to generate partition trees like the ones from Chan's "Optimal Partition Trees". The main file is partitions.py. 

These codes are all meant for generating small sized $\varepsilon$-samples for halfspace sampling. Given a set of points $X \subset \mathbb{R}^d$ and a corresponding set of ranges $\mathcal{A} \subset 2^X$ an $\varepsilon$-sample $S$ has the property that for any range $A \in \mathcal{A}$ it is true that $\left \vert \frac{\vert X \cap A \vert}{\vert X \vert} - \frac{\vert S \cap A \vert}{ \vert S \vert} \le \varepsilon$. In other words the $\varepsilon$-sample preserves the relative density of the original sample. This is a useful property since many algorithms just need the properties given by an $\varepsilon$-sample and so given an efficient method for computing a small sized $\varepsilon$-sample we automatically get faster approximate algorithms. 

The simplest method I have implemented is also in practice the best. Ham Sandwich sampling is based on using a partitioning scheme where the Ham Sandwich theorem is repeatedly applied to find a line that cuts two sets of points in half and then applied recursively to the subsets. I have two versions of this method. Both work about the same in practice, but in theory the partitioning method on the right should be slighly better.

![Ham Sandwich](https://michaelmathen.github.io/images/hamsandwich.jpg)

In theory the Chan Partitioning method should be the best algorithm for finding a small sized $\varepsilon$-sample for halfspace sampling. This algorithm works by alternatively partitioning cells to 
balance the number of contained points or the number of crossing lines. In practice we did not find that this method performed that well, but it could be useful as a starting point for developing a more practical theory inspired algorithm. We also implemented an algorithm based on a paper by Matousek that has a similiar guarantee to Chan's algorithm. 

![Chan Partitioning](https://michaelmathen.github.io/images/Partitioning.jpg)

Chan partitioning and Matousek's algorithm both rely on computing something called a Cutting. This is a subdivision of space into constant sized cells where each cell is crossed by at most $r$ fraction of the lines and in the optimal case there are at most $O(r^d)$ cells. Our implementation of this was based on a paper by Sariel Har-Peled. We designed methods that computed either polygonal cells or trapezoidal cells. 

<div class="container-fluid">
    <div class="row equal-height">
    <div class="col-md-3 col-xs-12">

    <img src="https://michaelmathen.github.io/images/poly.png" class="img-responsive center-block">
            <div class="caption text-center">
            <h6>Polygonal Cutting</h6>
            </div>
   </div>
  
    <div class="col-md-3 col-xs-12">
            <img src="https://michaelmathen.github.io/images/trap_cutting.png" class="img-responsive center-block">
            <div class="caption text-center">
            <h6>Trapezoidal Cutting</h6>
            </div>
    </div>
  </div>
</div>


