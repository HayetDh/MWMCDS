Minimum Weight Minimum Connected Dominating Set (MWMCDS)

1-	Context
In graph theory,  a dominating set (DS) for a simple undirected graph G = (V, E) where V is the set of vertices and E is the set of edges, is a subset D of V such that each vertex not in D has at least one neighbour in D. If its induced subgraph G(D) is connected then it represents a connected dominating set (CDS).
The minimum weight minimum connected dominating set problem (MWMCDS) is a bi-objective optimization problem defined on a simple undirected edge-weighted graph as a CDS with minimum cardinality and minimum total weight.


2-	Data Description
Two types of datasets were used in this work :
Dataset1 : it contains 9 instances of graphs which are undirected and edge-weighted.
Dataset2 : it contains 360 problem instances. Each instance consists of an undirected vertex-weighted graph, and as MWMCDS problem needs an edge-weighted graph, we randomly generate the edge weights in the interval [5, 50]. The number of edges m is varied for each vertex count n, and for a specific number of vertices and edges, 10 instances exist for most graphs.

3-	.exe files
A greedy randomized local search algorithm based on non-dominated sorting concept is proposed to solve the MWMCDS problem. The program code is entirely written in C++ language and the executable versions produced are MWMCDS_dataset1.exe and MWMCDS_dataset2.exe files, where :
MWMCDS_dataset1.exe : presents the executable version of the previously mentioned algorithm using dataset1. To analyze its performance, a simple data transfer system is used, wherein case of successful transfer the total edges weight traversed from a vertex sender to a vertex receiver through dominator vertices is represented by energy consumption.
MWMCDS_dataset2.exe : presents the executable version of the algorithm using dataset2. The Pareto fronts obtained are measured by different performance metrics: hypervolume indicator (noted by HVI), overall non-dominated vector generation (noted by ONVG), and the the CPU time expressed in seconds (noted by Time).


