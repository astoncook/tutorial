```py
class Stacks:

    def __init__(self):
        self.stack = []

    def push(self, item):
        return self.stack.append(item)
        #code added

    def pop(self):
        return self.stack.pop()
        #code added

    x = Stack()
    x.push('red')
    x.push('blue')
    x.pop()
    x.push('yellow')
    x.pop()
    print(self.stack) # Answer [red]

```
Go back to [Stacks](1-topic.md)