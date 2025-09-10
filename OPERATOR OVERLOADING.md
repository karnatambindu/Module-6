# Exp.No:6E Operator Overloading
# AIM
To write a Python program to perform division of two complex numbers using the binary '/' operator overloading. Class name: Complex, where the objects Ob1 = Complex(10, 21) and Ob2 = Complex(2, 3) represent complex numbers.

# ALGORITHM
1. Start the Program.
2. Define the Complex class: Define the constructor init() to accept two parameters: real and imag (representing the real and imaginary parts of the complex number).
3. Assign these values to self.real and self.imag respectively.
4. Define the truediv() method to perform the division of two complex numbers: Calculate the real part of the result as the division of self.real by other.real.
5. Calculate the imaginary part of the result as the division of self.imag by other.imag. Return a new Complex object with the calculated real and imaginary parts. Define the repr() method to represent the complex number as a string.
6. Return a string formatted to display the real and imaginary parts with one decimal place using f"{self.real:.1f}, {self.imag:.1f}".
7. Create two objects of the Complex class: Ob1 = Complex(10, 21) represents the complex number 10 + 21i. Ob2 = Complex(2, 3) represents the complex number 2 + 3i. Perform the division operation: Use the / operator to divide Ob1 by Ob2.
8. This will call the truediv() method. Print the result: Print the result of the division, which will be formatted by the repr() method.
9. End the Program.

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
<img width="612" height="184" alt="image" src="https://github.com/user-attachments/assets/d1607f10-0779-4273-8bf9-0b3ec1922fe5" />

# RESULT
Thus the program to perform division of two complex numbers using the binary '/' operator overloading has been implemented and executed successfully.


