# Notes 19

## sorted(list) vs list.sort()  
* `sorted()` Returns a new sorted list, original list unchanged.
* `list.sort()` Sorts in-place, returns None. Faster (cuz dont have to create copy).  

Use sorted() if you need the orignal position.  
Use list.sort() if you want to mutate the list.

## Dictionary
**Creating an empty dictionary**
```python 
data = {} # or data = dict()
```
