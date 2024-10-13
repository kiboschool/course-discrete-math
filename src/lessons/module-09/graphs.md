# Graphs

Graph Theory is a branch of mathematics concerned with Graphs. These mathematical structures can represent a variety of situations, and therefore, studying different properties of graphs can help inform decisions that must be made and problems that need to be solved.

## Readings

[Chapter 9](https://discretemath.org/ads/s-graphs-introduction.html)
[Chapter 4](https://discrete.openmathbooks.org/dmoi3/ch_graphtheory.html)

## Definition of a Graph

The following video gives a short introduction to the idea behind graph theory.

<div class="embed"><iframe width="560" height="315" src="https://www.youtube.com/embed/_XPIQZSrHaA?si=CMFN4eh4TJQL1mqI" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe></div>

This video gives the idea behind a few different definitions of graphs.

<div class="embed"><iframe width="560" height="315" src="https://www.youtube.com/embed/cm89jiyD5Vo?si=pAz4A1zayGVYz8F-" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe></div>

The last definition in this video is likely the most useful in our context, but I want to introduce one more method of representing a graph that is often used in code.

### Adjacency List Representation

Similar to the last example, we want to attach an edge in one step. First, we store a list of vertices. Then, we define our edges under each vertex. We do this by taking each vertex in our list and storing a list of all vertices that it has a directed edge pointed towards.

Again, similar to the last example, if we want an undirected edge, we simply make sure the edge points both ways. If we want to represent multiple edges, we could include the vertex multiple times. This is known as an Adjacency List.

We can represent this in an even simpler way by creating a table, with a row and a column for each vertex. We fill in a 1 if there is an edge from the row vertex to the column vertex, and 0 if there is not. For multi-edges, we can write 2, 3, or more instead of 1.

This representation is called an Adjacency Matrix, and since it's in the form of a matrix (or 2D array), it is easy to create the structure in code.

> Think about it: Try to create a class to represent a graph.

## Directed Graphs

As mentioned above, edges can have direction. If a graph has any directed edges, it is known as a directed graph. This includes graphs where some edges are undirected. A graph is only undirected if all of its edges are undirected.

## Weighted Graphs

Along with having a direction, some graphs give edges another piece of information: weight. This can be representative of many things, like distance, difficulty, or cost. Since graphs are discussed in terms of shape, and not the length of each specific edge, if we have a problem where moving between two vertices is easier or harder, we can introduce weight to include this distinction.
