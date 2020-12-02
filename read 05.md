# *Linked List*


*A linked list is a sequence of data elements, which are connected together via links. Each data element contains a connection to another data element in form of a pointer. Python does not have linked lists in its standard library. We implement the concept of linked lists using the concept of nodes.*
*Each element of a linked list is called a node, and every node has two different fields:*

*1.Data contains the value to be stored in the node.*

*2.Next contains a reference to the next node on the list.*

*A linked list is a collection of nodes. The first node is called the head, and it’s used as the starting point for any iteration through the list. The last node must have its next reference pointing to None to determine the end of the list.*

***Why Linked List?***
> *Arrays can be used to store linear data of similar types, but arrays have the following limitations.*

- *The size of the arrays is fixed: So we must know the upper limit on the number of elements in advance. Also, generally, the allocated memory is equal to the upper limit irrespective of the usage.*
- *Inserting a new element in an array of elements is expensive because the room has to be created for the new elements and to create room existing elements have to be shifted.*

**Advantages over arrays:**

*1.Dynamic size*

*2.Ease of insertion/deletion*

<hr>

***Linear data structures***
*If we really want to understand the basics of linked lists, it’s important that we talk about what type of data structure they are. One characteristic of linked lists is that they are linear data structures, which means that there is a sequence and an order to how they are constructed and traversed.*
*Similarly*, when we use arrays in our code, we’re implementing a linear data structure! It can be helpful to think of arrays and linked lists as being similar in the way that we sequence data. In both of these structures, order matters. But what makes arrays and linked lists different?*


