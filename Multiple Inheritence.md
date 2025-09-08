# Arithmetic Operations Using Multiple Inheritance in Python

This Python program demonstrates **multiple inheritance** by performing basic arithmetic operations — Addition, Subtraction, and Division — using three classes.

## 🎯 Aim

To write a Python program to calculate **Add, Sub & Division** using **Multiple Inheritance**.

## 🧠 Algorithm

1. **Define `Calculation1` class**
   - Contains `Summation(a, b)` method to return the sum of two numbers.
2. **Define `Calculation2` class**
   - Contains `Subtraction(a, b)` method to return the difference of two numbers.
3. **Define `Derived` class**
   - Inherits from both `Calculation1` and `Calculation2`.
   - Contains `Division(a, b)` method to return the division result.
4. **Input**
   - Prompt the user to enter two numbers.
5. **Process**
   - Create an object of the `Derived` class.
   - Call `Summation`, `Subtraction`, and `Division` methods.
6. **Output**
   - Display the results of the three operations.

## 💻 Program 
~~~
class Addition:
   def add(self, a, b):
      return a + b
class Subtraction:
   def subtract(self, a, b):
      return a - b
class Calculator(Addition, Subtraction):
   def divide(self, a, b):
      if b != 0:
         return a / b
      else:
         return "Division by zero error!"
a = int(input())
b = int(input())
calc = Calculator()
print(calc.add(a, b))
print(calc.subtract(a, b))
print(calc.divide(a, b))
~~~
## Output 

<img width="707" height="266" alt="image" src="https://github.com/user-attachments/assets/51406dfa-2717-4eb4-b06d-b86d6663d240" />

## Result
Thus, the program has been executed successfully.
