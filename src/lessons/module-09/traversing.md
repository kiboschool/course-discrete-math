# Traversing Graphs

There are many ways to discuss traversing a graph. We'll cover all the different terms here.

## What is Traversing?

In basic terms, we want to know how we can follow edges in certain ways. This relates back to the bridges problem, as a person wanted to know if you could physically travel across each edge exactly once.

## Traversing

Please watch these videos in order to understand the different ways we can discuss traversing a graph.

### Walk

<div class="embed"><iframe width="560" height="315" src="https://www.youtube.com/embed/YlJ8plSab6g?si=aGNgWWE37Y30mmOF" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe></div>

### Trail

<div class="embed"><iframe width="560" height="315" src="https://www.youtube.com/embed/2ZgfZgmC9rA?si=GqySnqvEzhTzZoli" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe></div>

### Path

<div class="embed"><iframe width="560" height="315" src="https://www.youtube.com/embed/RfC8sLCHSGE?si=cU_oGCv-hvpYbmpu" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe></div>

### Circut

<div class="embed"><iframe width="560" height="315" src="https://www.youtube.com/embed/_YvlvSO7RBQ?si=Yjd8FIUUvvd1QsZ2" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe></div>

### Cycle

<div class="embed"><iframe width="560" height="315" src="https://www.youtube.com/embed/Cte3zFJ59Nk?si=I8o7zy8-0SbBxYn-" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe></div>

### Eulerian Cycles

<div class="embed"><iframe width="560" height="315" src="https://www.youtube.com/embed/sw79Z34v0dQ?si=voHI9o4qKKYyjuca" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe></div>

As a note, there is the term "Eulerian Path"

>Think first: Can you guess what its definition would be?

This is an Eulerian Cycle without the restriction of ending on the same vertex we started on. As such, we're allowed two odd-degree nodes for a graph to have an Eulerian Path.

>Check your understanding: Thinking back to the Königsberg bridges problem, can you explain why it is impossible to cross each bridge exactly once?

<details><summary>Check your answer</summary>
The degrees of the vertices are all odd! This graph doesn't even have an Eulerian Path.
</details>

>Think about it: Why do you think we need even degree vertices for an Eulerian cycle?
> Hint: Try drawing out some graphs, and tracing a path with a pencil. What happens as you pass through a vertex?
> Eulerian Paths allow 2 odd-degree vertices. Why is this?

## Distance

The distance between two vertices is the length of the shortest path between them. We define this length as the number of edges we cross, or the number of vertices in the path minus 1.

>Think about it: Does this make sense as a definition of distance?