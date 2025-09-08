# Multilevel Inheritance Example in Python

This Python project demonstrates the concept of **Multilevel Inheritance** to collect and display the **name**, **age**, and **location** of a person.

## 🎯 Aim

To write a Python program that uses multilevel inheritance to get and display a person’s name, age, and location.

## 🧠 Algorithm

1. **Parent Class**  
   - `__init__(name)` initializes the `name` attribute.  
   - `getName()` returns the `name`.

2. **Child Class (inherits Parent)**  
   - `__init__(name, age)` initializes `name` using `super()` and adds `age`.  
   - `getAge()` returns the `age`.

3. **Grandchild Class (inherits Child)**  
   - `__init__(name, age, location)` initializes `name` and `age` using `super()` and adds `location`.  
   - `getLocation()` returns the `location`.

4. **Input & Output**  
   - Take user input for name, age, and location.  
   - Create an instance of `Grandchild`.  
   - Print all details using class methods.

## Program
~~~
class Parent:
   def init(self,name):
      self.name = name
   def getName(self):
      return self.name
class Child(Parent):
   def init(self,name,age):
       Parent.__init__(self,name)
       self.age = age
   def getAge(self):
      return self.age
class Grandchild(Child):
   def init(self,name,age,sal):
      Child.__init__(self,name,age)
      self.sal=sal
   def getsal(self):
      return self.sal
name=input()
age=int(input())
sal=int(input())
gc = Grandchild(name,age,sal)
print(gc.getName(), gc.getAge(), gc.getsal())
~~~

## Output
<img width="765" height="247" alt="image" src="https://github.com/user-attachments/assets/06f207dd-2cca-4c0f-9b5b-e44d65052232" />

## Result
Thus, the program has been executed successfully.
