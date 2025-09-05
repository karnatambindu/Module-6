# Exp.No:28 Abstraction

# AIM
To write a Python program to define the abstract base class named Polygon and also define the abstract method. This base class is inherited by various subclasses. Implement the abstract method in each subclass. Create objects of the subclasses and invoke the sides() method.

# ALGORITHM
Start the Program.
Import the ABC class from the abc module to implement abstraction.
Define the abstract base class Polygon:
Inherit from ABC (Abstract Base Class).
Define an abstract method sides() with no implementation.
Define the Triangle class that inherits from Polygon:
Implement the sides() method to print "Triangle has 3 sides".
Define the Pentagon class that inherits from Polygon:
Implement the sides() method to print "Pentagon has 5 sides".
Define the Hexagon class that inherits from Polygon:
Implement the sides() method to print "Hexagon has 6 sides".
Define the Square class that inherits from Polygon:
Implement the sides() method to print "I have 4 sides".
Create an object t of the Triangle class and call the sides() method to print the number of sides.
Create an object s of the Square class and call the sides() method to print the number of sides.
Create an object p of the Pentagon class and call the sides() method to print the number of sides.
Create an object k of the Hexagon class and call the sides() method to print the number of sides.
End the Program.
# PROGRAM
```
Reg-212223060113 Name-Karnatam Bindu
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
<img width="1210" height="270" alt="Screenshot 2025-09-05 213526" src="https://github.com/user-attachments/assets/1bd02039-b3ab-4906-abd0-05d3acc72768" />

# RESULT
Thus the program to define the abstract base class and also define the abstract method has been implemented and executed successfully.

# Exp.No:30 COUNTER CLASS
# AIM
To write a Python program to create a Counter class that can increment the value of a counter.

# ALGORITHM
Start the Program.
Define the Counter class.
Initialize the current variable with 0.
Define the increment() method to increment the value of current by 1.
Define the value() method to return the current value of current.
Define the reset() method to reset the current value back to 0.
Create a counter object of the Counter class.
Call the increment() method three times to increment the counter.
Call the value() method and print the result to show the current counter value.
End the program.

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
<img width="652" height="162" alt="Screenshot 2025-09-05 215449" src="https://github.com/user-attachments/assets/d3c2047e-5143-4762-9872-dc1932fdebbb" />

# RESULT
Thus the program to create a class that can increment the value of a counter has been implemented and executed successfully.

# Exp.No:29 Encapsulation
# AIM
To write a Python program to create a class Student with the private members name and age, and add getter and setter methods to initialize and modify the age variable.

# ALGORITHM
Start the Program.
Define the Student class.
Inside the Student class, define the __init__ method to initialize name and the private member __age.
Define a getter method get_age to return the value of the private member __age.
Define a setter method set_age to set a new value to the private member __age.
Create an object stud of the Student class with the name 'Jessa' and age 14.
Print the name and the age of stud using the getter method.
Use the setter method set_age to change the age of stud to 16.
Print the name and the updated age of stud using the getter method.
End the program.
# PROGRAM
```
class Student:
    def __init__(self, name, roll_no, age):
        self.name = name
        self.__roll_no = roll_no   # private variable
        self.__age = age           # private variable

    def show(self):
        print('Student Details:', self.name, self.__roll_no)

    def get_roll_no(self):        # getter method
        return self.__roll_no

    def set_roll_no(self, number):  # setter method
        if number > 50:
            print('Invalid roll no. Please set correct roll number')
        else:
            self.__roll_no = number


# Create an object
jessa = Student('Jessa', 10, 15)

jessa.show()           # prints current details
jessa.set_roll_no(52)  # tries to set roll_no = 52 (invalid)
jessa.set_roll_no(25)  # sets roll_no = 25 (valid)
jessa.show()           # prints updated details
```

# OUTPUT
<img width="947" height="221" alt="Screenshot 2025-09-05 215741" src="https://github.com/user-attachments/assets/82783c0a-86bd-405c-b663-2a6029a72192" />

# RESULT
Thus the program to create class with private members and add getter and setter methods to initialize and modify the given variable has been implemented and executed successfully.

# Exp.No:26 Method Overriding
# AIM
To write a Python program to create a Parent class Bird and inherit two child classes Sparrow and Ostrich from the Bird class with the same method flight(). Create an object for each class and call the methods of the class which will print the name of the bird that is flying.
# ALGORITHM
Begin the program.
Define the Bird class:
Create a method intro() to print "There are many types of birds."
Create a method flight() to print "Most of the birds can fly but some cannot."
Define the Sparrow class, which inherits from Bird:
Override the flight() method.
Call the intro() method from the parent class.
Print "Sparrows can fly."
Define the Ostrich class, which inherits from Bird:
Override the flight() method.
Call the intro() method from the parent class.
Print "Ostriches cannot fly."
Create an object obj_bird of the Bird class.
Create an object obj_spr of the Sparrow class.
Create an object obj_ost of the Ostrich class.
Print the general message "There are many types of birds."
Call the flight() method on each object (obj_bird, obj_spr, obj_ost) to display the respective messages.
Terminate the program.
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
<img width="826" height="269" alt="Screenshot 2025-09-05 220016" src="https://github.com/user-attachments/assets/5f2eaf3e-960a-487a-a0f6-bd6b0f928b85" />

# RESULT
Thus the program to create a Parent class and inherit two child classes from the class with the same method has been implemented and executed successfully.

# Exp.No:27 Operator Overloading
# AIM
To write a Python program to perform division of two complex numbers using the binary '/' operator overloading. Class name: Complex, where the objects Ob1 = Complex(10, 21) and Ob2 = Complex(2, 3) represent complex numbers.
# ALGORITHM
Start the Program.
Define the Complex class:
Define the constructor __init__() to accept two parameters: real and imag (representing the real and imaginary parts of the complex number).
Assign these values to self.real and self.imag respectively.
Define the __truediv__() method to perform the division of two complex numbers:
Calculate the real part of the result as the division of self.real by other.real.
Calculate the imaginary part of the result as the division of self.imag by other.imag.
Return a new Complex object with the calculated real and imaginary parts.
Define the __repr__() method to represent the complex number as a string.
Return a string formatted to display the real and imaginary parts with one decimal place using f"{self.real:.1f}, {self.imag:.1f}".
Create two objects of the Complex class:
Ob1 = Complex(10, 21) represents the complex number 10 + 21i.
Ob2 = Complex(2, 3) represents the complex number 2 + 3i.
Perform the division operation: Use the / operator to divide Ob1 by Ob2. This will call the __truediv__() method.
Print the result: Print the result of the division, which will be formatted by the __repr__() method.
End the Program.
# PROGRAM
```
class complex:
    def init(self,a,b):
        self.a=a
        self.b=b

    def add(self,other):
        return self.a/other.a, self.b/other.b

obj1=complex(10,21)
obj2=complex(2,3)
print(obj1+obj2)
```
# OUTPUT
<img width="612" height="184" alt="Screenshot 2025-09-05 220504" src="https://github.com/user-attachments/assets/cfb9e5cb-fa8e-44ef-8c6d-647cb48f0017" />

# RESULT
Thus the program to perform division of two complex numbers using the binary '/' operator overloading has been implemented and executed successfully.

