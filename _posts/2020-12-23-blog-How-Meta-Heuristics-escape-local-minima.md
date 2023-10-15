---
title: 'How Meta-Heuristics can escape Local Minima'
collection: posts
permalink: /posts/2020/12/blog-post-How-Meta-Heuristics-escape-local-minima/
excerpt: ''
venue: ''
paperurl: ''
authors: 'Umberto Junior Mele'
year: '(2020)'
journal: ''
paged: ''
citation: ''
date: 2020-12-23
tags:
  - Meta-Heuristics
  - Local Search
  - Constructive Algorithms
---

<div align="center">
    <img src="/images/localsearchAI.png" alt="AI local searching for better solutions">
</div>


Local search algorithms are powerful approaches that allows to continously improve the current solution by applying small changes to the solution that always lead to a better solutions in terms of objective function.
The 2-opt is a simple example of these local searches, where the process consists in exchanging 2 edges in the current solution with two edges that are not currently in the solution. This move is applied only if the exchange leads to an improvement in terms of cost.
Therefore, how is shown in the image below exchanges are operated just when they lead to un improvement of the tour, for example when two crossing edges should be removed.

<div align="center">
    <img src="/images/Two-Opt-operation.png" alt="2-opt move example">
</div>


The Traveling Salesman Problem (TSP) stands as one of the most studied and iconic optimization problems in the realm of combinatorial optimization. Formally defined, the TSP seeks the shortest possible route that visits each city exactly once and returns to the original city. As a member of the NP-hard class of problems, the TSP is renowned for its computational complexity, particularly when the number of cities (or nodes) increases. The quest for efficient solutions has engendered the development of myriad heuristics and exact algorithms.

Within this vast landscape, the Lin-Kernighan heuristic emerges as a particularly notable local search algorithm for the TSP. Introduced by Shen Lin and Brian Kernighan in 1973, this heuristic constitutes an improvement over simpler methods, such as the 2-opt and 3-opt procedures, by exploring a broader set of potential exchanges to enhance a given tour.

The core philosophy underpinning the Lin-Kernighan heuristic is the idea that optimal or near-optimal solutions for the TSP can be found by making a series of incremental improvements to a given tour. To achieve this, the algorithm commences with an initial solution and attempts to refine it through a sequence of k-opt moves, where k>2. The essence of a k-opt move is the identification and exchange of k links in the current tour to achieve a reduction in tour length.

While, at a glance, it may seem akin to the 2-opt or 3-opt procedures, the Lin-Kernighan heuristic boasts a dynamic approach. Rather than being confined to a fixed k value, it systematically varies the value of k during its search process, allowing for a deeper and more nuanced exploration of the solution space.

In this blog, we will embark on a detailed exploration of the Lin-Kernighan heuristic, unraveling its intricacies and mechanics. Through illustrative examples and computational analyses, we will underscore its effectiveness in delivering high-quality solutions for the TSP, elucidating why it continues to be regarded as one of the preeminent heuristics in the field.

Join us as we navigate the captivating realm of TSP and delve deep into the nuances of the Lin-Kernighan heuristic, a testament to the innovative thinking of its creators and a cornerstone in the world of combinatorial optimization.

