## What is a graph (data structure)?
A graph is a common data structure that consists of a finite set of nodes (or vertices) and a set of edges connecting them. A pair (x,y)
is referred to as an edge, which communicates that the x vertex connects to the y vertex. In the examples below, circles represent vertices,
while lines represent edges.
In the examples below, circles represent vertices, while lines represent edges.


 ![image](https://user-images.githubusercontent.com/90922969/170011561-64cfb13f-5cf1-4fbb-b152-76a51f69ad1a.png)

 Graphs are used to solve real-life problems that involve representation of the problem space as a network. Examples of networks include telephone networks,
circuit networks, social networks (like LinkedIn, Facebook etc.).
 For example, a single user in Facebook can be represented as a node (vertex) while their connection with others can be represented as an edge between nodes.
Each node can be a structure that contains information like user’s id, name, gender, etc.

## Types of graphs:
- Undirected Graph:
In an undirected graph, nodes are connected by edges that are all bidirectional. For example if an edge connects node 1 and 2, 
we can traverse from node 1 to node 2, and from node 2 to 1.

- Directed Graph
In a directed graph, nodes are connected by directed edges – they only go in one direction. For example, if an edge connects 
node 1 and 2, but the arrow head points towards 2, we can only traverse from node 1 to node 2 – not in the opposite direction.

## Types of Graph Representations:
- Adjacency List
To create an Adjacency list, an array of lists is used. The size of the array is equal to the number of nodes.
A single index, array[i] represents the list of nodes adjacent to the ith node.


- Adjacency Matrix:
An Adjacency Matrix is a 2D array of size V x V where V is the number of nodes in a graph. A slot matrix[i][j] = 1 indicates that 
there is an edge from node i to node j.

## Here is some common terminology used when working with Graphs:

- Vertex - A vertex, also called a “node”, is a data object that can have zero or more adjacent vertices.
- Edge - An edge is a connection between two nodes.
- Neighbor - The neighbors of a node are its adjacent nodes, i.e., are connected via an edge.
- Degree - The degree of a vertex is the number of edges connected to that vertex.
