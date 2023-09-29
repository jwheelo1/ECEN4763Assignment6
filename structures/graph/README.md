# Data Structures Graph

This data structure should be mostly copied from assignment 3, but it needs to be adjusted to include edge weights to work with Bellman Ford. Only interface changes will be included here, reference assignment 3 for the functions that have not changed.

## Getting Started Steps

- running "make setup" will install correct dependencies and check for correct python version (3.7+)
- running "make clean" will clean the project by removing all "pycache" folders and files
- running "make format will run autopep8 and docformatter to auto format the code
- running "make style" will run a lint checker on your code
- running "make test" or "make" will run all unit tests that have been created
- running "make coverage" will run all unit tests and give you a code coverage report

# Graph

## Requirements

- You must implement a class that handles the below interfaces for a graph data structure.
- The class name must be called "Graph".
- You must implement at least 14 unit tests.
- Must get a 10/10 when running "make style"
- Your unit tests must reach 100% code coverage

## Interface

- The constructor init(self, graph=None) should initialize the graph if given, or initialize it to be empty if not.
Note: The graph dictionary will look different than before. Now, it includes the edge weights. An example is given below, where the first value in a tuple is the neighboring vertex, and the second is the weight on the edge between the two vertices.
```
graph_dict = {
    0: [(1, 5), (2, 4)],
    1: [(3, 3)],
    2: [(1, 6)],
    3: [(2, 2), (0, 9)]
}
```
- The function add_edge(self, vertex1, vertex2, weight) adds an edge between vertex 1 and vertex 2 with the given weight. If vertex1 or vertex2 are not yet in the graph, add them and then add the edge.
- The function get_neighbors(self, node) returns all of the vertixes going out of the node passed in (return empty list if the graph is empty or if the node does not exist)

## Tests

- Tests all functions as usual, but now with the weights included.
- Test intializing with the given dictionary
- Test adding edges with weights

## Corner Cases

- Removal of nonexistent vertices and edges
- Edges going to and from new vertices

## Library

You can only use basic python libraries (no special imports).
