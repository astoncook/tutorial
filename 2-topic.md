# Sets

## Introduction
A set is used to store data and is very useful when dealing with soring big things in small places. In a more textbook definition it allows us to store multiple items in a single variable. But sets are also unordered to any specific order and the stored values are unchangeable.

Some simple opperators in sets are:

* Add
* Remove

We will be going over those in this lesson.

![Sets](pictures/set-picture.png)
## Basics of Sets
Sets are created and visulized by using curly brackets and inputing the data using basic set rules. Creating a empty set also requires the following: aset = set(). Here are some simple examples below.
```py
set1 = {1, 10, 100, 1000, -100} # These are all integers
set2 = {'hamburger', 'icecream', 'soda', 'cat', 'dog'} # These are  srting values
set3 = {True, False, True, True, False} # These are boolean values
set4 = {1, 'hambruger', True, -100, 'soda', False} # We can combine them too.
```

## Add
This is very simple. We can add items into the set using the add opperator. This opperator has a efficency of 0(1). Here is an example:
```py
set1 = {10, 100, 1000}
set1.add(10000) # Added 10000 to set1
set1.add(100000) # Added 100000 to set1
#set1 = {10, 100, 1000, 10000, 100000}
```
We can also add sets together by using the update opperator, but be careful, sets cannor have duplicates. I will show this in the example below.
```py
set1 = {10, 100, 1000}
set2 = {10, 200, 2000}

set1.update(set2)
#set1 = {10, 100, 200, 1000, 2000} 
```
## Remove
This is very simple. We can remove items into the set using the remove opperator. This opperator has a efficency of 0(1). Here is an example:
```py
set1 = {'hamburger', 10, 'soda', 100}

set1.remove('soda') # Removes cat from set1
set1.discard(10) # Discards cow from set1
# set1 = {'hamburger', 100}
```

## Efficiency
Operators | Efficency
 --- | ---
   Add | O(1)
Remove | O(1)
These two are very concistant. They run at an average efficency is O(1).

## Example
This example will help you practice with keeping trakc of the variables and remembering to not count the douplicate items in the sets. Look back to the reading above for some help.

```py
food = {'soda', 'hamburger', 'pizza', 'cheese', 'icecream'}
food.add('ice')
food.remove('soda')
food.remove('ice')
food.add('soda')
food.remove('cheese')
food.add('beef')
food.add('ketchup')
# What remains
```
<details>
<summary markdown="span">Solution To Practice Example</summary>

```py
food = {'soda', 'hamburger', 'pizza', 'cheese', 'icecream'}
food.add('ice') # {'soda', 'hamburger', 'pizza', 'cheese', 'icecream', 'ice'}
food.remove('soda') # {'hamburger', 'pizza', 'cheese', 'icecream', 'ice'}
food.remove('ice')  # {'hamburger', 'pizza', 'cheese', 'icecream'}
food.add('soda') # {'hamburger', 'pizza', 'cheese', 'icecream', 'soda'}
food.remove('cheese') # {'hamburger', 'pizza', 'icecream', 'soda'}
food.add('beef') # {'hamburger', 'pizza', 'icecream', 'soda', 'beef'}
food.add('ketchup') # {'hamburger', 'pizza', 'icecream', 'soda', 'beef', 'ketchup'}

#Solution is : {'hamburger', 'pizza', 'icecream', 'soda', 'beef'}
```
</details>

## Problem To Solve: Sets
Now its time to show what you have learned!

I have created a more complex set using some functions corresponding with the set. Finish the code for the functions to print out correctly.
```py
def add_sets(set1, set2):
    # Update or add one set to the other.

def remove_even(set1):
    # Remove even numbers in a set.

def remove_odd(set1):
    # Remove odd numbers in a set.

sul1 = {1, 6, 9, 10}
sul2 = {10, 100, 1000, 1000}
sul3 = {2, 3, 4, 5}

print(add_sets(sul1, sul2)) # {1, 6, 9, 10, 100, 1000, 10000}
print(add_sets(sul1, sul3)) # {1, 2, 3, 4, 5, 6, 9, 10}
print(add_sets(sul2, sul3)) # {1, 10, 20, 25, 30, 35, 40}
print(remove_odd(sul1)) # {6, 10}
print(remove_odd(sul2)) # {10, 100, 1000, 10000}
print(remove_even(su3)) # {3, 5}
print(remove_even(sul1)) # {1, 9}
```
Solution to [Problem To Solve](answers/set-answer.md)

Go to [Welcome Page](0-welcome.md)!