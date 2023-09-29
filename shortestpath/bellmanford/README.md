# Bellman Ford

The Bellman Ford algorithm calculates the shortest path between one vertex and all other vertices in a weighted graph. It is capable of handling graphs in which edge weights are provided, including with negative numbers. Negative cycles can be detected by the algorithm.

## Getting Started Steps

- running "make setup" will install correct dependencies and check for correct python version (3.7+)
- running "make clean" will clean the project by removing all "pycache" folders and files
- running "make format will run autopep8 and docformatter to auto format the code
- running "make style" will run a lint checker on your code
- running "make test" or "make" will run all unit tests that have been created
- running "make coverage" will run all unit tests and give you a code coverage report

# Bellman Ford

## Requirements

- You must implement a class that handles the below interfaces for a graph data structure.
- The class name must be called "BellmanFord".
- You must implement at least 14 unit tests.
- Must get a 10/10 when running "make style"
- Your unit tests must reach 100% code coverage

## Interface

- The constructor __init__(self, graph_dict) should initialize the graph the class uses with graph_dict
- The function add_graph(self, graph_dict) sets the class graph variable to a new graph, initialized with graph_dict
- The function bellman_ford(self, src) implements the Bellman Ford algorithm, returning a list of the vertices in the graph along with their associated distances from the vertex src.
  - If a vertex cannot be reached from the passed src vertex, its distance should be float("inf")
  - All pairs of vertex, distance should be tuples
  - ex. [('a', 0), ('b', 5), ('2', -4), ('3', 8), ('d', float("Inf"))]
  - If a negative cycle is found, then the function should return None

## Tests

- Test to calculate the shortest paths from a given vertex on a variety of graphs.
- Test to see if there are any negative cycles.
- Test with an empty graph, and a src that is not in the graph
- Time and space complexity of the data structure.

## Library

You can only use basic python libraries (no special imports).
