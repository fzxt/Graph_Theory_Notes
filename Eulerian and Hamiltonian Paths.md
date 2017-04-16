# Definitions

## Degree
- Out degree of a vertex in the graph.

## Closed paths
- A path is closed iff you start and end at the same vertex.

## Trail
- An open path which visits every edge of a graph once and only once.

## Circuit
- A closed trail.

## Eulerian graph

### Eulerian Trail
  - A Eulerian trail is a trail that visits every edge of the graph once and only once. It can end on a vertex different from the one on which it began.

  - A graph which has a Eulerian trail is said to be traversable.

  - A Eulerian trail exists in a graph if and only if there are either **no odd vertices** or **two odd vertices**  

### Eulerian circuit
  - A Eulerian circuit is a Eulerian trail that is closed.

  - For a graph to contain a Eulerian Circuit, all vertices of the graph must be of even degree.

  - A Eulerian circuit exists iff there **no odd vertices**.

### Eulerian graph
  - A graph is called Eulerian when it has at least one Eulerian circuit

## Hamiltonian Graphs

### Hamiltonian Circuit
  - A Hamiltonian Circuit in a graph is a closed path that visits every vertex in the graph exactly once.

### Hamiltonian Graph
  - A graph is Hamiltonian iff it contains a Hamiltonian circuit.

## Important note for Hamiltonian and Eulerian graphs
- A Eulerian circuit traverses every edge in a graph exactly once, but **may repeat vertices**, while a Hamiltonian circuit visits each vertex in a graph exactly once but **may repeat edges**.

### Useful links

[How to tell if a graph has a Eulerian path or circuit](http://www.ctl.ua.edu/math103/euler/howcanwe.htm)

[Eulerian and Hamiltonian Graphs](http://www3.ul.ie/cemtl/pdf%20files/cm2/GraphEulerHamilton.pdf)
