# Exp.No:5  
## Constructors - Parameterized Constructor

---

### AIM  
To Write a python code to implement a parameterised constructor that will initialize the name and age of the student and print the details using user defined function.

---

### ALGORITHM

1. Begin the program.  
2. Define a `person` class.  
3. The `person` class should have a parameterized `__init__` method that accepts two parameters: `name` and `userid`.  
4. Inside the `__init__` method, assign the `name` to `self.name` and the `userid` to `self.userid`.  
5. Print the `self.userid`.  
6. Prompt the user to enter their `name` (string) and `userid`.  
7. Create an instance `s1` of the `person` class by passing the entered `name` and `userid` to the constructor.  
8. Terminate the program.

---

### PROGRAM

```
class Student:
    def __init__(self, name, age):
        self.name = name
        self.age = age

    def display(self):
        print("Student name is :", self.name)
        print("Student age is : ", self.age)

name = input()
age = input()
s = Student(name, age)
s.display()

```

### OUTPUT
<img width="892" height="185" alt="image" src="https://github.com/user-attachments/assets/dcf31636-fd5a-4dcf-9a7f-92f0821d88bc" />

### RESULT:
Thus a python code to implement a parameterised constructor that will initialize the name and age of the student and print the details using user defined function.
