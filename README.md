Trabalho de implementação de uma biblioteca de grafos.

## Overview
Graph library in C (`grafo.c` / `grafo.h`) with a test driver (`teste.c`), built with the provided `makefile`.

Implemented with adjacency lists and reading a graph from a text file (`le_grafo`; see `input.txt`). Supported operations:
- graph name, number of vertices and number of edges
- number of connected components (DFS)
- bipartiteness check
- diameter of each component (BFS)
- cut vertices and cut edges (Tarjan's DFS low-link algorithm)

Build and run: `make`, then `./teste < input.txt`.
