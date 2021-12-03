```py
def add_sets(set1, set2):
    # Update or add one set to the other.
    set1.update(set2)
def remove_even(set1):
    # Remove even numbers in a set.
    for i in set1:
        if i % 2 == 0: # If the number is equal and divisible to 2, then it is removed.
            set1.remove(i)
def remove_odd(set1):
    # Remove odd numbers in a set.
    for i in set1:
        if i % 2 != 0: # Same topic. If the number doesnt equal 2, then it is removed.
            set1.remove(i)

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
Go back to [Sets](https://github.com/astoncook/tutorial/blob/master/2-topic.md)