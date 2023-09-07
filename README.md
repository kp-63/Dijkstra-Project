# Dijkstra-Project

Dijkstra's algorithm is used to find the shortest path from a single source vertex to all other vertices in a weighted graph. It was developed by Dutch computer scientist Edsger W. Dijkstra in 1956. The main objectives and needs for Dijkstra's algorithm are as follows:

Shortest Path: Dijkstra's algorithm helps find the shortest path from a specified source vertex to all other vertices in a graph. This information is valuable in various applications, such as network routing, GPS navigation, and optimization problems.

Weighted Graphs: Dijkstra's algorithm is particularly useful when dealing with graphs where each edge has a non-negative weight. It finds the shortest path based on the sum of edge weights.

Single-Source: The algorithm focuses on finding the shortest paths from a single source vertex to all other vertices in the graph. This is in contrast to other algorithms like Bellman-Ford, which can handle graphs with negative edge weights but are more general.

# Algorithm

The code defines a function minDistance to find the vertex with the minimum distance value among the vertices that are not yet included in the shortest path tree.

The printSolution function is used to display the final distances from the source vertex to all other vertices.

In the dijkstra function, arrays dist and sptSet are initialized to keep track of the shortest distances and whether a vertex is included in the shortest path tree, respectively.

The algorithm proceeds by iteratively selecting the vertex with the minimum distance from the source (u) and including it in the shortest path tree (sptSet[u] = true).

It then updates the distances to adjacent vertices (v) if a shorter path is found through u.

This process continues until all vertices are included in the shortest path tree.

Finally, the printSolution function is called to display the shortest distances from the source vertex.

In the main function, an example graph is defined as an adjacency matrix, and Dijkstra's algorithm is called with source vertex 0. The output will show the shortest distances from vertex 0 to all other vertices in the graph.
