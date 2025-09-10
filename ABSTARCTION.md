# Exp.No:6A Abstraction
# AIM
To write a Python program to define the abstract base class named Polygon and also define the abstract method. This base class is inherited by various subclasses. Implement the abstract method in each subclass. Create objects of the subclasses and invoke the sides() method.

# ALGORITHM
1. Start the Program.
2. Import the ABC class from the abc module to implement abstraction.
3. Define the abstract base class Polygon: Inherit from ABC (Abstract Base Class).
4. Define an abstract method sides() with no implementation. Define the Triangle class that inherits from Polygon: Implement the sides() method to print "Triangle has 3 sides".
5. Define the Pentagon class that inherits from Polygon: Implement the sides() method to print "Pentagon has 5 sides". Define the Hexagon class that inherits from Polygon: Implement the sides() method to print "Hexagon has 6 sides". Define the Square class that inherits from Polygon: Implement the sides() method to print "I have 4 sides".
6. Create an object t of the Triangle class and call the sides() method to print the number of sides. Create an object s of the Square class and call the sides() method to print the number of sides.
7. Create an object p of the Pentagon class and call the sides() method to print the number of sides. Create an object k of the Hexagon class and call the sides() method to print the number of sides.
8. End the Program.

# PROGRAM
Reg-212223060113 Name-Karnatam Bindu
```
from abc import ABC  
  
class Polygon(ABC):   
  
   # abstract method   
   def sides(self):   
      pass  
  
class Triangle(Polygon):   
  
     
   def sides(self):   
      print("Triangle has 3 sides")   
  
class Pentagon(Polygon):   
    def sides(self):
        print("Pentagon has 5 sides")
   #Add code here
class Hexagon(Polygon):  
    def sides(self):
        print("Hexagon has 6 sides")
  
   #Add your code
class square(Polygon):   
  
   def sides(self):   
      print("I have 4 sides")   
  
# Driver code   
t = Triangle()   
s = square()  
p = Pentagon()   
k = Hexagon()   
t.sides ()
s.sides ()
p.sides ()
k.sides ()
```
# OUTPUT
<img width="1210" height="270" alt="image" src="https://github.com/user-attachments/assets/616a877e-2f1f-49c9-b512-370083e90d6c" />


# RESULT
Thus the program to define the abstract base class and also define the abstract method has been implemented and executed successfully.
