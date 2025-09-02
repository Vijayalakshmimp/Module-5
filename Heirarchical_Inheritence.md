# Hierarchical Inheritance in Python

This Python project demonstrates **Hierarchical Inheritance** using a base class `Details` and two derived classes `Employee` and `Patient`. The program collects and displays details for both employees and patients.

## 🎯 Aim

To write a Python program that uses **Hierarchical Inheritance** to input and display **Employee** and **Patient** details.

## 📘 Description

- **Base Class:** `Details`
  - Stores common attributes: `name`, `age`
  - Provides methods: `getName()`, `getAge()`

- **Derived Class 1:** `Employee`
  - Inherits from `Details`
  - Adds: `employee_id`, `department`
  - Method: `getEmployeeDetails()`

- **Derived Class 2:** `Patient`
  - Inherits from `Details`
  - Adds: `patient_id`, `disease`
  - Method: `getPatientDetails()`

## 🧠 Algorithm

1. Create base class `Details` with common attributes.
2. Create `Employee` class extending `Details`, adding employee-specific data.
3. Create `Patient` class extending `Details`, adding patient-specific data.
4. Get user input for employee and patient data.
5. Display collected information using class methods.

## Program
class Details:

def get_basic_details(self, id, name, gender):

    self.id = id
    
    self.name = name
    
    self.gender = gender
class Employee(Details):

def get_employee_details(self, company, department):

    self.company = company
    
    self.department = department

def display(self):
    
    print("Employee Object")
    
    print("Id: ", self.id)
    
    print("Name: ", self.name)
    
    print("Gender: ", self.gender)
    
    print("Company: ", self.company)
    
    print("Department: ", self.department)
    
    print()
class Patient(Details):

def get_patient_details(self, hospital, department):

    self.hospital = hospital
    
    self.department = department

def display(self):
    
    print("Patient Object")
    
    print("Id: ", self.id)
    
    print("Name: ", self.name)
    
    print("Gender: ", self.gender)
    
    print("Hospital: ", self.hospital)
    
    print("Department: ", self.department)
    
    print()
eid = int(input())

ename = input()

egender = input()

company = input()

edept = input()

pid = int(input())

pname = input()

pgender = input()

hospital = input()

pdept = input()

emp = Employee()

emp.get_basic_details(eid, ename, egender)

emp.get_employee_details(company, edept)

pat = Patient()

pat.get_basic_details(pid, pname, pgender)

pat.get_patient_details(hospital, pdept)

emp.display()

pat.display()
## Sample Output
<img width="1150" height="454" alt="Screenshot 2025-09-02 131305" src="https://github.com/user-attachments/assets/97c141f0-673d-4bf9-a63d-9a0d25d998cb" />

## Result

Thus the Python program that uses **Hierarchical Inheritance** to input and display **Employee** and **Patient** details is executed and verified successfully.

