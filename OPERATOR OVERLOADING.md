# Exp.No:27  
## Operator Overloading

---

### AIM  
To write a Python program to perform division of two complex numbers using the binary '/' operator overloading. Class name: `Complex`, where the objects `Ob1 = Complex(10, 21)` and `Ob2 = Complex(2, 3)` represent complex numbers.

---

### ALGORITHM

1. **Start the Program.**
2. **Define the Complex class**:
   - Define the constructor `__init__()` to accept two parameters: `real` and `imag` (representing the real and imaginary parts of the complex number).
   - Assign these values to `self.real` and `self.imag` respectively.
3. **Define the `__truediv__()` method** to perform the division of two complex numbers:
   - Calculate the real part of the result as the division of `self.real` by `other.real`.
   - Calculate the imaginary part of the result as the division of `self.imag` by `other.imag`.
   - Return a new Complex object with the calculated real and imaginary parts.
4. **Define the `__repr__()` method** to represent the complex number as a string.
   - Return a string formatted to display the real and imaginary parts with one decimal place using `f"{self.real:.1f}, {self.imag:.1f}"`.
5. **Create two objects of the Complex class**:
   - `Ob1 = Complex(10, 21)` represents the complex number `10 + 21i`.
   - `Ob2 = Complex(2, 3)` represents the complex number `2 + 3i`.
6. **Perform the division operation**: Use the `/` operator to divide `Ob1` by `Ob2`. This will call the `__truediv__()` method.
7. **Print the result**: Print the result of the division, which will be formatted by the `__repr__()` method.
8. **End the Program.**

---

### PROGRAM

```
Reg.No: 212223060120
Name: KAVIYA PRIYA K

class Complex:
    def __init__(self,real,imag):
        self.real=real
        self.imag=imag
    def __add__(self,other):
        real_part=self.real*other.real
        imag_part=self.imag*other.imag
        return(real_part,imag_part)
obj1=Complex(1, 2)
obj2=Complex(2, 3)
print(obj1+obj2)

```

### OUTPUT
<img width="402" height="216" alt="image" src="https://github.com/user-attachments/assets/734bd2a8-dafb-4af8-9bca-0b8ef2de3b05" />

### RESULT
Thus, the program to overload the addition operator for complex numbers was executed successfully and the output was verified.

