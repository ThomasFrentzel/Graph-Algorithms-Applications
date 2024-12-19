# Graph Algorithms Applications

This project implements six main graph algorithms in Java. These algorithms are commonly used to solve various real-world problems related to networks, optimization, and pathfinding. Below are the descriptions of each algorithm, its use cases within this repository, and the implementation details.


## 1. Dijkstra's Algorithm

**Description**:  
Dijkstra's algorithm is a famous algorithm for finding the shortest paths between nodes in a graph. It works by systematically exploring the closest neighbors to the starting node and updating their distances based on the shortest known path.

**Applications**:  
- In this repository, Dijkstra's algorithm is used to find the shortest path between cities in a directed graph.  
- The graph represents cities connected by roads with specific distances (edge weights).
- The program allows the user to choose a starting city, and then it calculates the shortest paths to all other cities using the algorithm. The result includes the distances and the corresponding paths.
  
**Explanation**:  
The algorithm starts at a source node (city) and explores all of the neighboring nodes at the current level before moving on to nodes at the next level. It uses a priority queue to ensure that the shortest path is always explored first. The user can interact with the program by selecting a starting city and seeing the shortest routes to all other cities.

## 2. Bellman-Ford Algorithm

**Description**:  
Bellman-Ford algorithm is another algorithm for finding the shortest paths in a graph. It is capable of handling graphs with negative edge weights and detecting negative cycles.

**Applications**:  
- This algorithm is used in the repository to calculate the shortest paths between cities, similar to Dijkstra's algorithm.  
- However, Bellman-Ford is used here to demonstrate its capability to handle graphs with negative edge weights, should the need arise (e.g., negative costs for some routes).
- The program computes the shortest paths from a chosen city to all others, checking for any negative-weight cycles in the graph.

**Explanation**:  
Bellman-Ford works by iteratively relaxing all edges in the graph, making it a bit slower than Dijkstra's algorithm but more versatile. This algorithm also detects negative cycles, which is useful in applications like financial networks.

## 3. Floyd-Warshall Algorithm

**Description**:  
The Floyd-Warshall algorithm computes the shortest paths between all pairs of nodes in a graph. It works on both directed and undirected graphs and is particularly useful for dense graphs.

**Applications**:  
- In this repository, Floyd-Warshall is applied to find the shortest paths between all cities in a network.  
- It calculates the shortest distance between each pair of cities in the graph, providing a complete matrix of all shortest paths.
- This algorithm is used here to calculate the distances between all cities, which is useful in applications where the shortest paths between multiple pairs of cities are needed.

**Explanation**:  
Floyd-Warshall uses dynamic programming to compute the shortest paths between all pairs of nodes. The program generates a matrix that shows the shortest path distance for every possible pair of cities and can be used to track how to get from one city to another.

## 4. Depth-First Search (DFS)

**Description**:  
Depth-First Search is an algorithm for traversing or searching tree or graph structures. It starts at the root (or an arbitrary node) and explores as far as possible along each branch before backtracking.

**Applications**:  
- In this repository, DFS is used to explore the graph structure representing cities and routes.  
- The program starts at a specified city and explores all connected cities before backtracking. This can be used for tasks like finding all possible routes from a city to other cities in a network.
- DFS can also be useful for detecting connected components in the graph, for example, checking if all cities are reachable from the starting city.

**Explanation**:  
DFS explores as deeply as possible down one branch before backtracking. This is useful for problems like finding all possible paths or connected components. In the context of the cities network, DFS allows for exploring all reachable cities from a chosen starting point.

## 5. Breadth-First Search (BFS)

**Description**:  
Breadth-First Search is an algorithm for traversing or searching tree or graph structures. It starts at the root and explores all neighbors at the present depth level before moving on to nodes at the next depth level.

**Applications**:  
- In this repository, BFS is used to find the shortest path between two cities in an unweighted graph.  
- The algorithm is ideal for scenarios where the edges (roads between cities) have equal weights, and the goal is to find the shortest path in terms of the number of edges.
- The program computes the shortest path from a source city to a destination city in terms of the number of intermediate cities.

**Explanation**:  
BFS explores the graph level by level, making it particularly useful for finding the shortest path in unweighted graphs. In this context, it can be used to determine the minimum number of roads (edges) needed to travel from one city to another.

## 6. Kruskal's Algorithm

**Description**:  
Kruskal's algorithm is a minimum spanning tree algorithm used to find the subset of edges that connects all the vertices in a graph with the minimum possible total edge weight.

**Applications**:  
- In this repository, Kruskal's algorithm is used to compute the minimum spanning tree (MST) for the cities network, ensuring that all cities are connected with the minimum total road length.  
- The program adds roads (edges) one by one, starting with the shortest available, to create a network that connects all cities with the least total cost.
- This is useful for problems like designing the least-cost network of roads between cities.

**Explanation**:  
Kruskal's algorithm sorts all the edges in the graph by weight and adds them one by one to the MST, ensuring no cycles are formed. It is particularly effective in sparse graphs and is used here to optimize the road network by minimizing the total length of roads needed to connect all cities.

---

## Clone the repository:
   ```bash
   git clone https://github.com/ThomasFrentzel/Graph-Algorithms-Applications
 ```
