# Exp.No:19  
## CLASS AND OBJECTS - AREA OF CIRCLE

---

### AIM  
To write a Python program to take the radius from the user and find the area of a circle using the class name `pen` and function name `stationary`.

---

### ALGORITHM

1. Begin the program.  
2. Create a class named `pen`.  
3. Define a method `rain(self, r)` inside the class `pen` that accepts a radius `r` as an argument.  
4. Inside the `stationary` method:  
   - Calculate the area of a circle using the formula:  
     \[ \text{Area} = \pi \times r^2 \]  
   - Use the `math.pi` constant to get the value of π and perform the calculation.  
   - Print the result, formatted to two decimal places.  
5. Prompt the user for an integer input to represent the radius of the circle.  
6. Create an instance of the `pen` class and store it in the variable `u`.  
7. Call the `stationary` method of the `pen` class, passing the user-provided radius `r` as an argument.  
8. Terminate the program.

---

### PROGRAM

```python
class Pen:
    @staticmethod
    def stationary(radius):
        pi = 3.141591
        area = pi * radius ** 2
        return area

# Get user input for radius
try:
    radius = float(input())
    if radius < 0:
        print("Radius cannot be negative. Please enter a positive value.")
    else:
        area = Pen.stationary(radius)
        print(f"Area of circle: {area:.2f}")
except ValueError:
    print("Invalid input. Please enter a valid numeric value for the radius.")




```

### OUTPUT
<img width="632" height="202" alt="image" src="https://github.com/user-attachments/assets/9eacc504-8d13-41e1-96d4-dae28c60348a" />


### RESULT
Thus the python program for ind the area of a circle using the class name `pen` and function name `stationary` has been implemented and executed successfully.
