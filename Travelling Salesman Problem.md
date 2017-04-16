## What is the traveling salesman problem?

Any problem that shares these common elements:
- A traveler
- A set of sites
- A cost function for travel between pairs of sites
- A need to tour all the sites
- A desire to minimize the total cost of the tour

is known as a **traveling salesman problem**, or **TSP** for short.

## What approaches to solve TSP
- Cheapest link algorithm
  - Order the cheapest edges
  - Construct a path by `adding` edges
    - While adding edges, avoid paths that would cause cycles that don't contain all the vertices of the graph.
    - Once you have a cycle that contains all the edges of a graph (i.e, a Hamiltonian Cycle), you may exit the algorithm
- Nearest neighbor algorithm
  - Start at some vertex
  - Visit neighbor with cheapest edge, add to path
  - Repeat until we have visited every node, while avoiding edges that would go back to any nodes we have already visited

- The following approaches are near equivalent and produce different results depending on the graph.

**These solutions don't guarantee the optimal solution**

- The simple gist of these algorithms is to keep adding to your path while avoiding going to back to any nodes you've already visited/where you started from.

## Videos to understand the different approaches to solve the TSP
- [Cheapest Link Algorithm](https://www.youtube.com/watch?v=nYKsLRxIBmA)

- [Nearest neighbor Algorithm](https://www.youtube.com/watch?v=G8a8bJuQxnw)
