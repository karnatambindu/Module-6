# Exp.No:6B COUNTER CLASS
# AIM
To write a Python program to create a Counter class that can increment the value of a counter.

# ALGORITHM
1. Start the Program.
2. Define the Counter class. Initialize the current variable with 0.
3. Define the increment() method to increment the value of current by 1. Define the value() method to return the current value of current. Define the reset() method to reset the current value back to 0. Create a counter object of the Counter class. C
4. all the increment() method three times to increment the counter.
5. Call the value() method and print the result to show the current counter value.
6. End the program.

# PROGRAM
```
class Counter:
    def __init__(self):   # constructor (initializes object attributes)
        self.current = 0

    def increment(self):  # increases counter value by 1
        self.current += 1

    def value(self):      # returns the current counter value
        return self.current

    def reset(self):      # resets counter back to 0
        self.current = 0


counter = Counter()      # create a new Counter object
counter.increment()      # now current = 1
counter.increment()      # now current = 2
counter.increment()      # now current = 3

print(counter.value())   # prints 3
```
# OUTPUT
<img width="652" height="162" alt="image" src="https://github.com/user-attachments/assets/323e26f0-977d-43b6-87d2-8a3ca1bea9b4" />

# RESULT
Thus the program to create a class that can increment the value of a counter has been implemented and executed successfully.
