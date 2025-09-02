# Exp.No:22  
## Destructor

---

### AIM  
To create a Python class `Student` with a destructor.

---

### ALGORITHM
1. Begin the program.
2. Define the Student class.
3. Inside the Student class:
   a) Define the __init__ method (constructor) to initialize the object with name and age.
      - Store the values in instance variables self.name and self.age.
      - Print the message: "My name is {self.name} and I am {self.age} years old."
   b) Define the __del__ method (destructor) to display a message when the object is deleted.
      - Print the message: "{self.name} student is deleted."
4. Create an object s of the Student class using:
      s = Student("Vishvajit Rao", 22)
   - This automatically calls the constructor (__init__) and prints the student's details.
5. Use the del statement to delete the object s.
   - This triggers the destructor (__del__), and the message confirming deletion is printed.
6. Terminate the program.


---

### PROGRAM

```
class Student:
    def __init__(self, name, age):
        self.name = name
        self.age = age
        print(f"My name is {self.name} and I am {self.age} years old.")

    def __del__(self):
        print(f"{self.name} student is deleted.")

s = Student("Vishvajit Rao", 22)
```

### OUTPUT
<img width="1160" height="192" alt="image" src="https://github.com/user-attachments/assets/5a2c97fe-ff14-469c-a497-510ae16b5a85" />


### RESULT
Thus a python program to create a Python class `Student` with a destructor has been executed successfully.
