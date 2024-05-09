
# Stacks 

A stack is an abstract, linear data type with a predefined capacity (or boundary). It follows a particular order for adding or removing elements. 

Linear data structures organize their components in a straight line, so if we add or remove an element, they will grow or shrink respectively.

This is called the ```Last In First Out (LIFO)``` or ```First In Last Out (FILO) ordering```.

The implementation of stacks is relatively easy. The functionality depends on the ```pop``` and ```push``` method, as you can see from the illustration above. The ```pop``` method removes or deletes elements from the stack, while the ```push``` method adds items to the stack.

#### Pros

 + It is easy to implement and logical for beginners.
 + It allows you to control how memory is allocated.
 + Easier to use than queues.

#### Cons

 + Neither flexible nor scalable.
 + Random access to elements in a stack is nearly impossible.

#### A typical stack must contain the following methods:

 + pop(): this method removes an element from the top of the stack and returns it.
 + push(): this method adds an element to the top of the stack.


# Queue

A Queue is also a linear structure that follows a ```First In First Out (FIFO) order```, but they differ in how elements are removed. 

Queues are open from both ends: one end for inserting data (```enqueue```), and the other end for removing data (```dequeue```). A stack is only open from one end.


So far, we learned about the Linear Queue. The other two queues are:

* ```Circular Queue```: In a circular queue, the last element is connected to the first element to form a circle. Initially, the front and rear parts of the queue point to the same location, but they move apart as more elements are inserted into the queue.

* ```Priority Queue```: In priority queues, elements are sorted based on priority. The most important element appears first, and the least important appears last. It is also used in load balancing in operating system.

#### Pros

 + Queues are flexible.
 + They can handle multiple data types.
 + Data queues are fast and optimized.

#### Cons

 + Inserting/ removing elements from the middle is complex.
 + Queues are not readily searchable.


#### A queue allows for the following operations:

 + ```enqueue()```: this method adds an element to the end/rear of the queue
 + ```dequeue()```: this method removes an element from the front of the queue
 + ```top()```: returns the first element in the queue
 + ```initialize()```: creates an empty queue



