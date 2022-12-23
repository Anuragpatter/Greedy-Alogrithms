<h1> About Prim's Algorithm </h1>
<b> It starts with an empty spanning tree. The idea is to maintain two sets of vertices. The first set contains the vertices already included in the MST, the other set contains the vertices not yet included. At every step, it considers all the edges that connect the two sets and picks the minimum weight edge from these edges. After picking the edge, it moves the other endpoint of the edge to the set containing MST. 

<br>Prim’s algorithm always starts with a single node and it moves through several adjacent nodes, in order to explore all of the connected edges along the way.</b>

<b>How does Prim’s Algorithm Work?</b>
<br>The idea behind Prim’s algorithm is simple, a spanning tree means all vertices must be connected. So the two disjoint subsets (discussed above) of vertices must be connected to make a Spanning Tree. And they must be connected with the minimum weight edge to make it a Minimum Spanning Tree.
<br><li>A group of edges that connects two sets of vertices in a graph is called cut in graph theory.
<li>At every step of Prim’s algorithm, find a cut (of two sets, one contains the vertices already included in MST and the other contains the rest of the vertices), pick the minimum weight edge from the cut, and include this vertex to MST Set (the set that contains already included vertices).
<li>Create a set mstSet that keeps track of vertices already included in MST. 
<li>Assign a key value to all vertices in the input graph. Initialize all key values as INFINITE. Assign the key value as 0 for the first vertex so that it is picked first.
<dl>
  <li>While mstSet doesn’t include all vertices,
  <dd><li>Pick a vertex u which is not there in mstSet and has a minimum key value. 
  <li>Include u in the mstSet.
  <li>Update the key value of all adjacent vertices of u. To update the key values, iterate through all adjacent vertices.
  <li>For every adjacent vertex v, if the weight of edge u-v is less than the previous key value of v, update the key value as the weight of u-v.
</dl>
