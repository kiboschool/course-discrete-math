# Properties of Graphs

There are more terms and properties of graphs we need to define before starting to use them.

## Neighbors

A vertex is considered a neighbor of another vertex if they are connected by an edge.

## Vertex Degrees

The degree of a vertex is the number of edges attached to the vertex.

## Graph Manipulation

Sometimes, we wish to make changes to a graph. If an edge is removed, this is called an edge-cut. If a vertex is removed, this is called a vertex-cut.

A graph that is disconnected, whether by cut or just the nature of the graph, is called a disconnected graph. We consider it to be disconnected if we cannot connect every single pair of vertices with some path through edges.

## Isomorphism

Two graphs are isomorphic if they have the same underlying structure. More specifically, they have the same number of vertices and edges, and we can form a one-to-one mapping of vertices in one graph to vertices in the other such that these verticies are connected to the same neighbors as their image (and their neighbors' images).

The following video explains this concept, along with this specific mathematical definition.

<div class="embed"><iframe width="560" height="315" src="https://www.youtube.com/embed/EwV4Puk2coU?si=hJ10-z8xcNhUyhXO" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe></div>

>Check your Understanding: What are the isomorphic graphs at the end of the video?

<details><summary>Check your answer</summary>
A & B are isomorphic, no other pair is.
</details>

Like we had equivalence in modulus, we have this idea of isomorphism, where isomorphic graph are basically "equal."

## Graph Coloring

As mentioned in a prior video, we can color graphs. Graphs are properly colored if no two adjacent vertices have the same color. There is a theorem, called the Four Color Theorem that states this can be done in 4 colors, for any graph of a specific type. We'll come back to this topic later on, when we've defined a few more things.

## Overview

The following video discusses many of the terms and topics discussed until now. The descriptions are brief, and it does not cover all topics, but it does discuss some of the relevance to computer science.

<div class="embed"><iframe width="560" height="315" src="https://www.youtube.com/embed/LFKZLXVO-Dg?si=7E7XLNuAIsUVg0ap" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe></div>

It may feel overwhelming to see all these definitions, and we are not at the end of them! Luckily, these terms usually have names that make sense, and they all fit together well enough that with practice, using them becomes easy.
