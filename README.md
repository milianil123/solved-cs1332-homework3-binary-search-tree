Download Link: https://assignmentchef.com/product/solved-cs1332-homework3-binary-search-tree
<br>
You are to code a binary search tree, BST, which is a collection of nodes, each having a data item and references pointing to left and right child nodes. The BST must follow the order property: for any given node, its left child’s data and all of its children’s data must be less than the current node while its right child’s data and all of its children’s data must be greater than the current node. In order to compare the data, all elements added to the tree must implement Java’s generic Comparable interface.

It will have two constructors: a no-argument constructor (which should initialize an empty tree), and a constructor that takes in a collection of data to be added to the tree, and initializes the tree with this collection of data.

You may import Java’s LinkedList/ArrayList classes for the 4 traversal methods and findPathBetween, but only for these methods.

<h2>Recursion</h2>

Since trees are naturally recursive structures, all methods that are not <em>O</em>(1) <strong>must be implemented recursively</strong>, except for level order traversal. You’ll also notice that a lot of the public method stubs we’ve provided do not contain the parameters necessary for recursion to work, so these public methods act as “wrapper methods” for the user to use. You will have to write private recursive helper methods and call them in these wrapper methods. Don’t forget to write javadocs for all private helper methods written. To reiterate, <strong>do not change the method headers for the provided methods</strong>.

For methods that change the structure of the tree in some way, we highly recommend you use a technique taught in class called pointer reinforcement. It is not required, but it will make the homework cleaner, and it’ll also help greatly when we get to a later homework.

<h2>Nodes</h2>

The binary search tree consists of nodes. A class BSTNode is provided to you. BSTNode has getter and setter methods to access and mutate the structure of the nodes.

<h2>Methods</h2>

You will implement all standard methods for a Java data structure (add, remove, etc.) in addition to a few other methods (such as traversals). You must follow the requirements stated in the javadocs of each method you implement.

<h2>Traversals</h2>

You will implement 4 different ways of traversing a tree: pre-order traversal, in-order traversal, postorder traversal, and level-order traversal. The first 3 MUST be implemented recursively; level-order is best implemented iteratively. For a level-order traversal, you may use Java’s Queue interface (and an implementing class for it such as LinkedList).

<h2>Height</h2>

You will implement a method to calculate the height of the tree. The height of any given node is max(left node’s height, right node’s height) + 1. When doing this calculation, a null node has a height of -1. As such, a leaf node will have a height of 0, which is calculated by max(-1, -1) + 1.

<h2>Comparable</h2>

As stated, the data in the BST must implement the Comparable interface. As you’ll see in the files, the generic typing has been specified to require that it implements the Comparable interface. You use the interface by making a method call like data1.compareTo(data2). This will return an int, and the value tells you how data1 and data2 are in relation to each other

<ul>

 <li>If positive, then data1 is larger than data2.</li>

 <li>If negative, then data1 is smaller than data2.</li>

 <li>If zero, then data1 equals data2.</li>

</ul>

Note that the returned value can be any integer in Java’s int range, not just -1, 0, 1.