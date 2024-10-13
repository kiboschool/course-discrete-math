# Types of Graphs

There are many different types of graphs. We will discuss a few common types here, so you know what these terms mean in the future.

## Traversing Graphs

Every means of traversing a graph can also be a type of graph. A path graph is a graph that is one path, a cycle graph is a graph that has one cycle. These are quite simple graphs, but they still have names.

## Complete Graphs

A complete graph is a graph that contains all possible edges without double counting (multiedges). We denote a complete graph as $K_n$ where $n$ is the number of vertices in the graph. The concept is simple enough and the video below shows a the first few complete graphs.

<div class="embed"><iframe width="560" height="315" src="https://www.youtube.com/embed/egz_cP6vbIc?si=JtYMOglCyOrptrzb" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe></div>

>Think about it: How many edges are in each complete graph? Can you come up with a formula for $K_n$?

## Trees / Acyclic Graphs

An acyclic graph is a graph that has no cycles. These are also sometimes known as trees, due to the visual appearance of these graphs. The video below details some other definitions.

Before watching, it is important to know that the order of a graph is the number of vertices, and the size of a graph is the number of edges. These are not strictly necessary to memorize, but these terms are used in this video.

<div class="embed"><iframe width="560" height="315" src="https://www.youtube.com/embed/tVuEZakQxhQ?si=ZPsuClsd9k_ZJJbX" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe></div>

## Bipartite

Bipartite graphs can be separated into two sets of vertices where each set contains vertices that are only connected to vertices in the other set.

<div class="embed"><iframe width="560" height="315" src="https://www.youtube.com/embed/HqlUbSA9cEY?si=IRLM3gfmqihxVpQg" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe></div>

> Think first: What would a complete bipartite graph look like?

As you might expect, this is a bipartite graph where every vertex is connected to all vertices in the other set of vertices. This way, it is still bipartite, but it also falls under the complete definition of having all possible edges.

We would denote this with a $K_m,n$ where $m$ and $n$ are the size of the partite sets.

## Planar

Planar graphs can be drawn on the plane with no edge crossings. The video below discusses planar graphs.

<div class="embed"><iframe width="560" height="315" src="https://www.youtube.com/embed/LSkB6jR44aE?si=HlRLHJPVyewCxQ5Q" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe></div>

### Euler's Formula

Euler's Formula was described in the video prior. The following video explains this formula intuitively

<div class="embed"><iframe width="560" height="315" src="https://www.youtube.com/embed/-9OUyo8NFZg?si=qgCWhD4-ZBWosGdS" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe></div>

### Kuratowski's Theorem / Wagner's theorem

Kuratowski's theorem gives a condition that is necessary and sufficient for planar graphs. Wagner's theorem states this same idea in a slightly different way. Watch the following videos on these theorems to see how we can tell if a graph is planar.

<div class="embed"><iframe width="560" height="315" src="https://www.youtube.com/embed/UkjJE3bmPV0?si=woyq7SJk6GA2vaKe" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe></div>

<div class="embed"><iframe width="560" height="315" src="https://www.youtube.com/embed/2hkLC2q2wT4?si=DnE9kSY4WBveKOuM" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe></div>

This video shows an example with the Petersen Graph, a famous non-planar graph.

<div class="embed"><iframe width="560" height="315" src="https://www.youtube.com/embed/SbjIdEbd754?si=mENH974C8sNIQcCV" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe></div>