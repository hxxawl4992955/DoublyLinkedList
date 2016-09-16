## Doubly Linked List

#### Materials

The material you need is the source code of a uni-threaded linked list. [code repo](https://github.com/iss-java/DoublyLinkedList.git).<br>


#### Readings

You are expected to read about how the following things are done in Java. 
- create a thread
- start a thread
- protect critical data

At least, you have to master the usage of `Mutex`. If you apply an advanced synchronization mechanism, such as 
a `reader-writer lock`, to improve the degree of concurrency - you will get extra credits.

#### Requirements

**Requirement A**<br>
> Refactor `Node` with a locking(synchronization) mechanism you like, ensuring that the `data` field of a `Node` will not be corrupted if read/written by multiple threads. Also, write a test case which starts multiple threads to read/write same nodes.

**Requirement B**<br>
> Refactor `MyList` with a locking mechanism you like, ensuring that the data structure of doubly-linked list will not be corrupted if some nodes are inserted/deleted by multiple threads. Also, write a test case which starts multiple threads to insert into / delete from the same list.

**Requirement C**<br>
> Refactor `Node` and `MyList` to ensure that insertion and removal can only be applied to nodes that belongs to the caller linked list.

#### Submission

Push your improved version to **your own** Git repo. This repo should be **private** and enroll us TAs as **collaborators**. Read the comments in the code carefully, and don't modify the original directory structure and the class structure. However, you can rename the project root folder and add your own functions as you like.
