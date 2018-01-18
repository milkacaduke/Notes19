# Notes 19

## sorted(list) vs list.sort()  
* `sorted()` Returns a new sorted list, original list unchanged.
* `list.sort()` Sorts in-place, returns None. Faster (cuz dont have to create copy).  

Use sorted() if you need the orignal position.  
Use list.sort() if you want to mutate the list.

## Dictionary
**Creating an empty dictionary**
```python 
data = {} 
# or 
data = dict()
```
**Creating a dictionary with initial values**
```python
data = {'a':1, 'b':2, 'c':3}
# or
data = dict(a=1, b=2, c=3)
# or
data = {k:v for k, v in(('a', 1), ('b', 2), ('c',3))}
```
    
**Inserting/Updating a single value**
```python
data['a'] = 1   # Updates if 'a' exists, else adds 'a'
# or
data.update({'a':1})
# or
data.update(dict(a=1))
# or
data.update(a=1)
```
    
**Inserting/Updating multi value**
```python
data.update({'c':3, 'd':4})   # Updates 'c' and adds 'd'
```

**Creating a merged dictionary without modifying original**
```python
data3 = {}
data3.update(data)  # Modifies data3, not data
data3.update(data2)  # Modifies data3, not data2
```

**Deleting items in dictionary**
```python
del data[key]  # Removes specific element in a dictionary
data.pop(key)  # Removes the key & returns the value
data.clear()  # Clears entire dictionary
```

**Iterate through pairs in a dictionary**
```python
for key in data: # Iterates just through the keys, ignore value
for key, value in d.item(): # Iterates through the pairs
```

**Check if a key is already in dictionary**
```python
key in data
```

 
## Binary Search Tree
**Inorder Successor in Binary Search Tree**  
In Binary Tree, Inorder successor of a node is the next node in Inorder traversal of the Binary Tree.  
In Binary Search Tree, Inorder Successor of an input node can also be defined as the node with the smallest key greater than the key of input node.
    
**How to find Inorder Successor in Binary Search Tree?**  
1. Method 1 (Uses Parent Pointer)
    Assume that every node has parent pointer
    - If right subtree of node is not NULL, then succ lies in right subtree.
    - If right subtree of node is NULL, then succ is one of the ancestors.
2. Method 2 (Search from root)

[ref](https://www.geeksforgeeks.org/inorder-successor-in-binary-search-tree/)

**Inorder vs Preorder vs Postorder**  
**....A  
..B...C**

ABC vs BAC vs ACB





