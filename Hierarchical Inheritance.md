# Exp.No:5  
## Hierarchical Inheritance

---

### AIM  
To write a Python program to get the employee and doctor details and display them using hierarchical inheritance. Create a parent (base) class named `Details` and two child (derived) classes named `Employee` and `Doctor`.

---

### ALGORITHM
1. Begin the program.
2. Create a base class `Details`:
   - Define `get_info()` to initialize id, name, gender, hospital, and department.
3. Create a derived class `Doctor`:
   - Inherit from `Details`.
   - Define `display()` to print doctor details.
4. Create a derived class `Patient`:
   - Inherit from `Details`.
   - Define `display()` to print patient details.
5. Accept input for doctor details: id1, name1, gender1, hospital1, department1.
6. Accept input for patient details: id2, name2, gender2, hospital2, department2.
7. Create a `Doctor` object and call `get_info()`.
8. Create a `Patient` object and call `get_info()`.
9. Call `display()` for the doctor object.
10. Call `display()` for the patient object.
11. Terminate the program.


---

### PROGRAM
```
class Details:
    def get_info(self, id, name, gender, hospital, department):
        self.id = id
        self.name = name
        self.gender = gender
        self.hospital = hospital
        self.department = department

class Doctor(Details):
    def display(self):
        print("Doctor Object")
        print("Id: ", self.id)
        print("Name: ", self.name)
        print("Gender: ", self.gender)
        print("Hospital: ", self.hospital)
        print("Department: ", self.department)

class Patient(Details):
    def display(self):
        print("Patient Object")
        print("Id: ", self.id)
        print("Name: ", self.name)
        print("Gender: ", self.gender)
        print("Hospital: ", self.hospital)
        print("Department: ", self.department)

# Input for Doctor
id1 = int(input())
name1 = input()
gender1 = input()
hospital1 = input()
department1 = input()

# Input for Patient
id2 = int(input())
name2 = input()
gender2 = input()
hospital2 = input()
department2 = input()

# Create objects and call methods
doctor = Doctor()
doctor.get_info(id1, name1, gender1, hospital1, department1)

patient = Patient()
patient.get_info(id2, name2, gender2, hospital2, department2)

# Output
doctor.display()
print()
patient.display()


```

### OUTPUT  
<img width="607" height="443" alt="image" src="https://github.com/user-attachments/assets/c9444201-8821-448c-8a74-b17d12c1ff4d" />



### RESULT:
Thus a python program to the given program has been executed successfully.
