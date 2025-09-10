# Exp.No:6D Method Overriding
# AIM
To write a Python program to create a Parent class Bird and inherit two child classes Sparrow and Ostrich from the Bird class with the same method flight(). Create an object for each class and call the methods of the class which will print the name of the bird that is flying.

# ALGORITHM
1. Begin the program.
2. Define the Bird class: Create a method intro() to print "There are many types of birds.
3. Create a method flight() to print "Most of the birds can fly but some cannot.
4. Define the Sparrow class, which inherits from Bird: Override the flight() method.
5. Call the intro() method from the parent class. Print "Sparrows can fly." Define the Ostrich class, which inherits from Bird: Override the flight() method. Call the intro() method from the parent class. Print "Ostriches cannot fly."
6. Create an object obj_bird of the Bird class.
7. Create an object obj_spr of the Sparrow class.
8.  Create an object obj_ost of the Ostrich class.
9.  Print the general message "There are many types of birds." Call the flight() method on each object (obj_bird, obj_spr, obj_ost) to display the respective messages.
10.  Terminate the program.

# PROGRAM
```
class Bird:
    def intro(self):
        print("There are many types of birds.")

    def flight(self):
        print("Most of the birds can fly but some cannot.")


class sparrow(Bird):   # inherits from Bird
    def flight(self):  # overrides the flight() method
        print("Sparrows can fly.")


class ostrich(Bird):   # inherits from Bird
    def flight(self):  # overrides the flight() method
        print("Ostriches cannot fly.")


# Objects
bird = Bird()
spr = sparrow()
ost = ostrich()

bird.intro()   # call Bird's intro()
bird.flight()  # call Bird's flight()
spr.intro()    # inherited from Bird
spr.flight()   # overridden in sparrow
bird.intro()   # Bird's intro again
ost.flight()   # overridden in ostrich
```
# OUTPUT
<img width="826" height="269" alt="image" src="https://github.com/user-attachments/assets/91b564b2-5757-466d-a1c5-3638ca8586f7" />

# RESULT
Thus the program to create a Parent class and inherit two child classes from the class with the same method has been implemented and executed successfully.
