<h1> About Prim's Algorithm </h1>
<b>Prim’s algorithm always starts with a single node and it moves through several adjacent nodes, in order to explore all of the connected edges along the way.</b>
<br><li>A group of edges that connects two sets of vertices in a graph is called cut in graph theory.
<li>At every step of Prim’s algorithm, find a cut (of two sets, one contains the vertices already included in MST and the other contains the rest of the vertices), pick the minimum weight edge from the cut, and include this vertex to MST Set (the set that contains already included vertices).
