---
title: "A New Constructive heuristic driven by Machine Learning for the Traveling Salesman Problem"
collection: publications
permalink: /publication/2021-paper-A-New-Constructive
excerpt: ''
date: 2021-09-14
venue: 'Algorithms'
paperurl: 'https://www.mdpi.com/1999-4893/14/9/267'
citation: 'Umberto Junior Mele, Luca Maria Gambardella, and Roberto Montemanni. (2021). <i>Algorithms</i>. 14(9), 267.'
---

<!--  &quot;A new constructive heuristic driven by machine learning for the traveling salesman problem.&quot; -->
<!-- [Download paper here](https://www.mdpi.com/1999-4893/14/9/267/pdf) -->


Recent systems applying Machine Learning (ML) to solve the Traveling Salesman Problem (TSP) exhibit issues when they try to scale up to real case scenarios with several hundred vertices. The use of Candidate Lists (CLs) has been brought up to cope with the issues. A CL is defined as a subset of all the edges linked to a given vertex such that it contains mainly edges that are believed to be found in the optimal tour. The initialization procedure that identifies a CL for each vertex in the TSP aids the solver by restricting the search space during solution creation. It results in a reduction of the computational burden as well, which is highly recommended when solving large TSPs. So far, ML was engaged to create CLs and values on the elements of these CLs by expressing ML preferences at solution insertion. Although promising, these systems do not restrict what the ML learns and does to create solutions, bringing with them some generalization issues. Therefore, motivated by exploratory and statistical studies of the CL behavior in multiple TSP solutions, in this work, we rethink the usage of ML by purposely employing this system just on a task that avoids well-known ML weaknesses, such as training in presence of frequent outliers and the detection of under-represented events. The task is to confirm inclusion in a solution just for edges that are most likely optimal. The CLs of the edge considered for inclusion are employed as an input of the neural network, and the ML is in charge of distinguishing when such edge is in the optimal solution from when it is not. The proposed approach enables a reasonable generalization and unveils an efficient balance between ML and optimization techniques. Our ML-Constructive heuristic is trained on small instances. Then, it is able to produce solutions—without losing quality—for large problems as well. We compare our method against classic constructive heuristics, showing that the new approach performs well for TSPLIB instances up to 1748 cities. Although ML-Constructive exhibits an expensive constant computation time due to training, we proved that the computational complexity in the worst-case scenario—for the solution construction after training—is $O(n^2 \log n^2)$, $n$ being the number of vertices in the TSP instance.


[Full view](https://www.mdpi.com/1999-4893/14/9/267)

Bibtex:
```
@article{mele2021new,
  title={A new constructive heuristic driven by machine learning for the traveling salesman problem},
  author={Mele, Umberto Junior and Gambardella, Luca Maria and Montemanni, Roberto},
  journal={Algorithms},
  volume={14},
  number={9},
  pages={267},
  year={2021},
  publisher={MDPI}
}
```