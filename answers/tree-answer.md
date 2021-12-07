```py
    def _insert(self, data, node):
        """
        This function will look for a place to insert a node
        with 'data' inside of it.  The current sub-tree is
        represented by 'node'.  This function is intended to be
        called the first time by the insert function.
        """
        if data < node.data:
            # Check left side.
            if node.left is None:
                # Find empty spot.
                node.left = node(data)
            else:
                # If not look again.
                self._insert(data, node.left)
        elif data > node.data:
            # Check the right side.
            if node.right is None:
                # Find empty spot.
                node.right = node(data)
            else:
                # Keep looking.
                self._insert(data, node.right)

tree.insert(5)
tree.insert(3)
tree.insert(7)
tree.insert(7)  
tree.insert(4)
tree.insert(10)
tree.insert(1)
tree.insert(6)
# The tree should print as follows.
for x in tree:
    print(x)  # 1, 3, 4, 5, 6, 7, 10
```
Go back to [Trees](https://github.com/astoncook/tutorial/blob/master/3-topic.md)