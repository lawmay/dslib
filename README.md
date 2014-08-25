dslib
==============

A library of useful data structures in Javascript

## Installation
```
npm install dslib --save
```
## Usage
```
var dslib = require('dslib');
```
###Stack
```
var stack = new dslib.Stack();

//methods
stack.push(item); //adds an item to top of stack
stack.pop(); // removes and returns last item added to stack
stack.size() // returns size of stack
```     

###Queue
```
var queue = new dslib.Queue();

//methods 
queue.enqueue(item); // adds an item to end of queue
queue.dequeue(); // removes and returns first item in queue
queue.size(); // returns size of queue 
```

###Set

```
var set = new dslib.Set();

//methods
set.add(item); //adds an item to the set
set.remove(item); //removes an item from the set
set.contains(item); // returns a boolean if item in slt 
```

###LinkedList
```
var linkedList = new dslib.LinkedList();

//methods
linkedList.addToTail(item); //adds an item to tail of linkedList
linkedList.removeHead(); //removes an item from head of linkedList
linkedList.contains(item); //returns a boolean if item in linkedList
```

###Tree
```
var tree = new dslib.Tree();

//methods
tree.addChild(value); //adds a child to tree with set value
tree.contains(value); //returns a boolean if node with value in tree;
```

###BinarySearchTree
```
var binarySearchTree = new dslib.BinarySearchTree();

//methods
binarySearchTree.insert(value) //inserts a node with the specific value
binarySearchTree.contains(value) //returns a boolean if the value is in the tree
binarySearchTree.depthFirstLog(callback) //executes callback on each node in tree, depth first order
```

## Tests

```
gulp mocha
//or
gulp watch
```

## Contributing

In lieu of a formal styleguide, take care to maintain the existing coding style.

To Contribute via Issue Notice:
* Write up a description of the problem
* I will write a fix correspondingly

To Contribute via Pull Request:
* Fork the repo

* Add unit tests for any new or changed functionality. Write tests in the 
appropriate spec file in the tests directory

* Submit a pull request to master branch

## Release History

* 0.1.0 Initial release
* 0.2.0 Tree, Stack, Queue, Set, LinkedList
* 0.3.0 BinarySearchTree
