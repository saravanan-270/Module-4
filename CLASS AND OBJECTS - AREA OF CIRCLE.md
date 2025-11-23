# Exp.No:16  
## DICTIONARY - SIZE OF DICTIONARY

---

### AIM  
To write a Python program to print the size of a dictionary using `getsizeof()` from the `sys` module.

---

### ALGORITHM

1. Begin the program.  
2. Import the `sys` module to use the `getsizeof()` function.  
3. Define the dictionaries with key-value pairs (`dic1`, `dic2`, `dic3`).  
4. Use `sys.getsizeof()` to calculate the memory size of each dictionary.  
5. Print the size of each dictionary in bytes.  
6. Terminate the program.

---

### PROGRAM

```python
import sys
dic1 = {"A": 1, "B": 2, "C": 3} 

dic2 = {"Geek1": "Raju", "Geek2": "Nikhil", "Geek3": "Deepanshu"}

dic3 = {1: "Lion", 2: "Tiger", 3: "Fox", 4: "Wolf"}

print(f"Size of dic1: {sys.getsizeof(dic1)}bytes")
print(f"Size of dic2: {sys.getsizeof(dic1)}bytes")
print(f"Size of dic3: {sys.getsizeof(dic1)}bytes")


```

### OUTPUT
<img width="585" height="240" alt="image" src="https://github.com/user-attachments/assets/e9ba3287-c659-4687-841a-8aab788d04e7" />


### RESULT
Thus the python program to print the size of a dictionary using `getsizeof()` from the `sys` module has been implemented and executed successfully.
