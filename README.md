# Research-Pathfinding

## DIJKSTRA
### what is dijkstra's algorithm?
Dijkstra's algorithm is an algorithm made by Edsger Wybe Dijkstra. The algorithm is used for finding the cheapest/shortest path between 2 nodes in a graph.
### How does it work?
The dijkstra's algorithm works by calculating the cheapest route to every node starting from the cheapest known node to the adjacent nodes and so on. 
This goes on until the cheapest route is found for the destination node.
### Pseudocode c++
```cpp
// NodeRecord contains (node, connection, costSoFar)
vector<node> path // path form start to destination
vector<NodeRecord> visited // all the visited nodes
vector<NodeRecord> openList // all the known nodes that still have to be visited
NodeRecord currentNode = startnode


add currentNode to openList

while openlist is not empty
{
  for each connection to currentNode
  {
    connectedNode costSoFar = connection cost + currentNode costSoFar
  
    if connectedNode is in visited // go to next connection
      continue
    
    if connectedNode is in openlist
      if connectedNode costSoFar < costSoFar in openList // assign the smallest connection to every node
        change openList node to connected node
        
    else
      add connectedNode to openList
  }
  
  add currentNode to visited
  remove currentNode from openList
  
  currentNode = smallest node in the openList// smallest = lowest costSoFar
  
  if currentNode == destinationNode
  {
    while currentNode != startNode
    {
      get node from connection in currentNode
      add this node to path
      currentNode = othernode
    }
    add startNode to path
    break
  }
}

 reverse the path // because it goes from destination to start now

```

### Visualization


## Breadth first search
### what is BFS?
BFS is an algorithm made by Konrad Zuse it was firstly used in pathfinding by Edward Forrest Moore, He used it for finding the shortest route in a maze.
### How does it work?
BFS does not use connection costs because it asumes that every connection is the same. The algorithm starts with the start node. It looks at all the connected nodes. If the destination isn't one of them he will look at the nodes connected to them. this goes on until the destination is found.
is one of them
### Pseudocode c++
```cpp
code
```
