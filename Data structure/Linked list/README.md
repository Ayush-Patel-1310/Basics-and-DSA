
# Listed list 

Linked lists are a sequential collection of data that uses relational pointers on each data node to link to the next node in the list.

Linked list, Queue, Stack are linear data structure but the main difference between linked list and (List,Queue,stack,string) is positioning, listed list are not continuous and list,queue,stack and string are continuous allocated in memory location.

The first node in a linked list is called the head node, and the final is called the tail node, which has a null pointer.

You can think of linked lists like a chain; individual links only have a connection to their immediate neighbors but all the links together form a larger structure.


Lets implement linked list
```
class Node:
    data = 0
    add = None
    def __init__(self,data);
        self.data = data
        sel.add = None


class List:
    root = None

    def append(s, data):
        t = Node(data)
        if not s.root:
            s.root = t
            return
        x = s.root
        while x.add:
            x = x.add
        x.add = t

    def display(s):
        x = s.root
        if x == None:
            return 0
        while x.add:
            print(x.data, end=' -> ')
            x = x.add
        print(x.data)

    def __len__(s):
        if not s.root:
            return 0
        count = 1
        x = s.root
        while x.add:
            count += 1
            x = x.add
        return count

    def pop(s):
        if not s.root:
            print("Dor kat chuki hai")
            return
        elif s.root.add == None:
            s.root = None
            print("Khali ho gaya")
            return
        x = s.root
        while x.add.add:
            x = x.add
        x.add = None

    def zpend(s, data):
        t = Node(data)
        if s.root == None:
            s.root = t
            return
        t.add = s.root
        s.root = t

    def fpop(s):
        if s.root == None:
            print("Khali hai bhai")
        s.root = s.root.add

    def index(s, key):
        if s.root == None:
            print("Empty dear")
        x = s.root
        c = 0
        while x:
            if x.data == key:
                print(x.data, c)
                return
            c += 1
            x = x.add
        print("Not found dear")
        return -1

    def insert_2(s, index, data):
        t = Node(data)
        if s.root == None:
            s.append(data)
        n = len(s)
        if index < 0:
            index = n + index
        if index >= n:
            s.append(data)
        if index <= 0:
            s.zpend(data)
            return
        x = s.root
        while index - 1:
            x = x.add
            index -= 1
        t.add = x.add
        x.add = t
        s.display()

    def __iter__(s):
        s.c = s.root
        return s

    def __next__(s):
        if s.c!=None:
            t = s.c.data
            s.c = s.c.add
            return t
        raise StopIteration()

    def sort(s):
        if not s.root:
            return
        n = len(s)
        for i in range(4,0,-1):
            x = s.root
            u = i
            while i-1:
                x=x.add
                i-=1
            val = x.data
            k=n-u
            j=x.add
            while k and val>j.data:
                x.data = j.data
                j = j.add
                x = x.add
                k -= 1
            x.data = val
        s.display()

l = List()
l.append(5)
l.append(4)
l.append(3)
l.insert_2(-900,2)
l.insert_2(-1000, 1)
l.sort()
```


### Pros

 + Efficient insertion and deletion of new elements
 + Simpler to reorganize than arrays
 + Useful as a starting point for advanced data structures like graphs or trees

### Cons

 + Storage of pointers with each data point increases memory usage
 + Must always traverse the linked list from Head node to find a specific element


#### There are many types of linked list as follow:
 
 + Singly Linked List
 + Doubly Linked List
 + Circular Linked List
 + Doubly Circular Linked link
