#  Traversing a linked list and checking :

In a linked list, we have a series of connected nodes, each containing data and a reference to the next node.
We can't use regular loops (like foreach or for) to go through the list, so we depend on the "Next" property in each node to guide us to the next node.

We use a while() loop to traverse the list. This loop keeps running as long as the current node is not null.
If we try to traverse a null node, it causes an issue, so the loop helps us avoid that.

We have a variable called "Current" that tells us where we are in the linked list.
We move forward in the list by updating "Current" to the next node.


```plaintext
Start with the head of the list
┌─> Node 1: Check value, not the one we're looking for
│
├─> Node 2: Check value, not the one we're looking for
│
├─> Node 3: Check value, found the one we're looking for
│
└─> End of the list
```

Example

```python 
CheckIfValueExists(value)
  Set Current to the beginning of the list (Head)

  While Current is not null
    If the value in the current node is equal to the target value
      Return true (we found the value)

    Move to the next node by updating Current to Current.Next

  If the loop finishes and we haven't found the value
    Return false (value is not in the list)

```

Resources

[Search an element in a Linked List (Iterative and Recursive)](https://www.geeksforgeeks.org/search-an-element-in-a-linked-list-iterative-and-recursive/)

