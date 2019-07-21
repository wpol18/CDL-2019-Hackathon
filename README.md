# CDL-2019-Hackathon
A repository for our group's CDL hackathon ideas/submission material.

## Graph coloring's connection to the real world
Given a graph with nodes and edges, the aim of graph coloring is to minimize the number of same-color nodes that share an edge; i.e. assign colors to each node in a graph such that no (or few) nodes connected by an edge share the same color.

This graph-theoretic problem underlies many important real-world applications. Some examples:
• Given a set of jobs and time-slots for those jobs, try to find the best time-schedule such that no jobs which share the same resource are scheduled at the same time. In this case, each job can be represented as a node, each time-slot as a color, and edges connecting nodes represent sets of jobs that share the same resource.
• Imagine your job is to allocate distribution networks and negotiate prices between suppliers and plants/factories that need to be supplied. Your goal is to have the maximum amount of leverage in price setting, and as such, you are interested in maximizing the amount of competitiveness between suppliers to supply regions of plants. In this case, each plant can be represented as a node, each supplier as a color; you want to spread out your suppliers across the plants in a network such that no supplier gains a monopoly over a large portion of a network.

## Graph coloring with Quantum Computing?
As the size of a graph increases node by node, the computational resources required for a good coloring scale exponentially: graph coloring for large problem sizes can be  computationally _expensive_ or even _intractable_. As such, it is a natural question to ask whether or not quantum computers can offer a performance advantage.

Here we demonstrate instances of graph coloring problems solved in a variety of popular quantum software frameworks, each targeting a different architecture and method of quantum information processing. The three we explored were D-Wave's annealing-based information processing, Rigetti Computing's gate-based framework, and Xanadu's continuous-variable photonics approach. Each approach tackles graph coloring in a radically different way.

## Some important files
1. ```DWave_GraphColoring```: Graph coloring applied to a real world problem with points distributed using real-world coordinates of distribution centres. 

2. ```Xanadu Photonic Processor GBS```: Example of graph coloring using Gaussian Boson Sampling ran on Xanadu's gaussian simulator.

3. ```Graph Coloring with QAOA in PyQuil```: Graph coloring done using Rigetti's QAOA implementation. 

4. ```Xanadu GBS Coloring Triangle:``` Graph coloring done on a tessalated triangular graph.
