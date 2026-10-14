# grafos-t1
Graph assignment (UFPR): implement the graph library whose interface is fixed in `grafo.h`, then check it with the provided driver `teste.c`.

**Input.** A graph read from `stdin`: first the graph name, then one vertex name per line and edges as `u -- v [weight]` (optional non-negative weight). Lines starting with `//` are comments, and vertices that appear in an edge need no separate line.

**Implemented in `grafo.c`** (adjacency lists):
- `le_grafo` / `destroi_grafo`: read and free the graph
- `nome`, `n_vertices`, `n_arestas`, `n_componentes`
- `bipartido`: bipartiteness check
- `diametros`: diameter of every component, in non-decreasing order (BFS)
- `vertices_corte`: cut vertices in alphabetical order (Tarjan's low-link DFS)
- `arestas_corte`: cut edges in alphabetical order

**Build and run:** `make`, then `./teste < input.txt`.
