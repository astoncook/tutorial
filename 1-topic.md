# Stacks

## Introduction
Stacks are a very important way for us to store items in First-In/Last-Out or Last-In/First-out. We can add a new varrible in one end and remove the varrible from the same end.

We can use this data structure in the real world for things like:

* Undo button on websites
* Back and foward opperations on browsers
* Language processing on programs

In simple terms we have two main functions associated with stack. Those are "Push" and "Pop". There are many more, but for today we will talk about the main two.

![Stack](pictures/stack-picture.png)

## Push

For pushing elements, we need to use the append() method on the elements to push the element to the top of the stack. Here is a basic example of using append():

```py
stack = []

stack.append(1) #adds 1
stack.append(10) #adds 10
stack.append(100) #adds 100
stack.append(1000) #adds 1000

print(stack)
# [ 1, 10, 100, 1000]
```
## Pop

Pop is a term to remove a element from the stack. You can use the element to remove the top element from the stack. Here is an example of me using the last data points from the push example:

```py
print(stack.pop()) #removes 1000
print(stack.pop()) #removes 100
print(stack.pop()) #removes 10

print(stack)
# [ 1]
```

## Efficiency
Push | Pop
 --- | ---
O(1) | O(1)
To keep it simple push and pop do not run any loops so the efficency is O(1).

## Example
Try this problem yourself and write on a paper line by line to keep track of this problem:

```py
stack[]

stack.append(1)
stack.append(10)
stack.pop()
stack.append(100)
stack.append(1000)
stack.pop()
stack.pop()
stack.append(10000)
stack.append(100000)
stack.pop()

# What remains
print(stack)
```
<details>
<summary markdown="span">Solution To Practice Example</summary>

```py
stack = []

stack.append(1) # [1]
stack.append(10) # [1, 10]
stack.pop() # [1]
stack.append(100) # [1, 100]
stack.append(1000) # [1, 100, 1000]
stack.pop() # [1, 100]
stack.pop() # [1]
stack.append(10000) # [1, 10000]
stack.append(100000) # [1, 10000, 100000]
stack.pop() # [1, 10000]

# What remains
print(stack) # [1, 10000] Final Answer
```
</details>

## Problem To Solve: Stacks

Now its time to show what you have learned!

I have created a more complex stack using a class called "Stacks" and some functions corresponding with the class. Finish the code for the functions to print out correctly.

```py
class Stacks:

    def __init__(self):
        self.stack = []

    def push(self, value):
        # Add code here

    def pop(self):
        # Add code here

    x = Stack()
    x.push('red')
    x.push('blue')
    x.pop()
    x.push('yellow')
    x.pop()
    print(self.stack)

```
Solution to [Problem To Solve](answers/stack-answer.md)

Go to [Welcome Page](0-welcome.md)!