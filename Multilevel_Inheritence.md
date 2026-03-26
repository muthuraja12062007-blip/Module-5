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
## Parent Class
class Parent: def init(self, name): self.name = name

def getName(self):
    return self.name
## Child Class (inherits Parent)
class Child(Parent): def init(self, name, age): super().init(name) self.age = age

def getAge(self):
    return self.age
## Grandchild Class (inherits Child)
class Grandchild(Child): def init(self, name, age, location): super().init(name, age) self.location = location

def getLocation(self):
    return self.location
## Take user input
name = input("Enter name: ") age = int(input("Enter age: ")) location = input("Enter location: ")

## Create object
obj = Grandchild(name, age, location)

## Print details
print("\nDetails:") print("Name:", obj.getName()) print("Age:", obj.getAge()) print("Location:", obj.getLocation())

## Sample Output
![WhatsApp Image 2026-03-27 at 1 13 43 AM](https://github.com/user-attachments/assets/af4941d0-8d98-4d53-925e-fb94a0380a35)

## Result
Thus the program was successfully executed.and obtained the result.

