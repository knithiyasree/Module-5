# Exp.No:23  
## Multiple Inheritance

---

### AIM  
To write a Python program to get the name, attendance, and ID of a student and check if they are eligible for the next module using multiple inheritance. If attendance > 80, the student is eligible; otherwise, not eligible.

---

### ALGORITHM

1. Define the `Student` class.
2. Inside the `Student` class, define the `__init__` method (constructor). The `__init__` method accepts two parameters: `name` and `student_id`.
    - Inside the `__init__` method: Assign the value of `name` to `self.name` and `student_id` to `self.student_id`.
3. Define the `get_student_info` method inside the `Student` class:
    - This method should return a string formatted with `self.name` and `self.student_id`.
4. Define the `Attendance` class, which inherits from the `Student` class.
5. Inside the `Attendance` class, define the `__init__` method (constructor).
    - The `__init__` method accepts three parameters: `name`, `student_id`, and `attendance`.
    - Inside the `__init__` method: Call the parent class constructor `super().__init__(name, student_id)` to initialize `name` and `student_id`. Assign the value of `attendance` to `self.attendance`.
6. Define the `check_eligibility` method inside the `Attendance` class:
    - If `self.attendance` is greater than 80, return a formatted string indicating the student is eligible for the module exam.
    - Otherwise, return a formatted string indicating the student is not eligible for the module exam.
7. Prompt the user to enter the `name` (as a string), `student_id` (as an integer), and `attendance` (as an integer).
8. Create an instance `student` of the `Attendance` class, passing the entered `name`, `student_id`, and `attendance` to the constructor.
9. Call the `check_eligibility` method on the `student` object and print the result.
10. Terminate the program.

---

### PROGRAM

```
class Parent:
   def __init__(self,name):
     self.name = name
   def getName(self):
     return self.name
class Child(Parent):
   def __init__(self,name,rollno):
     Parent.__init__(self,name)
     self.rollno = rollno
   def getrollno(self):
     return self.rollno
class Grandchild(Child):
   def __init__(self,name,rollno,p,c,m,b):
     Child.__init__(self,name,rollno)
     self.p=p
     self.c=c
     self.m=m
     self.b=b
   def gettotal(self):
       
     return self.p+ self.c+ self.m + self.b
name=input()
rollno=int(input())
p=int(input())
c=int(input())
m=int(input())
b=int(input())
gc = Grandchild(name,rollno,p,c,m,b)
av=gc.gettotal()
avg=av/4
print("Name: ",gc.getName(),"Rollno: " ,gc.getrollno(), "Total Marks out of 400: ",gc.gettotal())
print("Average :",avg)


```

### OUTPUT
<img width="1273" height="388" alt="Screenshot 2025-09-02 133051" src="https://github.com/user-attachments/assets/3d7fb626-ffee-4014-b7ee-20c86eef6a97" />


### RESULT:
Thus a a Python program to get the name, attendance, and ID of a student and check if they are eligible for the next module using multiple inheritance has been executed successfully.

