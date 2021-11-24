# Stacks

## Introduction
Stacks are a very important way for us to store items in First-In/Last-Out or Last-In/First-out. We can add a new varrible in one end and remove the varrible from the same end.

We can use this data structure in the real world for things like:

* Undo button on websites
* Back and foward opperations on browsers
* Language processing on programs

In simple terms we have two main functions associated with stack. Those are "Push" and "Pop". There are many more, but for today we will talk about the main two.

![Stack](stack-picture.png)

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