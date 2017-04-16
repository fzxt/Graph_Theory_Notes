## Definitions

### Postman Tour
- A postman tour in a graph G is a closed walk that traverses each of G at least once. A minimum postman tour in a weighted graph G is a postman tour of G of smallest weight.

## What is the Chinese Postman Problem?
- A letter carrier wishes to deliver mail along every street in a city. There is a cost (travel time) associated with the traversal of every street. How can the carrier deliver the mail and then return to the starting point so that the total cost of her traversal is as small as possible?

- The problem is asking to find a minimum closed walk in a weighted graph that traverses each edge at least once, that is a minimum postman tour.

## Notes
- If the graph is **Eulerian**, then every **Euler tour** is in fact a minimum postman tour of the graph.

- If the graph his not Eulerian, then some of the edges will have to traversed more than once.
  - This means we should be choosing edges that we will be traversing more than once to have weights as small as possible

## Solutions
- There exists an algorithm to solve this.

- The main idea behind this algorithm, is recognizing that if we have a graph that does is not Eulerian (i.e, has vertices of out-degree that are odd), then no matter what, the postman will have to repeat an edge. Knowing this, the algorithm finds the pair of edges to revisit such that we obtain the minimum time. The algorithm will only use pairs of vertices that are odd in order to figure out the ones to revisit 

- Note, since we recognized that no matter what we have to revisit an edge, we essentially "draw" an extra edge on the graph (the edge we are revisiting). This makes the previous odd vertices, even, and thus Eulerian. Therefore we can be sure that any path with the "extra edges" will be a minimum solution to the problem.

## Useful video to explain the motivation and steps of the algorithm
- [Chinese Postman Algorithm](https://www.youtube.com/watch?v=spaUY8PlyYA)
