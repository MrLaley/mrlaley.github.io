---
title: "Graph Isomorphism & Algorithmic Solver"
description: "Collaborative development of a high-performance Python solver for the Graph Isomorphism problem, featuring parallel processing, automorphism-based pruning, and advanced data structures."
pubDate: "Jan 01 2026"
heroImage: '../../assets/graph-isomorphism-cover.png'
category: "university"
---

## Project Overview

This project involved the collaborative development of a highly optimized computational solver designed to tackle the Graph Isomorphism problem—a classic and complex challenge in combinatorial optimization. By analyzing structural equivalences between graphs, the solver leverages advanced theoretical concepts and high-performance programming techniques in Python to minimize execution time and space complexity.

## Technical Implementations & Algorithmic Depth

The software achieves high performance through a series of sophisticated algorithmic techniques and structural optimizations:

* **Fast Partition Refinement:** Implemented a robust partitioning algorithm based on Hopcroft's DFA minimization approach. Utilizing fast-indexing data structures (`deques`, `defaultdict`, and arrays), this reduced the time complexity for partitioning to **O((V+E)logV)**.
* **Automorphism-Based Pruning:** Developed a highly efficient Branch-and-Bound algorithm that prunes redundant search spaces dynamically. By identifying automorphism groups (using generators, stabilizers, and orbits) and applying the Schreier-Sims membership test, the algorithm skips symmetrically equivalent sub-trees, drastically cutting down computation times for highly symmetrical graphs.
* **Dynamic Branching Rules:** Designed a dynamic heuristic to select the optimal target color class to branch on. The algorithm adapts to the graph's typology in real-time—defaulting to the class with the highest-degree vertex for speed, but strategically switching to the smallest class when heavily refined to aggressively shatter partitions.
* **Advanced Graph Preprocessing:** 
  * **Twinning:** Contracted structural twins recursively in an **O(V+E)** pass, shrinking the graph size before heavy combinatorial algorithms begin.
  * **Trees & Forests:** Implemented the AHU (Aho, Hopcroft, Ullman) algorithm to rapidly detect and solve tree structures natively, bypassing the need for slower generic isomorphism checks.
  * **Complements:** For dense graphs, the algorithm strategically calculates the graph's complement in **O(V²)**, significantly speeding up edge traversals during the refinement phase.
* **Parallel Processing & Benchmarking:** Leveraged multi-threading pool optimization fine-tuned for modern CPU architectures (utilizing Performance and Efficient cores), ensuring concurrent processing of multiple graph instances and rigorous empirical time benchmarking.

## Execution & Collaboration

The project required strict code organization and mathematical rigor. The team successfully distributed complex theoretical implementations (such as fast color refinement, branching logic, and automorphism tracking), refactored legacy code for compatibility, and meticulously benchmarked execution times to prove algorithmic efficiency and achieve maximum grading.

**Skills:** Python, Graph Theory, Algorithm Optimization, Combinatorial Search, Data Structures, Parallel Processing.