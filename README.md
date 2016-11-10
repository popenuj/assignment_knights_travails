# assignment_search
Marco?  Polo!

[A data structures and algorithms Ruby challenge from the Viking Code School](http://www.vikingcodeschool.com)

James and Jonathan

What data structure is used to implement DFS?

Stack

What data structure is typically used to implement BFS?

Queue

Which one can be done recursively? (the clue should be the data structure)

DFS, with the stack

Which one would you use to print a list of all the nodes in a tree or graph, starting with depth 1, then depth 2, then depth 3 etc.?

BFS, with the queue

What is the difference between a tree and a graph?

Tree is top to bottom, each node has certain children. Graphs are less hierarchical; the vertices can be interconnected in all kinds of ways.


PSEUDOCODE
----
Next, pseudocode the following processes with enough detail to be clear:

## Searching a simple tree of nodes where each Node has an array of child nodes (some_node.children) using DFS.

stack = []
def DFS
  Check if the current node matches. If it does, return its value.
  If not, put its value onto the stack.
  Run this on this node's children. If it has none, return nothing and remove the last entry from the stack.
end
Run this on the root node.

## Searching the same tree using BFS.

queue = Start [] End

def enqueue
  Check this node. If it's on the queue, remove it.
  If it has children, put them on the queue.
  Run this on the queue.
end

## Searching a graph, represented as an adjacency list using DFS.

source = nil
def DFS
  Check this vertex
  source = this node
  traverse_edges
end

def traverse_edges
  Check this node. If it's the one, return source.
  If this node has an edge attached, go there
end

from_vertices.each { DFS }

## Searching the same graph using BFS.

queue = Start [] End

def enqueue
  Check this node. If it's on the queue, remove it.
  If it has a child, put it on the queue.
  Run this on the queue.
end
