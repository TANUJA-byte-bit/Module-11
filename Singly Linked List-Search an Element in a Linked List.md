# 11d)  Singly Linked List-To Search an Element in a Linked List

This project contains a simple implementation of a **singly linked list** in Python, allowing insertion and searching of elements.

---

##  Aim

To write a Python program to search for a given element in a singly linked list using object-oriented programming principles.

---

##  Algorithm

1. **Define a Node class** with `data` and `next` attributes.
2. **Define a LinkedList class** with:
   - A `head` pointer initialized to `None`.
   - A `push()` method to add elements at the beginning.
   - A `search()` method to check whether a given value exists.
3. Create a `LinkedList` instance.
4. Insert the elements **10, 30, 11, 21, 14** using `push()` (which results in reverse order).
5. Read an integer input from the user.
6. Use `search()` to check if the element exists in the list.
7. Output **"Yes"** if found, else **"No"**.

---

##  Program
```
class Node:
    def __init__(self, data=None):
        self.data = data
        self.next = None


class singly_linked_list:
    def __init__(self):
        self.head = None

    def append_item(self, data):
        node = Node(data)
        node.next = self.head
        self.head = node

    def iterate_item(self):
        temp = self.head
        while temp is not None:
            print(temp.data)
            temp = temp.next

    def search_item(self, val):
        temp = self.head
        while temp is not None:
            if temp.data == val:
                return True
            temp = temp.next
        return False


items = singly_linked_list()
items.append_item('PHP')
items.append_item('Python')
items.append_item('C#')
items.append_item('C++')
items.append_item('Java')

items.iterate_item()

data = input()

if items.search_item(data):
    print("True")
else:
    print("False")
```
## Sample Output
<img width="367" height="452" alt="image" src="https://github.com/user-attachments/assets/d89a323f-31c4-4b4a-a2a2-3ab9912c0ed0" />

## Result
Program executed Successfully.
