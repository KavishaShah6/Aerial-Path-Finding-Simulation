# FlightRoute
Network Optimization in Constrained Graphs
Overview
This project explores the challenge of identifying the optimal path within a fully connected graph where edge traversal is restricted by a maximum allowable length, x. In this problem, edges exceeding the threshold x are deemed unusable, adding an extra layer of complexity to the optimization process. The objective is to find not only a path that meets the length constraint but also the most optimal one in terms of distance, efficiency, or another utility metric.

The problem is inherently combinatorial, requiring an examination of numerous potential paths and combinations. This project leverages algorithms and data structures to solve this complex task efficiently, balancing distance constraints with the goal of achieving an optimal route.

Problem Statement
Given:

A fully connected, weighted graph G where nodes represent locations and edges represent direct paths between these nodes with associated costs (distances).
A threshold x which determines whether an edge is usable. Edges with lengths greater than x are excluded from the traversal.
Objective:

Identify a path from a source to a target node that:
Avoids edges longer than x.
Minimizes total travel cost or maximizes a defined utility function (e.g., efficiency).
Ensure computational efficiency despite the combinatorial nature of the problem.
Approach
Graph Representation: Represent the graph as an adjacency matrix or adjacency list to facilitate efficient path exploration.

Constraint Filtering: Preprocess the graph to remove or ignore edges that exceed the length x.

Optimization Algorithms:

Dijkstra's Algorithm: Modified to respect the length constraint on edges, finding the shortest path in terms of distance.

A* Search: Incorporate heuristics if specific starting and target nodes are involved, further optimizing path selection.

Dynamic Programming: For subproblems with overlapping paths, a dynamic programming approach could be used to reduce redundant calculations.

Utility Function Customization: Allow the optimization criterion to be user-defined (e.g., minimizing travel cost, maximizing connectivity).
